---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: Obter uma entrada de uma lista do SharePoint
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 90095dce5b5cfdadfd37696cd9b43a7a5475b6f6
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35880227"
---
# <a name="get-an-item-in-a-list"></a><span data-ttu-id="1767b-102">Obter um item em uma lista</span><span class="sxs-lookup"><span data-stu-id="1767b-102">Get an item in a list</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1767b-103">Retorna os metadados de um [item][] em uma [lista][].</span><span class="sxs-lookup"><span data-stu-id="1767b-103">Returns the metadata for an [item][] in a [list][].</span></span>

[lista]: ../resources/list.md
[list]: ../resources/list.md
[item]: ../resources/listitem.md

## <a name="permissions"></a><span data-ttu-id="1767b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1767b-106">Permissions</span></span>

<span data-ttu-id="1767b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1767b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1767b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1767b-109">Permission type</span></span>      | <span data-ttu-id="1767b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1767b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1767b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1767b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1767b-112">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1767b-112">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="1767b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1767b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1767b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1767b-114">Not supported.</span></span>    |
|<span data-ttu-id="1767b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1767b-115">Application</span></span> | <span data-ttu-id="1767b-116">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1767b-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1767b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1767b-117">HTTP request</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields(select=Column1,Column2)
```

## <a name="example"></a><span data-ttu-id="1767b-118">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1767b-118">Example</span></span>

##### <a name="request"></a><span data-ttu-id="1767b-119">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1767b-119">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="1767b-120">HTTP</span><span class="sxs-lookup"><span data-stu-id="1767b-120">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-list-item" } -->

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1767b-121">C#</span><span class="sxs-lookup"><span data-stu-id="1767b-121">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-list-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1767b-122">Javascript</span><span class="sxs-lookup"><span data-stu-id="1767b-122">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-list-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1767b-123">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="1767b-123">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-list-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="1767b-124">Java</span><span class="sxs-lookup"><span data-stu-id="1767b-124">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-list-item-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="1767b-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="1767b-125">Response</span></span>

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
