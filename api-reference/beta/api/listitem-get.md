---
author: JeremyKelley
description: Retorna os metadados de um item em uma lista.
ms.date: 09/11/2017
title: Obter uma entrada de uma lista do SharePoint
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: b86348b7c1648a7246a9414a2f8d96e694692fd2
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36726162"
---
# <a name="get-an-item-in-a-list"></a><span data-ttu-id="27155-103">Obter um item em uma lista</span><span class="sxs-lookup"><span data-stu-id="27155-103">Get an item in a list</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="27155-104">Retorna os metadados de um [item][] em uma [lista][].</span><span class="sxs-lookup"><span data-stu-id="27155-104">Returns the metadata for an [item][] in a [list][].</span></span>

[lista]: ../resources/list.md
[list]: ../resources/list.md
[item]: ../resources/listitem.md

## <a name="permissions"></a><span data-ttu-id="27155-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="27155-107">Permissions</span></span>

<span data-ttu-id="27155-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="27155-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="27155-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="27155-110">Permission type</span></span>      | <span data-ttu-id="27155-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="27155-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="27155-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="27155-112">Delegated (work or school account)</span></span> | <span data-ttu-id="27155-113">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27155-113">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="27155-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="27155-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="27155-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="27155-115">Not supported.</span></span>    |
|<span data-ttu-id="27155-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="27155-116">Application</span></span> | <span data-ttu-id="27155-117">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27155-117">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="27155-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="27155-118">HTTP request</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields(select=Column1,Column2)
```

## <a name="example"></a><span data-ttu-id="27155-119">Exemplo</span><span class="sxs-lookup"><span data-stu-id="27155-119">Example</span></span>

##### <a name="request"></a><span data-ttu-id="27155-120">Solicitação</span><span class="sxs-lookup"><span data-stu-id="27155-120">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="27155-121">HTTP</span><span class="sxs-lookup"><span data-stu-id="27155-121">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-list-item" } -->

```msgraph-interactive
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="27155-122">C#</span><span class="sxs-lookup"><span data-stu-id="27155-122">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-list-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="27155-123">JavaScript</span><span class="sxs-lookup"><span data-stu-id="27155-123">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-list-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="27155-124">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="27155-124">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-list-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="27155-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="27155-125">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.listItem", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "d14922d8-43e6-4c8a-b029-e35c5b4e0d63",
  "listItemId": 2,
  "fields": {
    "Name": "Widget",
    "Color": "Blue",
    "Quantity": 2357
    }
}
```

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Get metadata",
  "suppressions": [
  ]
}
-->
