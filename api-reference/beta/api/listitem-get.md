---
author: JeremyKelley
description: Retorna os metadados de um item em uma lista.
ms.date: 09/11/2017
title: Obter uma entrada de uma lista do SharePoint
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 94536503949c5348da8a66a04cfc18fdb25f9223
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35993078"
---
# <a name="get-an-item-in-a-list"></a><span data-ttu-id="7e9c5-103">Obter um item em uma lista</span><span class="sxs-lookup"><span data-stu-id="7e9c5-103">Get an item in a list</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7e9c5-104">Retorna os metadados de um [item][] em uma [lista][].</span><span class="sxs-lookup"><span data-stu-id="7e9c5-104">Returns the metadata for an [item][] in a [list][].</span></span>

[lista]: ../resources/list.md
[list]: ../resources/list.md
[item]: ../resources/listitem.md

## <a name="permissions"></a><span data-ttu-id="7e9c5-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="7e9c5-107">Permissions</span></span>

<span data-ttu-id="7e9c5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7e9c5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7e9c5-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7e9c5-110">Permission type</span></span>      | <span data-ttu-id="7e9c5-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7e9c5-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7e9c5-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7e9c5-112">Delegated (work or school account)</span></span> | <span data-ttu-id="7e9c5-113">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e9c5-113">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="7e9c5-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7e9c5-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7e9c5-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7e9c5-115">Not supported.</span></span>    |
|<span data-ttu-id="7e9c5-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7e9c5-116">Application</span></span> | <span data-ttu-id="7e9c5-117">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e9c5-117">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7e9c5-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7e9c5-118">HTTP request</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields(select=Column1,Column2)
```

## <a name="example"></a><span data-ttu-id="7e9c5-119">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7e9c5-119">Example</span></span>

##### <a name="request"></a><span data-ttu-id="7e9c5-120">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7e9c5-120">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="7e9c5-121">HTTP</span><span class="sxs-lookup"><span data-stu-id="7e9c5-121">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-list-item" } -->

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7e9c5-122">C#</span><span class="sxs-lookup"><span data-stu-id="7e9c5-122">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-list-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7e9c5-123">Javascript</span><span class="sxs-lookup"><span data-stu-id="7e9c5-123">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-list-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7e9c5-124">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="7e9c5-124">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-list-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="7e9c5-125">Java</span><span class="sxs-lookup"><span data-stu-id="7e9c5-125">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-list-item-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="7e9c5-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="7e9c5-126">Response</span></span>

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
