---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: Obter uma entrada de uma lista do SharePoint
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 0864650701f9f6d4ee195373b5875dfe5a86b46a
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35449159"
---
# <a name="get-an-item-in-a-list"></a><span data-ttu-id="a23de-102">Obter um item em uma lista</span><span class="sxs-lookup"><span data-stu-id="a23de-102">Get an item in a list</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a23de-103">Retorna os metadados de um [item][] em uma [lista][].</span><span class="sxs-lookup"><span data-stu-id="a23de-103">Returns the metadata for an [item][] in a [list][].</span></span>

[lista]: ../resources/list.md
[list]: ../resources/list.md
[item]: ../resources/listitem.md

## <a name="permissions"></a><span data-ttu-id="a23de-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a23de-106">Permissions</span></span>

<span data-ttu-id="a23de-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a23de-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a23de-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a23de-109">Permission type</span></span>      | <span data-ttu-id="a23de-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a23de-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a23de-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a23de-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a23de-112">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a23de-112">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="a23de-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a23de-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a23de-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a23de-114">Not supported.</span></span>    |
|<span data-ttu-id="a23de-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a23de-115">Application</span></span> | <span data-ttu-id="a23de-116">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a23de-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a23de-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a23de-117">HTTP request</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields(select=Column1,Column2)
```

## <a name="example"></a><span data-ttu-id="a23de-118">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a23de-118">Example</span></span>

##### <a name="request"></a><span data-ttu-id="a23de-119">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a23de-119">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="a23de-120">HTTP</span><span class="sxs-lookup"><span data-stu-id="a23de-120">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-list-item" } -->

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a23de-121">C#</span><span class="sxs-lookup"><span data-stu-id="a23de-121">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-list-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a23de-122">Javascript</span><span class="sxs-lookup"><span data-stu-id="a23de-122">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-list-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a23de-123">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="a23de-123">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-list-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="a23de-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="a23de-124">Response</span></span>

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
