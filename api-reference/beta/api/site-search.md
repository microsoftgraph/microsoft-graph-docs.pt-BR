---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Localizar sites do SharePoint por palavra-chave
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 1cf88b825250ff602a28919a35dfff4a71edb1c8
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35453590"
---
# <a name="search-for-sites"></a><span data-ttu-id="3096c-102">Procurar sites</span><span class="sxs-lookup"><span data-stu-id="3096c-102">Search for sites</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3096c-103">Pesquisar em um locatário do SharePoint para [sites][] que correspondam a palavras-chave fornecidas.</span><span class="sxs-lookup"><span data-stu-id="3096c-103">Search across a SharePoint tenant for [sites][] that match keywords provided.</span></span>

[sites]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="3096c-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="3096c-105">Permissions</span></span>

<span data-ttu-id="3096c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3096c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3096c-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3096c-108">Permission type</span></span>                        | <span data-ttu-id="3096c-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3096c-109">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="3096c-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3096c-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="3096c-111">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3096c-111">Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="3096c-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3096c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3096c-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3096c-113">Not supported.</span></span>
|<span data-ttu-id="3096c-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3096c-114">Application</span></span>                            | <span data-ttu-id="3096c-115">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3096c-115">Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="3096c-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3096c-116">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="3096c-117">HTTP</span><span class="sxs-lookup"><span data-stu-id="3096c-117">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "search-sites", "scopes": "service.sharepoint sites.readwrite.all" } -->

```http
GET https://graph.microsoft.com/beta/sites?search={query}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3096c-118">C#</span><span class="sxs-lookup"><span data-stu-id="3096c-118">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/search-sites-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3096c-119">Javascript</span><span class="sxs-lookup"><span data-stu-id="3096c-119">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/search-sites-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3096c-120">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="3096c-120">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/search-sites-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="3096c-121">Resposta</span><span class="sxs-lookup"><span data-stu-id="3096c-121">Response</span></span>

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
><span data-ttu-id="3096c-122">**Observação:** A única propriedade que funciona para classificação é **createdDateTime**.</span><span class="sxs-lookup"><span data-stu-id="3096c-122">**Note:** The only property that works for sorting is **createdDateTime**.</span></span> <span data-ttu-id="3096c-123">O filtro de pesquisa é uma pesquisa de texto livre que usa várias propriedades ao recuperar os resultados da pesquisa.</span><span class="sxs-lookup"><span data-stu-id="3096c-123">The search filter is a free text search that uses multiple properties when retrieving the search results.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Sites/Search",
  "suppressions": [
  ]
}
-->
