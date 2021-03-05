---
author: JeremyKelley
description: Obtém uma coleção de subsites definidos para um site.
ms.date: 09/10/2017
title: Listar os subsites de um site do SharePoint
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 4e69e016f1a83db1b4a2f23e4829ef28d3e3cff0
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50475790"
---
# <a name="enumerate-subsites"></a><span data-ttu-id="7078d-103">Enumerar subsites</span><span class="sxs-lookup"><span data-stu-id="7078d-103">Enumerate subsites</span></span>

<span data-ttu-id="7078d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7078d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7078d-105">Obtém uma coleção de subsites definidos para um [site][].</span><span class="sxs-lookup"><span data-stu-id="7078d-105">Get a collection of subsites defined for a [site][].</span></span>

[site]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="7078d-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="7078d-107">Permissions</span></span>

<span data-ttu-id="7078d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7078d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7078d-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7078d-110">Permission type</span></span>      | <span data-ttu-id="7078d-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7078d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7078d-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7078d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="7078d-113">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7078d-113">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="7078d-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7078d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7078d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7078d-115">Not supported.</span></span>    |
|<span data-ttu-id="7078d-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7078d-116">Application</span></span> | <span data-ttu-id="7078d-117">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7078d-117">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7078d-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7078d-118">HTTP request</span></span>

```http
GET /sites/{site-id}/sites
```

# <a name="http"></a>[<span data-ttu-id="7078d-119">HTTP</span><span class="sxs-lookup"><span data-stu-id="7078d-119">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "list-subsites", "scopes": "service.sharepoint sites.read.all" } -->

```msgraph-interactive
GET https://graph.microsoft.com/beta/sites/{site-id}/sites
```
# <a name="c"></a>[<span data-ttu-id="7078d-120">C#</span><span class="sxs-lookup"><span data-stu-id="7078d-120">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-subsites-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7078d-121">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7078d-121">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-subsites-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7078d-122">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7078d-122">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-subsites-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7078d-123">Java</span><span class="sxs-lookup"><span data-stu-id="7078d-123">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-subsites-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="7078d-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="7078d-124">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.site", "isCollection": true, "truncated": true } -->

```http
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


