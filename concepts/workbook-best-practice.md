---
title: Práticas recomendadas para trabalhar com a API do Excel
description: Encontre dicas para trabalhar com APIs do Excel no Microsoft Graph. Saiba como gerenciar sessões, trabalhar com APIs que levam muito tempo para serem concluídas e reduzir erros de limitação.
author: grangeryy
ms.localizationpriority: medium
ms.prod: excel
ms.openlocfilehash: 6f2b3a0a9c0213098a9a6a214b03e448050a3a1d
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66447020"
---
# <a name="best-practices-for-working-with-the-excel-api"></a>Práticas recomendadas para trabalhar com a API do Excel

Este artigo fornece recomendações para trabalhar com as [APIs do Excel](/graph/api/resources/excel) no Microsoft Graph.

## <a name="manage-sessions-in-the-most-efficient-way"></a>Gerenciar sessões da maneira mais eficiente

Se você tiver mais de uma chamada para fazer dentro de um determinado período de tempo, recomendamos que você crie uma sessão e passe a ID da sessão com cada solicitação. Para representar a sessão na API, use o cabeçalho `workbook-session-id: {session-id}`. Ao fazer isso, você pode usar as APIs do Excel da maneira mais eficiente.

O exemplo a seguir mostra como adicionar um novo número a uma tabela e localizar um registro em uma pasta de trabalho usando essa abordagem.

### <a name="step-1-create-a-session"></a>Etapa 1: Criar uma sessão

#### <a name="request"></a>Solicitação

```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/createSession
Content-type: application/json

{
  "persistChanges": true
}
```

#### <a name="response"></a>Resposta

A seguir está uma resposta bem-sucedida.

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "persistChanges": true
}
```

### <a name="step-2-add-a-new-row-to-the-table"></a>Etapa 2: Adicionar uma nova linha à tabela

#### <a name="request"></a>Solicitação

```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/Table1/rows/add
Content-type: application/json
workbook-session-id: {session-id}

{
  "values": [[“east”, “pear”, 4]]
}
```

#### <a name="response"></a>Resposta

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "index": 6,
  "values": [[“east”, “pear”, 4]]
}
```

### <a name="step-3-look-up-a-value-in-the-updated-table"></a>Etapa 3: Pesquisar um valor na tabela atualizada

#### <a name="request"></a>Solicitação

```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/functions/vlookup
Content-type: application/json
workbook-session-id: {session-id}

{
    "lookupValue":"pear",
    "tableArray":{"Address":"Sheet1!B2:C7"},
    "colIndexNum":2,
    "rangeLookup":false
}
```

#### <a name="response"></a>Resposta

```http
HTTP code: 200 OK
content-type: application/json

{
    "value": 5
}
```

### <a name="step-4-close-the-session-after-all-the-requests-are-completed"></a>Etapa 4: Fechar a sessão depois que todas as solicitações forem concluídas

#### <a name="request"></a>Solicitação

```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/closeSession
Content-type: application/json
workbook-session-id: {session-id}

{
}
```

#### <a name="response"></a>Resposta

```http
HTTP/1.1 204 No Content
```

Para obter mais detalhes, consulte [Criar sessão e](/graph/api/workbook-createsession) [fechar sessão](/graph/api/workbook-closesession).

## <a name="work-with-apis-that-take-a-long-time-to-complete"></a>Trabalhar com APIs que levam muito tempo para serem concluídas

Você pode observar que algumas operações levam um tempo indeterminado para serem concluídas; por exemplo, abrir uma pasta de trabalho grande. É fácil atingir o tempo limite enquanto aguarda a resposta a essas solicitações. Para resolver esse problema, fornecemos o padrão de operação de execução longa. Ao usar esse padrão, você não precisa se preocupar com o tempo limite para a solicitação.

Atualmente, a API do Excel de criação de sessão no Microsoft Graph tem o padrão de operação de execução longa habilitado. Esse padrão envolve as seguintes etapas:

1. Adicione um `Prefer: respond-async` cabeçalho à solicitação para indicar que ela é uma operação de execução longa quando você cria uma sessão.
2. Uma operação de execução longa retornará uma `202 Accepted` resposta junto com um cabeçalho Location para recuperar o status da operação. Se a criação da sessão for concluída em vários segundos, ela retornará uma resposta de sessão de criação regular em vez de usar o padrão de operação de execução longa.
3. Com a `202 Accepted` resposta, você pode recuperar o status da operação no local especificado. Os valores de status da `notStarted`operação incluem `running`, `succeeded`e `failed`.
4. Depois que a operação for concluída, você poderá obter o resultado da criação da sessão por meio da URL especificada na resposta bem-sucedida.

O exemplo a seguir cria uma sessão usando o padrão de operação de execução longa.

### <a name="initial-request-to-create-session"></a>Solicitação inicial para criar sessão

#### <a name="request"></a>Solicitação

```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{drive-item-id}/workbook/worksheets({id})/createSession
Prefer: respond-async
Content-type: application/json
{
    "persistChanges": true
}
```

#### <a name="response"></a>Resposta
O padrão de operação de execução longa retornará uma `202 Accepted` resposta semelhante à seguinte.

```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/v1.0/me/drive/items/{drive-item-id}/workbook/operations/{operation-id}
Content-type: application/json

{
}
```

