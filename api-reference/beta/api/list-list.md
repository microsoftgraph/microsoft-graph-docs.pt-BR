---
author: JeremyKelley
description: Obter a coleção de listas de um site.
ms.date: 09/11/2017
title: Lista as listas do SharePoint em um site
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 0068c927192d22d86ad91fad1c5b0e360312587c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35993120"
---
# <a name="enumerate-lists-in-a-site"></a><span data-ttu-id="da27b-103">Enumerar listas em um site</span><span class="sxs-lookup"><span data-stu-id="da27b-103">Enumerate lists in a site</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="da27b-104">Obter a coleção de [listas][] de um [site][].</span><span class="sxs-lookup"><span data-stu-id="da27b-104">Get the collection of [lists][] for a [site][].</span></span>

[listas]: ../resources/list.md
[lists]: ../resources/list.md
[site]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="da27b-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="da27b-107">Permissions</span></span>

<span data-ttu-id="da27b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="da27b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da27b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="da27b-110">Permission type</span></span>      | <span data-ttu-id="da27b-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="da27b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="da27b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="da27b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="da27b-113">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da27b-113">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="da27b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="da27b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="da27b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="da27b-115">Not supported.</span></span>    |
|<span data-ttu-id="da27b-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="da27b-116">Application</span></span> | <span data-ttu-id="da27b-117">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da27b-117">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="da27b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="da27b-118">HTTP request</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists
```

## <a name="example"></a><span data-ttu-id="da27b-119">Exemplo</span><span class="sxs-lookup"><span data-stu-id="da27b-119">Example</span></span>

#### <a name="request"></a><span data-ttu-id="da27b-120">Solicitação</span><span class="sxs-lookup"><span data-stu-id="da27b-120">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="da27b-121">HTTP</span><span class="sxs-lookup"><span data-stu-id="da27b-121">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "enum-lists", "scopes": "sites.read.all service.sharepoint" } -->

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="da27b-122">C#</span><span class="sxs-lookup"><span data-stu-id="da27b-122">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/enum-lists-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="da27b-123">Javascript</span><span class="sxs-lookup"><span data-stu-id="da27b-123">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/enum-lists-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="da27b-124">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="da27b-124">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/enum-lists-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="da27b-125">Java</span><span class="sxs-lookup"><span data-stu-id="da27b-125">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/enum-lists-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="da27b-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="da27b-126">Response</span></span>

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

## <a name="remarks"></a><span data-ttu-id="da27b-127">Comentários</span><span class="sxs-lookup"><span data-stu-id="da27b-127">Remarks</span></span>

<span data-ttu-id="da27b-128">Listas com a faceta [system][] estão ocultas por padrão.</span><span class="sxs-lookup"><span data-stu-id="da27b-128">Lists with the [system][] facet are hidden by default.</span></span>
<span data-ttu-id="da27b-129">Para listá-los, inclua `system` na instrução `$select`.</span><span class="sxs-lookup"><span data-stu-id="da27b-129">To list them, include `system` in your `$select` statement.</span></span>

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
