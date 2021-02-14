---
author: JeremyKelley
ms.date: 09/10/2017
title: Listar os subsites de um site do SharePoint
localization_priority: Priority
ms.prod: sharepoint
description: Obtém uma coleção de subsites definidos para um site.
doc_type: apiPageType
ms.openlocfilehash: 8032f070f54ac8945444d70fe7fc189de7ddf983
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/14/2021
ms.locfileid: "50238488"
---
# <a name="enumerate-subsites"></a><span data-ttu-id="06ef7-103">Enumerar subsites</span><span class="sxs-lookup"><span data-stu-id="06ef7-103">Enumerate subsites</span></span>

<span data-ttu-id="06ef7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="06ef7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="06ef7-105">Obtém uma coleção de subsites definidos para um [site][].</span><span class="sxs-lookup"><span data-stu-id="06ef7-105">Get a collection of subsites defined for a [site][].</span></span>

[site]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="06ef7-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="06ef7-107">Permissions</span></span>

<span data-ttu-id="06ef7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="06ef7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="06ef7-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="06ef7-110">Permission type</span></span>      | <span data-ttu-id="06ef7-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="06ef7-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="06ef7-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="06ef7-112">Delegated (work or school account)</span></span> | <span data-ttu-id="06ef7-113">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06ef7-113">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="06ef7-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="06ef7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="06ef7-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="06ef7-115">Not supported.</span></span>    |
|<span data-ttu-id="06ef7-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="06ef7-116">Application</span></span> | <span data-ttu-id="06ef7-117">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06ef7-117">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="06ef7-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="06ef7-118">HTTP request</span></span>


# <a name="http"></a>[<span data-ttu-id="06ef7-119">HTTP</span><span class="sxs-lookup"><span data-stu-id="06ef7-119">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "list-subsites", "scopes": "sites.read.all", "tags": "service.sharepoint" } -->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/sites/{site-id}/sites
```
# <a name="c"></a>[<span data-ttu-id="06ef7-120">C#</span><span class="sxs-lookup"><span data-stu-id="06ef7-120">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-subsites-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="06ef7-121">JavaScript</span><span class="sxs-lookup"><span data-stu-id="06ef7-121">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-subsites-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="06ef7-122">Objective-C</span><span class="sxs-lookup"><span data-stu-id="06ef7-122">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-subsites-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="06ef7-123">Java</span><span class="sxs-lookup"><span data-stu-id="06ef7-123">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-subsites-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="06ef7-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="06ef7-124">Response</span></span>

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

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Sites/List subsites",
  "suppressions": [
  ]
} -->

