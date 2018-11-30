---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: Lista as listas do SharePoint em um site
ms.openlocfilehash: 4171947eb2a7ac6be18ba385de39c5befd762f26
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006484"
---
# <a name="enumerate-lists-in-a-site"></a><span data-ttu-id="c0c95-102">Enumerar listas em um site</span><span class="sxs-lookup"><span data-stu-id="c0c95-102">Enumerate lists in a site</span></span>

<span data-ttu-id="c0c95-103">Obter a coleção de [listas][] de um [site][].</span><span class="sxs-lookup"><span data-stu-id="c0c95-103">Get the collection of [lists][] for a [site][].</span></span>

[listas]: ../resources/list.md
[lists]: ../resources/list.md
[site]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="c0c95-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c0c95-106">Permissions</span></span>

<span data-ttu-id="c0c95-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c0c95-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0c95-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c0c95-109">Permission type</span></span>      | <span data-ttu-id="c0c95-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c0c95-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c0c95-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c0c95-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c0c95-112">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0c95-112">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="c0c95-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c0c95-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c0c95-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c0c95-114">Not supported.</span></span>    |
|<span data-ttu-id="c0c95-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c0c95-115">Application</span></span> | <span data-ttu-id="c0c95-116">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0c95-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c0c95-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c0c95-117">HTTP request</span></span>

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists
```

## <a name="example"></a><span data-ttu-id="c0c95-118">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c0c95-118">Example</span></span>

#### <a name="request"></a><span data-ttu-id="c0c95-119">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c0c95-119">Request</span></span>

<!-- { "blockType": "request", "name": "enum-lists", "scopes": "sites.read.all", "tags": "service.sharepoint" } -->

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists
```

##### <a name="response"></a><span data-ttu-id="c0c95-120">Resposta</span><span class="sxs-lookup"><span data-stu-id="c0c95-120">Response</span></span>

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

## <a name="remarks"></a><span data-ttu-id="c0c95-121">Comentários</span><span class="sxs-lookup"><span data-stu-id="c0c95-121">Remarks</span></span>

<span data-ttu-id="c0c95-122">Listas com a faceta [system][] estão ocultas por padrão.</span><span class="sxs-lookup"><span data-stu-id="c0c95-122">Lists with the [system][] facet are hidden by default.</span></span>
<span data-ttu-id="c0c95-123">Para listá-los, inclua `system` na instrução `$select`.</span><span class="sxs-lookup"><span data-stu-id="c0c95-123">To list them, include `system` in your `$select` statement.</span></span>

[sistema]: ../resources/systemfacet.md
[system]: ../resources/systemfacet.md

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Lists/Enumerate"
} -->
