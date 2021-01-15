---
title: Atualizar todoTask
description: Atualizar as propriedades de um objeto todoTask.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: bc3b5fc228d2c553dec3469825f74dfe4a5298ea
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49874274"
---
# <a name="update-todotask"></a>Atualizar todoTask
Namespace: microsoft.graph

Atualizar as propriedades de um [objeto todoTask.](../resources/todotask.md)

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|Tasks.ReadWrite|
|Delegado (conta pessoal da Microsoft)|Tasks.ReadWrite|
|Aplicativo|Sem suporte|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /me/todo/lists/{todoTaskListId}/tasks/{taskId}
PATCH /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks/{taskId}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON do [objeto todoTask.](../resources/todotask.md)

A tabela a seguir mostra as propriedades que são necessárias ao criar [todoTask](../resources/todotask.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O identificador exclusivo da tarefa. Herdado da [entidade](../resources/entity.md)|
|body|[itemBody](../resources/itembody.md)|Corpo da tarefa que normalmente contém informações sobre a tarefa. Observe para qual tipo de HTML há suporte.|
|completedDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)|A data no fuso horário especificado que a tarefa foi concluída.|
|dueDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)|A data no fuso horário especificado que a tarefa será concluída.|
|importância|importância|A importância do evento. Os valores possíveis são: `low`, `normal`, `high`.|
|isReminderOn|Booliano|Definido como verdadeiro se um alerta é definido para lembrar o usuário da tarefa.|
|recurrence|[patternedRecurrence](../resources/patternedrecurrence.md)|O padrão de recorrência da tarefa.|
|reminderDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)|A data e hora do alerta de lembrete da tarefa.|
|status|taskStatus|Indica o estado ou o progresso da tarefa. Os valores possíveis são: `notStarted`, `inProgress`, `completed`, `waitingOnOthers`, `deferred`.|
|title|Cadeia de caracteres|Uma breve descrição da tarefa.|
|createdDateTime|DateTimeOffset|A data e a hora da criação da tarefa. Por padrão, está definida em UTC. Você pode fornecer um fuso horário personalizado no cabeçalho da solicitação.|
|lastModifiedDateTime|DateTimeOffset|A data e hora da última modificação da tarefa. Por padrão, está definida em UTC. Você pode fornecer um fuso horário personalizado no cabeçalho da solicitação.|
|bodyLastModifiedDateTime|DateTimeOffset|A data e a hora em que o corpo da tarefa foi modificado pela última vez. Por padrão, está definida em UTC. Você pode fornecer um fuso horário personalizado no cabeçalho da solicitação.|



## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta e um objeto `200 OK` [todoTask](../resources/todotask.md) atualizado no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_todotask",
  "sampleKeys": ["AAMkADA1MTHgwAAA=", "721a35e2-35e2-721a-e235-1a72e2351a72"],
  "@odata.type": "microsoft.graph.todoTask"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/me/todo/lists/AAMkADA1MTHgwAAA=/tasks/721a35e2-35e2-721a-e235-1a72e2351a72
Content-Type: application/json
Content-length: 608

{
   "dueDateTime":{
      "dateTime":"2020-07-25T16:00:00",
      "timeZone":"Eastern Standard Time"
   }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-todotask-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-todotask-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-todotask-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-todotask-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Resposta
**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
   "@odata.type": "microsoft.graph.todoTask"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#tasks/$entity",
    "@odata.etag": "W/\"s8/ERWT3WEeFpBGD0bDgAA+TWq9g==\"",
    "importance": "low",
    "isReminderOn": false,
    "status": "notStarted",
    "title": "Shop for dinner",
    "createdDateTime": "2020-07-22T10:39:03.7937971Z",
    "lastModifiedDateTime": "2020-07-22T12:02:10.8835421Z",
    "id": "721a35e2-35e2-721a-e235-1a72e2351a72",
    "body": {
        "content": "",
        "contentType": "text"
    },
    "dueDateTime": {
        "dateTime": "2020-08-25T04:00:00.0000000",
        "timeZone": "UTC"
    }
}
   
```



