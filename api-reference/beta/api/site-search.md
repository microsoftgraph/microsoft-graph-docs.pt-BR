---
author: JeremyKelley
description: Pesquise num locatário do SharePoint por sites que correspondam a palavras-chave fornecidas.
ms.date: 09/10/2017
title: Localizar sites do SharePoint por palavra-chave
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: c41f49f217e669a35ef77872161394186ec4b392
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42453202"
---
# <a name="search-for-sites"></a><span data-ttu-id="6a5ca-103">Procurar sites</span><span class="sxs-lookup"><span data-stu-id="6a5ca-103">Search for sites</span></span>

<span data-ttu-id="6a5ca-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="6a5ca-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6a5ca-105">Pesquisar em um locatário do SharePoint para [sites][] que correspondam a palavras-chave fornecidas.</span><span class="sxs-lookup"><span data-stu-id="6a5ca-105">Search across a SharePoint tenant for [sites][] that match keywords provided.</span></span>

[sites]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="6a5ca-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="6a5ca-107">Permissions</span></span>

<span data-ttu-id="6a5ca-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6a5ca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6a5ca-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6a5ca-110">Permission type</span></span>                        | <span data-ttu-id="6a5ca-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6a5ca-111">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="6a5ca-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6a5ca-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="6a5ca-113">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a5ca-113">Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="6a5ca-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6a5ca-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6a5ca-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6a5ca-115">Not supported.</span></span>
|<span data-ttu-id="6a5ca-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6a5ca-116">Application</span></span>                            | <span data-ttu-id="6a5ca-117">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a5ca-117">Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="6a5ca-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6a5ca-118">HTTP request</span></span>
```http
GET /sites?$search={query}
```

# <a name="http"></a>[<span data-ttu-id="6a5ca-119">HTTP</span><span class="sxs-lookup"><span data-stu-id="6a5ca-119">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "search-sites", "scopes": "service.sharepoint sites.readwrite.all" } -->

```msgraph-interactive
GET https://graph.microsoft.com/beta/sites?$search={query}
```
# <a name="c"></a>[<span data-ttu-id="6a5ca-120">C#</span><span class="sxs-lookup"><span data-stu-id="6a5ca-120">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/search-sites-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6a5ca-121">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6a5ca-121">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/search-sites-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6a5ca-122">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6a5ca-122">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/search-sites-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="6a5ca-123">Resposta</span><span class="sxs-lookup"><span data-stu-id="6a5ca-123">Response</span></span>

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
><span data-ttu-id="6a5ca-124">**Observação:** A única propriedade que funciona para classificação é **createdDateTime**.</span><span class="sxs-lookup"><span data-stu-id="6a5ca-124">**Note:** The only property that works for sorting is **createdDateTime**.</span></span> <span data-ttu-id="6a5ca-125">O filtro de pesquisa é uma pesquisa de texto livre que usa várias propriedades ao recuperar os resultados da pesquisa.</span><span class="sxs-lookup"><span data-stu-id="6a5ca-125">The search filter is a free text search that uses multiple properties when retrieving the search results.</span></span>

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
