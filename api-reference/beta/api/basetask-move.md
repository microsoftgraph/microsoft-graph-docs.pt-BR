---
title: 'baseTask: move'
description: Mova um objeto baseTask de um baseTaskList para outro.
author: devindrajit
ms.localizationpriority: medium
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 313f4c330f8d239dc84e36917073124e146a3304
ms.sourcegitcommit: c900d22144429ac7aecae3355a4cdc1987cc4234
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/13/2021
ms.locfileid: "61424772"
---
# <a name="basetask-move"></a>baseTask: move
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Mova um [objeto baseTask](../resources/basetask.md) de [um baseTaskList](../resources/basetasklist.md) para outro.

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
POST /me/tasks/lists/{baseTaskListId}/tasks/{baseTaskId}/move
POST /users/{userId|userPrincipalName}/tasks/lists/{baseTaskListId}/tasks/{baseTaskId}/move

POST /me/tasks/alltasks/{baseTaskId}/move
POST /users/{userId|userPrincipalName}/tasks/alltasks/{baseTaskId}/move
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta. Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON dos parâmetros.

A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.

|Parâmetro|Tipo|Descrição|
|:---|:---|:---|
|destinationTaskListId|Cadeia de Caracteres|O [baseTaskList para](../resources/basetasklist.md) o qual [o objeto baseTask](../resources/basetask.md) deve ser movido.|



## <a name="response"></a>Resposta

Se tiver êxito, essa ação retornará `200 OK` um código de resposta e um [baseTask](../resources/basetask.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "basetask_move"
}
-->
``` http
POST /me/tasks/lists/AAMkAGVjMzJmMWZjLTgyYjgtNGIyNi1hOGQ0LWRjMjNmMGRmOWNiYQAuAAAAAAAboFsPFj7gQpLAt/tasks/AAkALgAAAAAAHYQDEapmEc2byACqAC-EWg0AkOO4xOT/move
Content-Type: application/json
Content-length: 41

{
  "destinationTaskListId": "AAMkAGVjMzJmMWZjLTgyYjgtNGIyNi1hOGQ0LWRjMjNmMGRmOWNiYQAuAAAAAAAboFsPFj7gQqFxG"
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
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.type": "#microsoft.graph.task",
    "@odata.etag": "W/\"kOO4xOT//0qFRAqk3TNe0QAAAymRCA==\"",
    "importance": "normal",
    "status": "notStarted",
    "displayName": "T1",
    "createdDateTime": "2021-11-15T13:16:53.0831814Z",
    "lastModifiedDateTime": "2021-11-15T13:17:24.9876101Z",
    "id": "AAkALgAAAAAAHYQDEapmEc2byACqAC-EWg0AkOO4xOT",
    "body": {
        "content": "",
        "contentType": "text"
    },
    "parentList": {
        "id": "AAMkAGVjMzJmMWZjLTgyYjgtNGIyNi1hOGQ0LWRjMjNmMGRmOWNiYQAuAAAAAAAboFsPFj7gQqFxG"
    }
}
```

