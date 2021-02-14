---
author: JeremyKelley
ms.date: 09/11/2017
title: Lista as listas do SharePoint em um site
localization_priority: Priority
ms.prod: sharepoint
description: Obter a coleção de listas de um site.
doc_type: apiPageType
ms.openlocfilehash: ffafff7ed35f8e88d32ccd5f0e6daf3f9861e1a7
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/14/2021
ms.locfileid: "50238796"
---
# <a name="enumerate-lists-in-a-site"></a><span data-ttu-id="472ef-103">Enumerar listas em um site</span><span class="sxs-lookup"><span data-stu-id="472ef-103">Enumerate lists in a site</span></span>

<span data-ttu-id="472ef-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="472ef-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="472ef-105">Obter a coleção de [listas][] de um [site][].</span><span class="sxs-lookup"><span data-stu-id="472ef-105">Get the collection of [lists][] for a [site][].</span></span>

[listas]: ../resources/list.md
[lists]: ../resources/list.md
[site]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="472ef-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="472ef-108">Permissions</span></span>

<span data-ttu-id="472ef-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="472ef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="472ef-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="472ef-111">Permission type</span></span>      | <span data-ttu-id="472ef-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="472ef-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="472ef-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="472ef-113">Delegated (work or school account)</span></span> | <span data-ttu-id="472ef-114">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="472ef-114">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="472ef-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="472ef-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="472ef-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="472ef-116">Not supported.</span></span>    |
|<span data-ttu-id="472ef-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="472ef-117">Application</span></span> | <span data-ttu-id="472ef-118">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="472ef-118">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="472ef-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="472ef-119">HTTP request</span></span>

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists
```

## <a name="example"></a><span data-ttu-id="472ef-120">Exemplo</span><span class="sxs-lookup"><span data-stu-id="472ef-120">Example</span></span>

#### <a name="request"></a><span data-ttu-id="472ef-121">Solicitação</span><span class="sxs-lookup"><span data-stu-id="472ef-121">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="472ef-122">HTTP</span><span class="sxs-lookup"><span data-stu-id="472ef-122">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "enum-lists", "scopes": "sites.read.all", "tags": "service.sharepoint" } -->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists
```
# <a name="c"></a>[<span data-ttu-id="472ef-123">C#</span><span class="sxs-lookup"><span data-stu-id="472ef-123">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/enum-lists-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="472ef-124">JavaScript</span><span class="sxs-lookup"><span data-stu-id="472ef-124">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/enum-lists-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="472ef-125">Objective-C</span><span class="sxs-lookup"><span data-stu-id="472ef-125">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/enum-lists-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="472ef-126">Java</span><span class="sxs-lookup"><span data-stu-id="472ef-126">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/enum-lists-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="472ef-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="472ef-127">Response</span></span>

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

## <a name="remarks"></a><span data-ttu-id="472ef-128">Comentários</span><span class="sxs-lookup"><span data-stu-id="472ef-128">Remarks</span></span>

<span data-ttu-id="472ef-129">Listas com a faceta [system][] estão ocultas por padrão.</span><span class="sxs-lookup"><span data-stu-id="472ef-129">Lists with the [system][] facet are hidden by default.</span></span>
<span data-ttu-id="472ef-130">Para listá-los, inclua `system` na instrução `$select`.</span><span class="sxs-lookup"><span data-stu-id="472ef-130">To list them, include `system` in your `$select` statement.</span></span>

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

