---
title: Práticas recomendadas para APIs do Excel no Microsoft Graph
description: Listar as práticas recomendadas e exemplos para as APIs do Excel no Microsoft Graph
author: grangeryy
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: c113d162874c3121e97534b8d098d1c52a24fe77
ms.sourcegitcommit: f26428bce3034e206b901e9c747cffcf64b55882
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47651292"
---
# <a name="best-practices-for-working-with-the-excel-api-in-microsoft-graph"></a>Práticas recomendadas para trabalhar com a API do Excel no Microsoft Graph

Este artigo fornece recomendações para trabalhar com as APIs do Excel no Microsoft Graph.

## <a name="manage-sessions-in-the-most-efficient-way"></a>Gerenciar sessões da maneira mais eficiente

Se você tiver mais de uma chamada para fazer dentro de um determinado período de tempo, recomendamos que você crie uma sessão e passe a ID da sessão com cada solicitação. Para representar a sessão na API, use o cabeçalho `workbook-session-id: {session-id}`. Fazendo isso, você pode usar as APIs do Excel da maneira mais eficiente.

O exemplo a seguir mostra como adicionar um novo número a uma tabela e localizar um registro em uma pasta de trabalho usando essa abordagem.

### <a name="step-1-create-a-session"></a>Etapa 1: criar uma sessão

#### <a name="request"></a>Solicitação

```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/createSession
Content-type: application/json
Content-length: 52

{
  "persistChanges": true
}
```
#### <a name="response"></a>Resposta

A seguir está uma resposta bem-sucedida.

```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "persistChanges": true
}
```

### <a name="step-2-add-a-new-row-to-the-table"></a>Etapa 2: adicionar uma nova linha à tabela

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
Content-length: 42

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

### <a name="step-4-close-the-session-after-all-the-requests-are-completed"></a>Etapa 4: fechar a sessão após todas as solicitações serem concluídas

#### <a name="request"></a>Solicitação

```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/closeSession
Content-type: application/json
workbook-session-id: {session-id}
Content-length: 0

{
}
```

#### <a name="response"></a>Resposta

```http
HTTP/1.1 204 No Content
```

Para obter mais detalhes, consulte [criar sessão](/graph/api/workbook-createsession?view=graph-rest-1.0) e [fechar sessão](/graph/api/workbook-closesession?view=graph-rest-1.0).

## <a name="working-with-apis-that-take-a-long-time-to-complete"></a>Trabalhar com APIs que levar muito tempo para ser concluído

Você pode notar que algumas operações levam um tempo indeterminado para a conclusão; por exemplo, abrir uma pasta de trabalho grande. É fácil atingir o tempo limite enquanto aguarda a resposta para essas solicitações. Para resolver esse problema, fornecemos o padrão de operação de longa execução. Ao usar esse padrão, você não precisa se preocupar com o tempo limite da solicitação.

Atualmente, a API do Excel de criação de sessão no Microsoft Graph tem o padrão de operação de execução demorada habilitado. Este padrão envolve as seguintes etapas:

1. Adicione um `Prefer: respond-async` cabeçalho à solicitação para indicar que é uma operação de execução demorada quando você faz uma sessão.
2. Uma operação de execução longa retornará uma `202 Accepted` resposta junto com um cabeçalho de local para recuperar o status da operação. Se a criação da sessão for concluída em vários segundos, ela retornará uma resposta de criação de sessão regular em vez de usar o padrão de operação de longa execução.
3. Com a `202 Accepted` resposta, você pode recuperar o status da operação no local especificado. Os valores de status de operação incluem `notStarted` ,, `running` `succeeded` e `failed` .
4. Após a conclusão da operação, você pode obter o resultado da criação da sessão através da URL especificada na resposta bem-sucedida.

O exemplo a seguir cria uma sessão usando o padrão de operação de longa execução.

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

Em alguns casos, se a criação for bem-sucedida em segundos, ela não irá inserir o padrão de operação de longa execução; em vez disso, ele retorna como uma sessão de criação regular e a solicitação bem-sucedida retornará uma `201 Created` resposta.

```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 52

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

### <a name="poll-status-of-the-long-running-create-session"></a>Status de pesquisa da sessão de criação de execução longa


Com o padrão de operação de execução longa, você pode obter o status de criação no local especificado usando a seguinte solicitação. O intervalo sugerido para o status da pesquisa é de cerca de 30 segundos. O intervalo máximo não deve ser superior a 4 minutos.

#### <a name="request"></a>Solicitação

```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{drive-item-id}/workbook/operations/{operation-id}
{
}
```

#### <a name="response"></a>Resposta

A seguir está a resposta quando a operação tem um status de `running` .

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": {operation-id},
    "status": "running"
}
```

A seguir está a resposta quando o status da operação é `succeeded` .

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": {operation-id},
    "status": "succeeded",
    "resourceLocation": "https://graph.microsoft.com/v1.0/me/drive/items/{drive-item-id}/workbook/sessionInfoResource(key='{key}')
}
```

A seguir está a resposta quando o status da operação é `failed` .

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

Para obter mais detalhes sobre erros, consulte [códigos de erro](/concepts/workbook-error-codes.md)

### <a name="acquire-session-information"></a>Obter informações de sessão

#### <a name="request"></a>Solicitação

Com o status de `succeeded` , você pode obter as informações da sessão criada por meio de `resourceLocation` uma solicitação semelhante à seguinte.

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

>**Observação:** Obter informações de sessão depende da solicitação inicial. Você não precisará adquirir o resultado se a solicitação inicial não retornar um corpo de resposta.
