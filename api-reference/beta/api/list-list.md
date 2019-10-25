---
author: JeremyKelley
description: Obter a coleção de listas de um site.
ms.date: 09/11/2017
title: Lista as listas do SharePoint em um site
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 0e365b1ee5a1f9bed585f2de557f24279c044b86
ms.sourcegitcommit: bbef506636bce5b72351ee3834123771c301b1b1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/25/2019
ms.locfileid: "37726327"
---
# <a name="enumerate-lists-in-a-site"></a><span data-ttu-id="2e889-103">Enumerar listas em um site</span><span class="sxs-lookup"><span data-stu-id="2e889-103">Enumerate lists in a site</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2e889-104">Obter a coleção de [listas][] de um [site][].</span><span class="sxs-lookup"><span data-stu-id="2e889-104">Get the collection of [lists][] for a [site][].</span></span>

[listas]: ../resources/list.md
[lists]: ../resources/list.md
[site]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="2e889-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="2e889-107">Permissions</span></span>

<span data-ttu-id="2e889-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2e889-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2e889-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2e889-110">Permission type</span></span>      | <span data-ttu-id="2e889-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2e889-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2e889-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2e889-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2e889-113">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e889-113">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="2e889-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2e889-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2e889-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2e889-115">Not supported.</span></span>    |
|<span data-ttu-id="2e889-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2e889-116">Application</span></span> | <span data-ttu-id="2e889-117">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e889-117">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2e889-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2e889-118">HTTP request</span></span>

```http
GET /sites/{site-id}/lists
```

## <a name="example"></a><span data-ttu-id="2e889-119">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2e889-119">Example</span></span>

#### <a name="request"></a><span data-ttu-id="2e889-120">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2e889-120">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="2e889-121">HTTP</span><span class="sxs-lookup"><span data-stu-id="2e889-121">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "enum-lists", "scopes": "sites.read.all service.sharepoint" } -->

```msgraph-interactive
GET https://graph.microsoft.com/beta/sites/{site-id}/lists
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2e889-122">C#</span><span class="sxs-lookup"><span data-stu-id="2e889-122">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/enum-lists-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2e889-123">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2e889-123">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/enum-lists-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2e889-124">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2e889-124">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/enum-lists-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="2e889-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="2e889-125">Response</span></span>

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

## <a name="remarks"></a><span data-ttu-id="2e889-126">Comentários</span><span class="sxs-lookup"><span data-stu-id="2e889-126">Remarks</span></span>

<span data-ttu-id="2e889-127">Listas com a faceta [system][] estão ocultas por padrão.</span><span class="sxs-lookup"><span data-stu-id="2e889-127">Lists with the [system][] facet are hidden by default.</span></span>
<span data-ttu-id="2e889-128">Para listá-los, inclua `system` na instrução `$select`.</span><span class="sxs-lookup"><span data-stu-id="2e889-128">To list them, include `system` in your `$select` statement.</span></span>

[system]: ../resources/systemfacet.md

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Lists/Enumerate",
  "suppressions": [
  ]
}
-->
