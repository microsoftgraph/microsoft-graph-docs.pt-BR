---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: Recuperar itens de uma lista do SharePoint
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: b5cdb31aa3f12fa6c5fee867f0a7b5ea62f16fd2
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35880182"
---
# <a name="enumerate-items-in-a-list"></a>Enumerar itens em uma lista

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obter a coleção de [itens][item] em uma [lista][].

[lista]: ../resources/list.md
[item]: ../resources/listitem.md

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Sites.Read.All, Sites.ReadWrite.All    |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | Sites.Read.All, Sites.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items?expand=fields
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items?expand=fields(select=Column1,Column2)
```

## <a name="example"></a>Exemplo

#### <a name="request"></a>Solicitação


# <a name="httptabhttp"></a>[HTTP](#tab/http)
<!-- { "blockType": "request", "name": "get-list-items" } -->

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items?expand=fields(select=Name,Color,Quantity)
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-list-items-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-list-items-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[Objetivo-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-list-items-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-list-items-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Resposta

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.listItem)", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "2",
      "fields": {
        "Name": "Gadget",
        "Color": "Red",
        "Quantity": 503
       }
    },
    {
      "id": "4",
      "fields": {
        "Name": "Widget",
        "Color": "Blue",
        "Quantity": 2357
       }
    },
    {
      "id": "7",
      "fields": {
        "Name": "Gizmo",
        "Color": "Green",
        "Quantity": 92
       }
    }
  ]
}
```

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Enumerate",
  "suppressions": [
  ]
}
-->
