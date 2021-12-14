---
title: Listar baseTasks
description: Obter os recursos baseTask da propriedade de navegação tarefas de uma baseTaskList específica.
author: devindrajit
ms.localizationpriority: medium
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 1a4df47f32a92d78bdd56bf1d1a786ddde83a64b
ms.sourcegitcommit: c99d3feb3ab5cae506c1f758bc277a637adc9111
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/13/2021
ms.locfileid: "61432639"
---
# <a name="list-basetasks"></a>Listar baseTasks
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obter os [recursos baseTask](../resources/basetask.md) da propriedade de navegação tarefas de uma [baseTaskList específica.](../resources/basetasklist.md)

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)|Tasks.Read, Tasks.ReadWrite|
|Delegada (conta pessoal da Microsoft)|Tasks.Read, Tasks.ReadWrite|
|Aplicativo|Sem suporte|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/tasks/lists/{baseTaskListId}/tasks
GET /users/{userId|userPrincipalName}/tasks/lists/{baseTaskListId}/tasks
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método oferece `$expand` suporte a `$filter` `$top` [parâmetros de consulta EData](/graph/query-parameters) para personalizar a resposta.  

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos baseTask](../resources/basetask.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "list_basetask"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/tasks/lists/AQMkAGVjMzJmMWZjLTgyYjgtNGIyNi1hOGQ0LWRjMjNm/tasks
```


### <a name="response"></a>Resposta
**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.baseTask)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('43e9e4fb-be9f-4ee4-b879-59688955ed54')/tasks/lists('AQMkAGVjMzJmMWZjLTgyYjgtNGIyNi1hOGQ0LWRjMjNm')/tasks",
    "value": [
        {
            "@odata.type": "#microsoft.graph.task",
            "@odata.etag": "W/\"kOO4xOT//0qFRAqk3TNe0QAABCEtjw==\"",
            "importance": "normal",
            "status": "notStarted",
            "displayName": "Buy medicine",
            "createdDateTime": "2021-11-17T06:58:32.4882235Z",
            "lastModifiedDateTime": "2021-11-17T07:02:49.1697427Z",
            "id": "AAkALgAAAAAAHYQDEapmEc2byACqAC",
            "body": {
                "content": "",
                "contentType": "text"
            },
            "parentList": {
                "id": "AQMkAGVjMzJmMWZjLTgyYjgtNGIyNi1hOGQ0LWRjMjNm"
            }
        }
    ]
}
```

