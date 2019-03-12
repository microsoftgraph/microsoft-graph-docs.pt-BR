---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: Lista as listas do SharePoint em um site
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: 4cafc4ea32b1dadd686f257946470ba41e32c48b
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2019
ms.locfileid: "30482095"
---
# <a name="enumerate-lists-in-a-site"></a><span data-ttu-id="897fb-102">Enumerar listas em um site</span><span class="sxs-lookup"><span data-stu-id="897fb-102">Enumerate lists in a site</span></span>

<span data-ttu-id="897fb-103">Obter a coleção de [listas][] de um [site][].</span><span class="sxs-lookup"><span data-stu-id="897fb-103">Get the collection of [lists][] for a [site][].</span></span>

[listas]: ../resources/list.md
[lists]: ../resources/list.md
[site]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="897fb-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="897fb-106">Permissions</span></span>

<span data-ttu-id="897fb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="897fb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="897fb-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="897fb-109">Permission type</span></span>      | <span data-ttu-id="897fb-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="897fb-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="897fb-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="897fb-111">Delegated (work or school account)</span></span> | <span data-ttu-id="897fb-112">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="897fb-112">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="897fb-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="897fb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="897fb-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="897fb-114">Not supported.</span></span>    |
|<span data-ttu-id="897fb-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="897fb-115">Application</span></span> | <span data-ttu-id="897fb-116">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="897fb-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="897fb-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="897fb-117">HTTP request</span></span>

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists
```

## <a name="example"></a><span data-ttu-id="897fb-118">Exemplo</span><span class="sxs-lookup"><span data-stu-id="897fb-118">Example</span></span>

#### <a name="request"></a><span data-ttu-id="897fb-119">Solicitação</span><span class="sxs-lookup"><span data-stu-id="897fb-119">Request</span></span>

<!-- { "blockType": "request", "name": "enum-lists", "scopes": "sites.read.all", "tags": "service.sharepoint" } -->

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists
```

##### <a name="response"></a><span data-ttu-id="897fb-120">Resposta</span><span class="sxs-lookup"><span data-stu-id="897fb-120">Response</span></span>

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

## <a name="remarks"></a><span data-ttu-id="897fb-121">Comentários</span><span class="sxs-lookup"><span data-stu-id="897fb-121">Remarks</span></span>

<span data-ttu-id="897fb-122">Listas com a faceta [system][] estão ocultas por padrão.</span><span class="sxs-lookup"><span data-stu-id="897fb-122">Lists with the [system][] facet are hidden by default.</span></span>
<span data-ttu-id="897fb-123">Para listá-los, inclua `system` na instrução `$select`.</span><span class="sxs-lookup"><span data-stu-id="897fb-123">To list them, include `system` in your `$select` statement.</span></span>

[system]: ../resources/systemfacet.md

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Lists/Enumerate"
} -->
