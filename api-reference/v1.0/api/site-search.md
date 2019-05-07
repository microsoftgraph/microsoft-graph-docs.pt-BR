---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Procurar sites
description: Pesquisar em um locatário do SharePoint para sites que correspondam a palavras-chave fornecidas.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 5dedb77a362507b5d59a8372f64bd72d6504c980
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33603070"
---
# <a name="search-for-sites"></a><span data-ttu-id="d1cca-103">Procurar sites</span><span class="sxs-lookup"><span data-stu-id="d1cca-103">Search for sites</span></span>

<span data-ttu-id="d1cca-104">Pesquisar em um locatário do SharePoint para [sites][] que correspondam a palavras-chave fornecidas.</span><span class="sxs-lookup"><span data-stu-id="d1cca-104">Search across a SharePoint tenant for [sites][] that match keywords provided.</span></span>

[sites]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="d1cca-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d1cca-106">Permissions</span></span>

<span data-ttu-id="d1cca-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d1cca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d1cca-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d1cca-109">Permission type</span></span>                        | <span data-ttu-id="d1cca-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d1cca-110">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="d1cca-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d1cca-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d1cca-112">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1cca-112">Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="d1cca-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d1cca-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d1cca-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d1cca-114">Not supported.</span></span>
|<span data-ttu-id="d1cca-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d1cca-115">Application</span></span>                            | <span data-ttu-id="d1cca-116">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1cca-116">Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="d1cca-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d1cca-117">HTTP request</span></span>

<!-- { "blockType": "request", "name": "search-sites", "scopes": "sites.readwrite.all", "tags": "service.sharepoint" } -->

```http
GET /sites?search={query}
```

## <a name="response"></a><span data-ttu-id="d1cca-118">Resposta</span><span class="sxs-lookup"><span data-stu-id="d1cca-118">Response</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="d1cca-119">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="d1cca-119">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d1cca-120">Basic</span><span class="sxs-lookup"><span data-stu-id="d1cca-120">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/search-sites-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d1cca-121">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d1cca-121">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/search-sites-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
><span data-ttu-id="d1cca-122">**Observação:** A única propriedade que funciona para classificação é **createdDateTime**.</span><span class="sxs-lookup"><span data-stu-id="d1cca-122">**Note:** The only property that works for sorting is **createdDateTime**.</span></span> <span data-ttu-id="d1cca-123">O filtro de pesquisa é uma pesquisa de texto livre que usa várias propriedades ao recuperar os resultados da pesquisa.</span><span class="sxs-lookup"><span data-stu-id="d1cca-123">The search filter is a free text search that uses multiple properties when retrieving the search results.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Sites/Search",
  "suppressions": [
    "Error: /api-reference/v1.0/api/site-search.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/site-search.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
} -->
