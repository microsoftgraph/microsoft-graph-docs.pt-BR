---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Procurar sites
description: Pesquisar em um locatário do SharePoint para sites que correspondam a palavras-chave fornecidas.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 48a479df2f91dd4d60455a26c4e16f561ea88f83
ms.sourcegitcommit: bbe42a15dad4ffe037a6934ab6001b585b7574c2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/17/2019
ms.locfileid: "31904116"
---
# <a name="search-for-sites"></a><span data-ttu-id="a5bc8-103">Procurar sites</span><span class="sxs-lookup"><span data-stu-id="a5bc8-103">Search for sites</span></span>

<span data-ttu-id="a5bc8-104">Pesquisar em um locatário do SharePoint para [sites][] que correspondam a palavras-chave fornecidas.</span><span class="sxs-lookup"><span data-stu-id="a5bc8-104">Search across a SharePoint tenant for [sites][] that match keywords provided.</span></span>

[sites]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="a5bc8-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a5bc8-106">Permissions</span></span>

<span data-ttu-id="a5bc8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a5bc8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a5bc8-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a5bc8-109">Permission type</span></span>                        | <span data-ttu-id="a5bc8-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a5bc8-110">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="a5bc8-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a5bc8-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a5bc8-112">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5bc8-112">Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="a5bc8-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a5bc8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a5bc8-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a5bc8-114">Not supported.</span></span>
|<span data-ttu-id="a5bc8-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a5bc8-115">Application</span></span>                            | <span data-ttu-id="a5bc8-116">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5bc8-116">Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="a5bc8-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a5bc8-117">HTTP request</span></span>

<!-- { "blockType": "request", "name": "search-sites", "scopes": "sites.readwrite.all", "tags": "service.sharepoint" } -->

```http
GET /sites?search={query}
```

## <a name="response"></a><span data-ttu-id="a5bc8-118">Resposta</span><span class="sxs-lookup"><span data-stu-id="a5bc8-118">Response</span></span>

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
><span data-ttu-id="a5bc8-119">**Observação:** A única propriedade que funciona para classificação é **createdDateTime**.</span><span class="sxs-lookup"><span data-stu-id="a5bc8-119">**Note:** The only property that works for sorting is **createdDateTime**.</span></span> <span data-ttu-id="a5bc8-120">O filtro de pesquisa é uma pesquisa de texto livre que usa várias propriedades ao recuperar os resultados da pesquisa.</span><span class="sxs-lookup"><span data-stu-id="a5bc8-120">The search filter is a free text search that uses multiple properties when retrieving the search results.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Sites/Search"
} -->
