---
title: Criar baseTask
description: Crie um novo objeto baseTask em uma baseTaskList específica.
author: devindrajit
ms.localizationpriority: medium
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 03d3ab9a0a16f1f2b16cf3aed5321fed8c535c76
ms.sourcegitcommit: c900d22144429ac7aecae3355a4cdc1987cc4234
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/13/2021
ms.locfileid: "61424783"
---
# <a name="create-basetask"></a>Criar baseTask
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Crie um novo [objeto baseTask](../resources/basetask.md) em uma [baseTaskList específica.](../resources/basetasklist.md)

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)|Tasks.ReadWrite|
|Delegada (conta pessoal da Microsoft)|Tasks.ReadWrite|
|Aplicativo|Sem suporte|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/tasks/lists/{baseTaskListId}/tasks
POST /users/{userId|userPrincipalName}/tasks/lists/{baseTaskListId}/tasks
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON do [objeto baseTask.](../resources/basetask.md)

Você pode especificar as seguintes propriedades ao criar **uma baseTask**.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|corpo|[itemBody](../resources/itembody.md)|Corpo da tarefa que normalmente contém informações sobre a tarefa.|
|createdDateTime|DateTimeOffset|A data no fuso horário especificado que a tarefa foi concluída.|
|lastModifiedDateTime|DateTimeOffset|A data e hora da última modificação da tarefa. Por padrão, está definida em UTC. Você pode fornecer um fuso horário personalizado no cabeçalho da solicitação. O valor da propriedade usa o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1º de janeiro de 2020 teria esta aparência: '2020-01-01T00:00:00Z'.|
|bodyLastModifiedDateTime|DateTimeOffset|A data e hora da última modificação da tarefa. Por padrão, está definida em UTC. Você pode fornecer um fuso horário personalizado no cabeçalho da solicitação. O valor da propriedade usa o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1º de janeiro de 2020 teria esta aparência: '2020-01-01T00:00:00Z'.|
|completedDateTime|DateTimeOffset|A data no fuso horário especificado que a tarefa foi concluída.|
|dueDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)|A data no fuso horário especificado que a tarefa será concluída.|
|startDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)|A data no fuso horário especificado que a tarefa será iniciada.|
|importância|importância|A importância da tarefa. Os valores possíveis são: `low`, `normal`, `high`.|
|recurrence|[patternedRecurrence](../resources/patternedrecurrence.md)|O padrão de recorrência da tarefa.|
|displayName|String|Uma breve descrição da tarefa.|
|status|taskStatus_v2|Indica o estado ou o andamento da tarefa. Os valores possíveis são: `notStarted`, `inProgress`, `completed`, `unknownFutureValue`. Obrigatório.|
|personalProperties|[personalTaskProperties](../resources/personaltaskproperties.md)|Propriedades que são pessoais para um usuário, como reminderDateTime.|



## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código `201 Created` de resposta e um objeto [baseTask](../resources/basetask.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "create_basetask_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/tasks/lists/AQMkAGVjMzJmMWZjLTgyYjgtNGIyNi1hOGQ0LWRjMjNmMGRmOWNi/tasks
Content-Type: application/json
Content-length: 634

{
  "@odata.type": "#microsoft.graph.baseTask",
  "body": {
    "@odata.type": "microsoft.graph.itemBody"
  },
  "bodyLastModifiedDateTime": "String (timestamp)",
  "completedDateTime": "String (timestamp)",
  "dueDateTime": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone"
  },
  "startDateTime": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone"
  },
  "importance": "String",
  "recurrence": {
    "@odata.type": "microsoft.graph.patternedRecurrence"
  },
  "displayName": "String",
  "status": "String",
  "personalProperties": {
    "@odata.type": "microsoft.graph.personalTaskProperties"
  }
}
```


### <a name="response"></a>Resposta
**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.baseTask"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.type": "#microsoft.graph.task",
    "@odata.etag": "W/\"kOO4xOT//0qFRAqk3TNe0QAABCE1Xg==\"",
    "importance": "normal",
    "status": "notStarted",
    "displayName": "Buy medicine",
    "createdDateTime": "2021-11-17T10:11:18.0229364Z",
    "lastModifiedDateTime": "2021-11-17T10:11:18.19789Z",
    "id": "AAkALgAAAAAAHYQDEapmEc2byACqAC",
    "body": {
        "content": "",
        "contentType": "text"
    },
    "parentList": {
        "id": "AQMkAGVjMzJmMWZjLTgyYjgtNGIyNi1hOGQ0LWRjMjNmMGRmOWNi"
    }
}
```

