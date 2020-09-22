---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Procurar sites
description: Pesquise num locatário do SharePoint por sites que correspondam a palavras-chave fornecidas.
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 0174031ed72a1c4833fcec411ebfba578aec1aa2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48038106"
---
# <a name="search-for-sites"></a><span data-ttu-id="7e130-103">Procurar sites</span><span class="sxs-lookup"><span data-stu-id="7e130-103">Search for sites</span></span>

<span data-ttu-id="7e130-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7e130-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7e130-105">Pesquisar em um locatário do SharePoint para [sites][] que correspondam a palavras-chave fornecidas.</span><span class="sxs-lookup"><span data-stu-id="7e130-105">Search across a SharePoint tenant for [sites][] that match keywords provided.</span></span>

[sites]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="7e130-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="7e130-107">Permissions</span></span>

<span data-ttu-id="7e130-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7e130-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7e130-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7e130-110">Permission type</span></span>                        | <span data-ttu-id="7e130-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7e130-111">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="7e130-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7e130-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="7e130-113">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e130-113">Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="7e130-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7e130-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7e130-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7e130-115">Not supported.</span></span>
|<span data-ttu-id="7e130-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7e130-116">Application</span></span>                            | <span data-ttu-id="7e130-117">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e130-117">Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="7e130-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7e130-118">HTTP request</span></span>


# <a name="http"></a>[<span data-ttu-id="7e130-119">HTTP</span><span class="sxs-lookup"><span data-stu-id="7e130-119">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "search-sites", "scopes": "sites.readwrite.all", "tags": "service.sharepoint" } -->

```msgraph-interactive
GET /sites?search={query}
```
# <a name="c"></a>[<span data-ttu-id="7e130-120">C#</span><span class="sxs-lookup"><span data-stu-id="7e130-120">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/search-sites-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7e130-121">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7e130-121">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/search-sites-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7e130-122">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7e130-122">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/search-sites-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7e130-123">Java</span><span class="sxs-lookup"><span data-stu-id="7e130-123">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/search-sites-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="7e130-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="7e130-124">Response</span></span>

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
><span data-ttu-id="7e130-125">**Observação:** A única propriedade que funciona para classificação é **createdDateTime**.</span><span class="sxs-lookup"><span data-stu-id="7e130-125">**Note:** The only property that works for sorting is **createdDateTime**.</span></span> <span data-ttu-id="7e130-126">O filtro de pesquisa é uma pesquisa de texto livre que usa várias propriedades ao recuperar os resultados da pesquisa.</span><span class="sxs-lookup"><span data-stu-id="7e130-126">The search filter is a free text search that uses multiple properties when retrieving the search results.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Sites/Search",
  "suppressions": [
  ]
} -->