Em alguns casos, se a criação for bem-sucedida em segundos, ela não entrará no padrão de operação de execução longa; em vez disso, ele retorna como uma sessão de criação regular e a solicitação bem-sucedida retornará uma `201 Created` resposta.

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "persistChanges": true
}
```

O exemplo a seguir mostra a resposta quando a solicitação falha.

>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

```http
HTTP/1.1 500 Internal Server Error
Content-type: application/json

{
  "error":{
    "code": "internalServerError",
    "message": "An internal server error occurred while processing the request.",
    "innerError": {
      "code": "internalServerErrorUncategorized",
      "message": "An unspecified error has occurred.",
      "innerError": {
        "code": "GenericFileOpenError",
        "message": "The workbook cannot be opened."
      }
    }
  }
}
```

### <a name="poll-status-of-the-long-running-create-session"></a>Status da sondagem da sessão de criação de execução longa

Com o padrão de operação de execução longa, você pode obter o status de criação no local especificado usando a solicitação a seguir. O intervalo sugerido para sondar o status é de cerca de 30 segundos. O intervalo máximo não deve ser superior a 4 minutos.

#### <a name="request"></a>Solicitação

```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{drive-item-id}/workbook/operations/{operation-id}
{
}
```

#### <a name="response"></a>Resposta

A seguir está a resposta quando a operação tem um status de `running`.

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": {operation-id},
    "status": "running"
}
```

A seguir está a resposta quando o status da operação é `succeeded`.

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": {operation-id},
    "status": "succeeded",
    "resourceLocation": "https://graph.microsoft.com/v1.0/me/drive/items/{drive-item-id}/workbook/sessionInfoResource(key='{key}')
}
```

A seguir está a resposta quando o status da operação é `failed`.

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": {operation-id},
  "status": "failed",
  "error":{
    "code": "internalServerError",
    "message": "An internal server error occurred while processing the request.",
    "innerError": {
      "code": ""internalServerErrorUncategorized",
      "message": "An unspecified error has occurred.",
      "innerError": {
        "code": "GenericFileOpenError",
        "message": "The workbook cannot be opened."
      }
    }
  }
}
```

Para obter mais detalhes sobre erros, consulte [Códigos de erro e mensagens](workbook-error-codes.md#error-codes-and-messages).

### <a name="acquire-session-information"></a>Adquirir informações da sessão

#### <a name="request"></a>Solicitação

Com um status de `succeeded`, você pode obter as informações de sessão criadas `resourceLocation` com uma solicitação semelhante à seguinte.

```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{drive-item-id}/workbook/sessionInfoResource(key='{key}')
{
}
```

#### <a name="response"></a>Resposta
Esta é a resposta.

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "id-value",
    "persistChanges": true
}
```

> [!NOTE]
> A aquisição de informações da sessão depende da solicitação inicial. Você não precisará adquirir o resultado se a solicitação inicial não retornar um corpo de resposta.

## <a name="reduce-throttling-errors"></a>Reduzir erros de limitação

As APIs do Excel no Microsoft Graph afetam o uso de recursos de vários serviços de dependência. O impacto pode variar entre solicitações diferentes: por exemplo, você pode esperar que a atualização de uma cadeia de caracteres curta em uma única célula de uma pasta de trabalho pequena consumiria menos recursos do que adicionar uma tabela grande com fórmulas complexas a uma pasta de trabalho grande.

Mesmo com a mesma API, os parâmetros e as pastas de trabalho de destino podem introduzir diferenças significativas. Portanto, a limitação da API do Excel não é definida com números de limite simples e universais, pois resultariam em limites mais restritivos. As práticas recomendadas a seguir ajudarão você a concluir tarefas mais rapidamente com menos erros de limitação.

### <a name="retry-after-header"></a>Retry-After cabeçalho

Em muitos casos, uma resposta de limitação inclui um `Retry-After` cabeçalho. Respeitar o valor do cabeçalho e atrasar solicitações semelhantes ajudaria o cliente a se recuperar da limitação. Para obter detalhes sobre como lidar com respostas de erro de APIs do Excel no Microsoft Graph, consulte Tratamento de erros para [APIs do Excel no Microsoft Graph](workbook-error-handling.md).

### <a name="throttling-and-concurrency"></a>Limitação e simultaneidade

Outro fator relacionado à limitação é a simultaneidade de solicitação. Não recomendamos aumentar a simultaneidade ao usar APIs do Excel (por exemplo, paralelizar as solicitações para a mesma pasta de trabalho), especialmente para solicitações de gravação. Em vez disso, a menos que haja uma preocupação específica, como sobrecarga de rede significativa em comparação com o tempo de execução de solicitação muito curto, recomendamos o uso sequencial no caso mais comum: para cada pasta de trabalho, envie apenas a próxima solicitação depois de receber uma resposta bem-sucedida à solicitação atual.

As solicitações de gravação simultâneas para a mesma pasta de trabalho geralmente não são executadas em paralelo (embora, em alguns casos, elas sim); em vez disso, elas geralmente são a causa da limitação, do tempo limite (quando as solicitações são enfileiradas em servidores), do conflito de mesclagem (quando sessões simultâneas estão envolvidas) e de outros tipos de falhas. Eles também complicam o tratamento de erros; por exemplo, quando você recebe uma resposta de falha, não há como confirmar o status de outras solicitações pendentes, o que dificulta determinar ou recuperar o estado da pasta de trabalho.

## <a name="see-also"></a>Confira também

* [Usar a API REST do Excel](/graph/api/resources/excel)