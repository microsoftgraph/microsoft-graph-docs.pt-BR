---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Procurar sites
description: Pesquisar em um locatário do SharePoint para sites que correspondam a palavras-chave fornecidas.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 2b1c598ed6c635487de2b2f35c0dc606f1e69b18
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35458597"
---
# <a name="search-for-sites"></a><span data-ttu-id="00294-103">Procurar sites</span><span class="sxs-lookup"><span data-stu-id="00294-103">Search for sites</span></span>

<span data-ttu-id="00294-104">Pesquisar em um locatário do SharePoint para [sites][] que correspondam a palavras-chave fornecidas.</span><span class="sxs-lookup"><span data-stu-id="00294-104">Search across a SharePoint tenant for [sites][] that match keywords provided.</span></span>

[sites]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="00294-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="00294-106">Permissions</span></span>

<span data-ttu-id="00294-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="00294-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="00294-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="00294-109">Permission type</span></span>                        | <span data-ttu-id="00294-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="00294-110">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="00294-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="00294-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="00294-112">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00294-112">Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="00294-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="00294-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="00294-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="00294-114">Not supported.</span></span>
|<span data-ttu-id="00294-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="00294-115">Application</span></span>                            | <span data-ttu-id="00294-116">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00294-116">Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="00294-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="00294-117">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="00294-118">HTTP</span><span class="sxs-lookup"><span data-stu-id="00294-118">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "search-sites", "scopes": "sites.readwrite.all", "tags": "service.sharepoint" } -->

```http
GET /sites?search={query}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="00294-119">C#</span><span class="sxs-lookup"><span data-stu-id="00294-119">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/search-sites-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="00294-120">Javascript</span><span class="sxs-lookup"><span data-stu-id="00294-120">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/search-sites-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="00294-121">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="00294-121">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/search-sites-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="00294-122">Resposta</span><span class="sxs-lookup"><span data-stu-id="00294-122">Response</span></span>

<!-- { "blockType": "response", "@type": "Collection(microsoft.graph.site)", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "contoso.sharepoint.com,da60e844-ba1d-49bc-b4d4-d5e36bae9019,712a596e-90a1-49e3-9b48-bfa80bee8740",
      "name": "Team A Site",
      "description": "",
      "createdDateTime": "2016-10-18T03:05:59Z",
      "lastModifiedDateTime": "2016-10-18T10:40:59Z",
      "webUrl": "https://contoso.sharepoint.com/sites/siteA"
    },
    {
      "id": "contoso.sharepoint.com,da60e844-ba1d-49bc-b4d4-d5e36bae9019,0271110f-634f-4300-a841-3a8a2e851851",
      "name": "Team B Site",
      "description": "",
      "createdDateTime": "2016-10-18T03:05:59Z",
      "lastModifiedDateTime": "2016-10-18T10:40:59Z",
      "webUrl": "https://contoso.sharepoint.com/sites/siteB"
    }
  ]
}
```
><span data-ttu-id="00294-123">**Observação:** A única propriedade que funciona para classificação é **createdDateTime**.</span><span class="sxs-lookup"><span data-stu-id="00294-123">**Note:** The only property that works for sorting is **createdDateTime**.</span></span> <span data-ttu-id="00294-124">O filtro de pesquisa é uma pesquisa de texto livre que usa várias propriedades ao recuperar os resultados da pesquisa.</span><span class="sxs-lookup"><span data-stu-id="00294-124">The search filter is a free text search that uses multiple properties when retrieving the search results.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Sites/Search",
  "suppressions": [
  ]
} -->
