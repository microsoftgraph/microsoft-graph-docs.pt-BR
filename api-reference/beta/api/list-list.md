---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: Lista as listas do SharePoint em um site
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: f7f6863f87814b56ea85b05ac1d96537828cb135
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33333460"
---
# <a name="enumerate-lists-in-a-site"></a><span data-ttu-id="2eb17-102">Enumerar listas em um site</span><span class="sxs-lookup"><span data-stu-id="2eb17-102">Enumerate lists in a site</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2eb17-103">Obter a coleção de [listas][] de um [site][].</span><span class="sxs-lookup"><span data-stu-id="2eb17-103">Get the collection of [lists][] for a [site][].</span></span>

[listas]: ../resources/list.md
[lists]: ../resources/list.md
[site]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="2eb17-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="2eb17-106">Permissions</span></span>

<span data-ttu-id="2eb17-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2eb17-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2eb17-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2eb17-109">Permission type</span></span>      | <span data-ttu-id="2eb17-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2eb17-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2eb17-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2eb17-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2eb17-112">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2eb17-112">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="2eb17-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2eb17-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2eb17-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2eb17-114">Not supported.</span></span>    |
|<span data-ttu-id="2eb17-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2eb17-115">Application</span></span> | <span data-ttu-id="2eb17-116">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2eb17-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2eb17-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2eb17-117">HTTP request</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists
```

## <a name="example"></a><span data-ttu-id="2eb17-118">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2eb17-118">Example</span></span>

#### <a name="request"></a><span data-ttu-id="2eb17-119">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2eb17-119">Request</span></span>

<!-- { "blockType": "request", "name": "enum-lists", "scopes": "sites.read.all service.sharepoint" } -->

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists
```

##### <a name="response"></a><span data-ttu-id="2eb17-120">Resposta</span><span class="sxs-lookup"><span data-stu-id="2eb17-120">Response</span></span>

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

## <a name="remarks"></a><span data-ttu-id="2eb17-121">Comentários</span><span class="sxs-lookup"><span data-stu-id="2eb17-121">Remarks</span></span>

<span data-ttu-id="2eb17-122">Listas com a faceta [system][] estão ocultas por padrão.</span><span class="sxs-lookup"><span data-stu-id="2eb17-122">Lists with the [system][] facet are hidden by default.</span></span>
<span data-ttu-id="2eb17-123">Para listá-los, inclua `system` na instrução `$select`.</span><span class="sxs-lookup"><span data-stu-id="2eb17-123">To list them, include `system` in your `$select` statement.</span></span>

[system]: ../resources/systemfacet.md

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Lists/Enumerate",
  "suppressions": []
}
-->
