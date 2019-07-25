---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: Lista as listas do SharePoint em um site
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 5eaa02bad7ce4997386a6b113bf7854493a67e90
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35880297"
---
# <a name="enumerate-lists-in-a-site"></a><span data-ttu-id="55bba-102">Enumerar listas em um site</span><span class="sxs-lookup"><span data-stu-id="55bba-102">Enumerate lists in a site</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="55bba-103">Obter a coleção de [listas][] de um [site][].</span><span class="sxs-lookup"><span data-stu-id="55bba-103">Get the collection of [lists][] for a [site][].</span></span>

[listas]: ../resources/list.md
[lists]: ../resources/list.md
[site]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="55bba-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="55bba-106">Permissions</span></span>

<span data-ttu-id="55bba-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="55bba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="55bba-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="55bba-109">Permission type</span></span>      | <span data-ttu-id="55bba-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="55bba-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="55bba-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="55bba-111">Delegated (work or school account)</span></span> | <span data-ttu-id="55bba-112">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="55bba-112">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="55bba-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="55bba-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="55bba-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="55bba-114">Not supported.</span></span>    |
|<span data-ttu-id="55bba-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="55bba-115">Application</span></span> | <span data-ttu-id="55bba-116">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="55bba-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="55bba-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="55bba-117">HTTP request</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists
```

## <a name="example"></a><span data-ttu-id="55bba-118">Exemplo</span><span class="sxs-lookup"><span data-stu-id="55bba-118">Example</span></span>

#### <a name="request"></a><span data-ttu-id="55bba-119">Solicitação</span><span class="sxs-lookup"><span data-stu-id="55bba-119">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="55bba-120">HTTP</span><span class="sxs-lookup"><span data-stu-id="55bba-120">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "enum-lists", "scopes": "sites.read.all service.sharepoint" } -->

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="55bba-121">C#</span><span class="sxs-lookup"><span data-stu-id="55bba-121">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/enum-lists-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="55bba-122">Javascript</span><span class="sxs-lookup"><span data-stu-id="55bba-122">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/enum-lists-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="55bba-123">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="55bba-123">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/enum-lists-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="55bba-124">Java</span><span class="sxs-lookup"><span data-stu-id="55bba-124">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/enum-lists-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="55bba-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="55bba-125">Response</span></span>

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

## <a name="remarks"></a><span data-ttu-id="55bba-126">Comentários</span><span class="sxs-lookup"><span data-stu-id="55bba-126">Remarks</span></span>

<span data-ttu-id="55bba-127">Listas com a faceta [system][] estão ocultas por padrão.</span><span class="sxs-lookup"><span data-stu-id="55bba-127">Lists with the [system][] facet are hidden by default.</span></span>
<span data-ttu-id="55bba-128">Para listá-los, inclua `system` na instrução `$select`.</span><span class="sxs-lookup"><span data-stu-id="55bba-128">To list them, include `system` in your `$select` statement.</span></span>

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
