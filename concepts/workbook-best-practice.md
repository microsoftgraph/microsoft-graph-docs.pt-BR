---
title: Práticas recomendadas para Excel APIs no Microsoft Graph
description: Listar práticas recomendadas e exemplos para Excel APIs no Microsoft Graph
author: grangeryy
ms.localizationpriority: medium
ms.prod: excel
ms.openlocfilehash: 8f1dc872dd94547545c3ca9d47ec08909119e0ea
ms.sourcegitcommit: 0e7927f34b7e55d323acbf281e11560cb40a89ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2022
ms.locfileid: "63672102"
---
# <a name="best-practices-for-working-with-the-excel-api-in-microsoft-graph"></a>Práticas recomendadas para trabalhar com a API Excel no Microsoft Graph

Este artigo fornece recomendações para trabalhar com as APIs Excel no Microsoft Graph.

## <a name="manage-sessions-in-the-most-efficient-way"></a>Gerenciar sessões da maneira mais eficiente

Se você tiver mais de uma chamada para fazer em um determinado período de tempo, recomendamos que você crie uma sessão e passe a ID da sessão com cada solicitação. Para representar a sessão na API, use o cabeçalho `workbook-session-id: {session-id}`. Ao fazer isso, você pode usar as APIs Excel de forma mais eficiente.

O exemplo a seguir mostra como adicionar um novo número a uma tabela e, em seguida, encontrar um registro em uma lista de trabalho usando essa abordagem.

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

A seguir, uma resposta bem-sucedida.

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

### <a name="step-3-look-up-a-value-in-the-updated-table"></a>Etapa 3: procurar um valor na tabela atualizada

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

### <a name="step-4-close-the-session-after-all-the-requests-are-completed"></a>Etapa 4: fechar a sessão depois que todas as solicitações são concluídas

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

Para obter mais detalhes, consulte [Create session and](/graph/api/workbook-createsession?view=graph-rest-1.0) [Close session](/graph/api/workbook-closesession?view=graph-rest-1.0).

## <a name="working-with-apis-that-take-a-long-time-to-complete"></a>Trabalhar com APIs que levam muito tempo para ser concluída

Você pode notar que algumas operações levam um tempo indeterminado para ser concluída; por exemplo, abrir uma grande workbook. É fácil atingir o tempo de espera enquanto aguarda a resposta a essas solicitações. Para resolver esse problema, fornecemos o padrão de operação de longa duração. Quando você usa esse padrão, não precisa se preocupar com o tempo de espera da solicitação.

Atualmente, a api de criação Excel sessão no Microsoft Graph tem o padrão de operação de longa execução habilitado. Esse padrão envolve as seguintes etapas:

1. Adicione um `Prefer: respond-async` header à solicitação para indicar que é uma operação de longa duração quando você engrada uma sessão.
2. Uma operação de longa duração retornará uma `202 Accepted` resposta juntamente com um header location para recuperar o status da operação. Se a criação da sessão for concluída em alguns segundos, ela retornará uma resposta de sessão de criação regular em vez de usar o padrão de operação de longa execução.
3. Com a `202 Accepted` resposta, você pode recuperar o status da operação no local especificado. Os valores de status da operação incluem `notStarted``running`, , `succeeded`e `failed`.
4. Depois que a operação for concluída, você poderá obter o resultado da criação da sessão por meio da URL especificada na resposta bem-sucedida.

O exemplo a seguir cria uma sessão usando o padrão de operação de longa duração.

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
O padrão de operação de longa duração retornará uma `202 Accepted` resposta semelhante à seguinte.

```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/v1.0/me/drive/items/{drive-item-id}/workbook/operations/{operation-id}
Content-type: application/json

{
}
```

Em alguns casos, se a criação for bem-sucedida em segundos, ela não entrará no padrão de operação de longa duração; em vez disso, ele retorna como uma sessão de criação regular e a solicitação bem-sucedida retornará uma `201 Created` resposta.

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

### <a name="poll-status-of-the-long-running-create-session"></a>Status da sondagem da sessão de criação de longa duração


Com o padrão de operação de longa duração, você pode obter o status de criação no local especificado usando a seguinte solicitação. O intervalo sugerido para o status da sondagem é de cerca de 30 segundos. O intervalo máximo não deve ser superior a 4 minutos.

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

Para obter mais detalhes sobre erros, consulte [Códigos de erro](workbook-error-codes.md#error-code).

### <a name="acquire-session-information"></a>Adquirir informações da sessão

#### <a name="request"></a>Solicitação

Com um status de `succeeded`, você pode obter as informações de sessão criadas com `resourceLocation` uma solicitação semelhante à seguinte.

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

>**Observação:** Adquirir informações da sessão depende da solicitação inicial. Você não precisa adquirir o resultado se a solicitação inicial não retornar um corpo de resposta.

## <a name="throttling"></a>Limitação

Excel APIs na Microsoft Graph afetar o uso de recursos de vários serviços de dependência. O impacto pode variar entre solicitações diferentes: por exemplo, você pode esperar que a atualização de uma cadeia de caracteres curta em uma única célula de uma pequena workbook consumiria menos recursos do que adicionar uma tabela grande com fórmulas complexas a uma grande lista de trabalho. Mesmo com a mesma API, os parâmetros e as guias de trabalho de destino podem apresentar diferenças significativas. Portanto Excel limitação da API não é definida com números de limite simples e universais, pois resultariam em limites mais restritivos. As práticas recomendadas a seguir ajudarão você a concluir tarefas mais rapidamente, com menos erros de throttling.

### <a name="retry-after-header"></a>Retry-After header

Em muitos casos, uma resposta de throttling inclui um `Retry-After` header. Respeitar o valor do header e atrasar solicitações semelhantes ajudaria o cliente a se recuperar da throttling. Para obter detalhes sobre como lidar com respostas de erro de Excel APIs no Microsoft Graph, consulte Tratamento de erros para [APIs Excel no Microsoft Graph](workbook-error-handling.md).

### <a name="throttling-and-concurrency"></a>Throttling and concurrency

Outro fator relacionado à throttling é a concurreência de solicitação. Não recomendamos aumentar a simulta ao usar apIs de Excel (por exemplo, paralelizar as solicitações para a mesma workbook), especialmente para solicitações de gravação. Em vez disso, a menos que haja uma preocupação específica, como sobrecarga de rede significativa em comparação com o tempo de execução de solicitação muito curto, recomendamos o uso sequencial no caso mais comum: para cada uma das guias de trabalho, envie apenas a próxima solicitação após receber uma resposta bem-sucedida à solicitação atual.

Solicitações de gravação simultâneas para a mesma lista de trabalho geralmente não são executados em paralelo (embora, em alguns casos, eles o fazem); em vez disso, eles geralmente são a causa da reação, do tempo de tempo (quando as solicitações são en filas em servidores), do conflito de mesclagem (quando sessões simultâneas estão envolvidas) e de outros tipos de falhas. Eles também complicam o tratamento de erros; por exemplo, quando você recebe uma resposta de falha, não há como confirmar o status de outras solicitações pendentes, o que torna difícil determinar ou recuperar o estado da workbook.
