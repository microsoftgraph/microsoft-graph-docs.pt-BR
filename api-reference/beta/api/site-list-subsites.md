---
author: JeremyKelley
description: Obtém uma coleção de subsites definidos para um site.
ms.date: 09/10/2017
title: Listar os subsites de um site do SharePoint
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 9c574c7d3235947407aca02b8a07ced64620aff4
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36410007"
---
# <a name="enumerate-subsites"></a><span data-ttu-id="d741b-103">Enumerar subsites</span><span class="sxs-lookup"><span data-stu-id="d741b-103">Enumerate subsites</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d741b-104">Obtém uma coleção de subsites definidos para um [site][].</span><span class="sxs-lookup"><span data-stu-id="d741b-104">Get a collection of subsites defined for a [site][].</span></span>

[site]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="d741b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d741b-106">Permissions</span></span>

<span data-ttu-id="d741b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d741b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d741b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d741b-109">Permission type</span></span>      | <span data-ttu-id="d741b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d741b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d741b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d741b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d741b-112">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d741b-112">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="d741b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d741b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d741b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d741b-114">Not supported.</span></span>    |
|<span data-ttu-id="d741b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d741b-115">Application</span></span> | <span data-ttu-id="d741b-116">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d741b-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d741b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d741b-117">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="d741b-118">HTTP</span><span class="sxs-lookup"><span data-stu-id="d741b-118">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "list-subsites", "scopes": "service.sharepoint sites.read.all" } -->

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/sites
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d741b-119">C#</span><span class="sxs-lookup"><span data-stu-id="d741b-119">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-subsites-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d741b-120">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d741b-120">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-subsites-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d741b-121">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="d741b-121">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-subsites-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="d741b-122">Resposta</span><span class="sxs-lookup"><span data-stu-id="d741b-122">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.site", "isCollection": true, "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "contoso.sharepoint.com,da60e844-ba1d-49bc-b4d4-d5e36bae9019,712a596e-90a1-49e3-9b48-bfa80bee8740",
      "name": "Team A Subsite",
      "description": "",
      "createdDateTime": "2016-10-18T03:05:59Z",
      "lastModifiedDateTime": "2016-10-18T10:40:59Z",
      "webUrl": "https://contoso.sharepoint.com/sites/site/subsiteA"
    },
    {
      "id": "contoso.sharepoint.com,da60e844-ba1d-49bc-b4d4-d5e36bae9019,0271110f-634f-4300-a841-3a8a2e851851",
      "name": "Team B Subsite",
      "description": "",
      "createdDateTime": "2016-10-18T03:05:59Z",
      "lastModifiedDateTime": "2016-10-18T10:40:59Z",
      "webUrl": "https://contoso.sharepoint.com/sites/site/subsiteB"
    }
  ]
}
```

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Sites/List subsites",
  "suppressions": [
  ]
}
-->
