---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: Lista as listas do SharePoint em um site
localization_priority: Priority
ms.prod: sharepoint
description: Obter a coleção de listas de um site.
doc_type: apiPageType
ms.openlocfilehash: d13ae20343ab434d9f26d7d63fc445fa55306af2
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36730285"
---
# <a name="enumerate-lists-in-a-site"></a><span data-ttu-id="b2cf0-103">Enumerar listas em um site</span><span class="sxs-lookup"><span data-stu-id="b2cf0-103">Enumerate lists in a site</span></span>

<span data-ttu-id="b2cf0-104">Obter a coleção de [listas][] de um [site][].</span><span class="sxs-lookup"><span data-stu-id="b2cf0-104">Get the collection of [lists][] for a [site][].</span></span>

[listas]: ../resources/list.md
[lists]: ../resources/list.md
[site]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="b2cf0-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="b2cf0-107">Permissions</span></span>

<span data-ttu-id="b2cf0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b2cf0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b2cf0-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b2cf0-110">Permission type</span></span>      | <span data-ttu-id="b2cf0-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b2cf0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b2cf0-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b2cf0-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b2cf0-113">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2cf0-113">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="b2cf0-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b2cf0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b2cf0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b2cf0-115">Not supported.</span></span>    |
|<span data-ttu-id="b2cf0-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b2cf0-116">Application</span></span> | <span data-ttu-id="b2cf0-117">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2cf0-117">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b2cf0-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b2cf0-118">HTTP request</span></span>

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists
```

## <a name="example"></a><span data-ttu-id="b2cf0-119">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b2cf0-119">Example</span></span>

#### <a name="request"></a><span data-ttu-id="b2cf0-120">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b2cf0-120">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="b2cf0-121">HTTP</span><span class="sxs-lookup"><span data-stu-id="b2cf0-121">--Http</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "enum-lists", "scopes": "sites.read.all", "tags": "service.sharepoint" } -->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b2cf0-122">C#</span><span class="sxs-lookup"><span data-stu-id="b2cf0-122">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/enum-lists-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b2cf0-123">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b2cf0-123">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/enum-lists-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b2cf0-124">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b2cf0-124">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/enum-lists-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b2cf0-125">Java</span><span class="sxs-lookup"><span data-stu-id="b2cf0-125">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/enum-lists-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b2cf0-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="b2cf0-126">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.list", "isCollection": true, "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "b57af081-936c-4803-a120-d94887b03864",
      "name": "Documents",
      "createdDateTime": "2016-08-30T08:32:00Z",
      "lastModifiedDateTime": "2016-08-30T08:32:00Z",
      "list": {
        "hidden": false,
        "template": "documentLibrary"
       }
    },
    {
      "id": "1234-112-112-4",
      "name": "MicroFeed",
      "createdDateTime": "2016-08-30T08:32:00Z",
      "lastModifiedDateTime": "2016-08-30T08:32:00Z",
      "list": {
        "hidden": false,
        "template": "genericList"
       }
    }
  ]
}
```

## <a name="remarks"></a><span data-ttu-id="b2cf0-127">Comentários</span><span class="sxs-lookup"><span data-stu-id="b2cf0-127">Remarks</span></span>

<span data-ttu-id="b2cf0-128">Listas com a faceta [system][] estão ocultas por padrão.</span><span class="sxs-lookup"><span data-stu-id="b2cf0-128">Lists with the [system][] facet are hidden by default.</span></span>
<span data-ttu-id="b2cf0-129">Para listá-los, inclua `system` na instrução `$select`.</span><span class="sxs-lookup"><span data-stu-id="b2cf0-129">To list them, include `system` in your `$select` statement.</span></span>

[system]: ../resources/systemfacet.md

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Lists/Enumerate",
  "suppressions": [
  ]
} -->
