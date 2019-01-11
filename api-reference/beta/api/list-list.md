---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: Lista as listas do SharePoint em um site
localization_priority: Normal
ms.openlocfilehash: fbba85c9bb1807955670d19398e2175c3805f64f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27851694"
---
# <a name="enumerate-lists-in-a-site"></a><span data-ttu-id="3030c-102">Enumerar listas em um site</span><span class="sxs-lookup"><span data-stu-id="3030c-102">Enumerate lists in a site</span></span>

> <span data-ttu-id="3030c-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="3030c-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3030c-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3030c-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3030c-105">Obter a coleção de [listas][] de um [site][].</span><span class="sxs-lookup"><span data-stu-id="3030c-105">Get the collection of [lists][] for a [site][].</span></span>

[listas]: ../resources/list.md
[lists]: ../resources/list.md
[site]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="3030c-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="3030c-108">Permissions</span></span>

<span data-ttu-id="3030c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3030c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3030c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3030c-111">Permission type</span></span>      | <span data-ttu-id="3030c-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3030c-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3030c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3030c-113">Delegated (work or school account)</span></span> | <span data-ttu-id="3030c-114">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3030c-114">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="3030c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3030c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3030c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3030c-116">Not supported.</span></span>    |
|<span data-ttu-id="3030c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3030c-117">Application</span></span> | <span data-ttu-id="3030c-118">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3030c-118">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3030c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3030c-119">HTTP request</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists
```

## <a name="example"></a><span data-ttu-id="3030c-120">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3030c-120">Example</span></span>

#### <a name="request"></a><span data-ttu-id="3030c-121">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3030c-121">Request</span></span>

<!-- { "blockType": "request", "name": "enum-lists", "scopes": "sites.read.all service.sharepoint" } -->

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists
```

##### <a name="response"></a><span data-ttu-id="3030c-122">Resposta</span><span class="sxs-lookup"><span data-stu-id="3030c-122">Response</span></span>

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

## <a name="remarks"></a><span data-ttu-id="3030c-123">Comentários</span><span class="sxs-lookup"><span data-stu-id="3030c-123">Remarks</span></span>

<span data-ttu-id="3030c-124">Listas com a faceta [system][] estão ocultas por padrão.</span><span class="sxs-lookup"><span data-stu-id="3030c-124">Lists with the [system][] facet are hidden by default.</span></span>
<span data-ttu-id="3030c-125">Para listá-los, inclua `system` na instrução `$select`.</span><span class="sxs-lookup"><span data-stu-id="3030c-125">To list them, include `system` in your `$select` statement.</span></span>

[sistema]: ../resources/systemfacet.md
[system]: ../resources/systemfacet.md

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Lists/Enumerate"
} -->
