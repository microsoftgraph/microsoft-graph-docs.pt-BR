---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: Lista as listas do SharePoint em um site
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: 24ec21489d0a5100eef02d8f31fb63ba8b5cad7f
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33598383"
---
# <a name="enumerate-lists-in-a-site"></a><span data-ttu-id="181af-102">Enumerar listas em um site</span><span class="sxs-lookup"><span data-stu-id="181af-102">Enumerate lists in a site</span></span>

<span data-ttu-id="181af-103">Obter a coleção de [listas][] de um [site][].</span><span class="sxs-lookup"><span data-stu-id="181af-103">Get the collection of [lists][] for a [site][].</span></span>

[listas]: ../resources/list.md
[lists]: ../resources/list.md
[site]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="181af-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="181af-106">Permissions</span></span>

<span data-ttu-id="181af-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="181af-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="181af-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="181af-109">Permission type</span></span>      | <span data-ttu-id="181af-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="181af-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="181af-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="181af-111">Delegated (work or school account)</span></span> | <span data-ttu-id="181af-112">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="181af-112">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="181af-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="181af-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="181af-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="181af-114">Not supported.</span></span>    |
|<span data-ttu-id="181af-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="181af-115">Application</span></span> | <span data-ttu-id="181af-116">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="181af-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="181af-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="181af-117">HTTP request</span></span>

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists
```

## <a name="example"></a><span data-ttu-id="181af-118">Exemplo</span><span class="sxs-lookup"><span data-stu-id="181af-118">Example</span></span>

#### <a name="request"></a><span data-ttu-id="181af-119">Solicitação</span><span class="sxs-lookup"><span data-stu-id="181af-119">Request</span></span>

<!-- { "blockType": "request", "name": "enum-lists", "scopes": "sites.read.all", "tags": "service.sharepoint" } -->

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists
```

##### <a name="response"></a><span data-ttu-id="181af-120">Resposta</span><span class="sxs-lookup"><span data-stu-id="181af-120">Response</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="181af-121">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="181af-121">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="181af-122">Basic</span><span class="sxs-lookup"><span data-stu-id="181af-122">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/enum-lists-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="181af-123">JavaScript</span><span class="sxs-lookup"><span data-stu-id="181af-123">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/enum-lists-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="remarks"></a><span data-ttu-id="181af-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="181af-124">Remarks</span></span>

<span data-ttu-id="181af-125">Listas com a faceta [system][] estão ocultas por padrão.</span><span class="sxs-lookup"><span data-stu-id="181af-125">Lists with the [system][] facet are hidden by default.</span></span>
<span data-ttu-id="181af-126">Para listá-los, inclua `system` na instrução `$select`.</span><span class="sxs-lookup"><span data-stu-id="181af-126">To list them, include `system` in your `$select` statement.</span></span>

[system]: ../resources/systemfacet.md

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Lists/Enumerate",
  "suppressions": [
    "Error: /api-reference/v1.0/api/list-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/list-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
} -->
