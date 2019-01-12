---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Obter uma versão anterior de um item de lista - API do SharePoint
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 4068ebd1e8a245f2418954ce04bad1f78530acd0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27983874"
---
# <a name="get-a-listitemversion-resource-preview"></a>Obter um recurso ListItemVersion (prévia)

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Recuperar os metadados de uma versão específica de um [ListItem](../resources/listitem.md).

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|            Tipo de permissão             | Permissões (da com menos para a com mais privilégios) |
| :------------------------------------- | :------------------------------------------ |
| Delegado (conta corporativa ou de estudante)     | Sites.Read.All, Sites.ReadWrite.All         |
| Delegada (conta pessoal da Microsoft) | n/d                                         |
| Aplicativo                            | Sites.Read.All, Sites.ReadWrite.All         |


## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored"} -->

```http
GET /sites/{site-id}/items/{item-id}/versions/{version-id}
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}
```


## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [ListItemVersion](../resources/listitemversion.md) no corpo da resposta.


## <a name="example"></a>Exemplo

Este exemplo recupera uma versão de um item de lista e expande o conjunto de campos para solicitar os valores dos campos no listItem.

### <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "request", "name": "get-single-version-listItem", "scopes": "files.read" } -->

```http
GET /sites/{site-id}/items/{item-id}/versions/{version-id}?expand=fields
```

### <a name="response"></a>Resposta

Isso retornará uma coleção de versões:

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.listItemVersion", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "id": "1.0",
    "lastModifiedBy": {
    "user": {
        "id": "CE251278-EF9E-4FE5-833C-1D89EEAE68E0",
        "displayName": "Ryan Gregg"
    }
    },
    "lastModifiedDateTime": "2017-09-14T12:34:53.912Z",
    "fields": {  }
}
```

<!-- {
  "type": "#page.annotation",
  "description": "List, review, and download previous versions of a driveItem",
  "keywords": "version, version history, versions",
  "section": "documentation",
  "tocPath": "Items/Version history"
} -->
