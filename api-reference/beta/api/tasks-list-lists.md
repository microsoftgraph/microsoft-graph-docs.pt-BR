---
title: List lists
description: Obter uma lista dos objetos baseTaskList de um usuário e suas propriedades.
author: devindrajit
ms.localizationpriority: medium
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 94ea95d30e3dddfe6cc4f050d05348de2c9498ee
ms.sourcegitcommit: c99d3feb3ab5cae506c1f758bc277a637adc9111
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/13/2021
ms.locfileid: "61432637"
---
# <a name="list-lists"></a>List lists
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obter uma lista dos [objetos baseTaskList](../resources/basetasklist.md) de um usuário e suas propriedades.

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
GET /me/tasks/lists
GET /users/{userId|userPrincipalName}/tasks/lists
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

Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos baseTaskList](../resources/basetasklist.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "list_basetasklist"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/tasks/lists
```


### <a name="response"></a>Resposta
**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.baseTaskList)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "value": [
        {
            "@odata.type": "#microsoft.graph.wellKnownTaskList",
            "@odata.etag": "W/\"kOO4xOT//0qFRAqk3TNe0QAAAAAAkw==\"",
            "wellKnownListName": "defaultList",
            "displayName": "Tasks",
            "id": "AQMkAGVjMzJmMWZjLTgyYjgtNGIyNi1hOGQ0LWRjMj"
        }
    ]
}
```

