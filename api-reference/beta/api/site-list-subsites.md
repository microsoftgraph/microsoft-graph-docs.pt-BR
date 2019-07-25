---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Listar os subsites de um site do SharePoint
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 3bbf709bfe031da433f054f6a51b2b8068b1e3af
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35869655"
---
# <a name="enumerate-subsites"></a><span data-ttu-id="62c6e-102">Enumerar subsites</span><span class="sxs-lookup"><span data-stu-id="62c6e-102">Enumerate subsites</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="62c6e-103">Obtém uma coleção de subsites definidos para um [site][].</span><span class="sxs-lookup"><span data-stu-id="62c6e-103">Get a collection of subsites defined for a [site][].</span></span>

[site]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="62c6e-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="62c6e-105">Permissions</span></span>

<span data-ttu-id="62c6e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="62c6e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="62c6e-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="62c6e-108">Permission type</span></span>      | <span data-ttu-id="62c6e-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="62c6e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="62c6e-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="62c6e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="62c6e-111">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="62c6e-111">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="62c6e-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="62c6e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="62c6e-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="62c6e-113">Not supported.</span></span>    |
|<span data-ttu-id="62c6e-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="62c6e-114">Application</span></span> | <span data-ttu-id="62c6e-115">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="62c6e-115">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="62c6e-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="62c6e-116">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="62c6e-117">HTTP</span><span class="sxs-lookup"><span data-stu-id="62c6e-117">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "list-subsites", "scopes": "service.sharepoint sites.read.all" } -->

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/sites
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="62c6e-118">C#</span><span class="sxs-lookup"><span data-stu-id="62c6e-118">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-subsites-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="62c6e-119">Javascript</span><span class="sxs-lookup"><span data-stu-id="62c6e-119">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-subsites-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="62c6e-120">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="62c6e-120">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-subsites-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="62c6e-121">Java</span><span class="sxs-lookup"><span data-stu-id="62c6e-121">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-subsites-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="62c6e-122">Resposta</span><span class="sxs-lookup"><span data-stu-id="62c6e-122">Response</span></span>

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
