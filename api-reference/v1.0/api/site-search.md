---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Localizar sites do SharePoint por palavra-chave
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 03e5a43c80ff5107f4e3aca514b1b411d71eb61d
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2019
ms.locfileid: "30482116"
---
# <a name="search-for-sites"></a><span data-ttu-id="223a7-102">Procurar sites</span><span class="sxs-lookup"><span data-stu-id="223a7-102">Search for sites</span></span>

<span data-ttu-id="223a7-103">Pesquise em um locatário do SharePoint por [sites][] que correspondam a palavras-chave fornecidas.</span><span class="sxs-lookup"><span data-stu-id="223a7-103">Search across a SharePoint tenant for [sites][] that match provided keywords.</span></span>

[sites]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="223a7-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="223a7-105">Permissions</span></span>

<span data-ttu-id="223a7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="223a7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="223a7-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="223a7-108">Permission type</span></span>                        | <span data-ttu-id="223a7-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="223a7-109">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="223a7-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="223a7-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="223a7-111">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="223a7-111">Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="223a7-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="223a7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="223a7-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="223a7-113">Not supported.</span></span>
|<span data-ttu-id="223a7-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="223a7-114">Application</span></span>                            | <span data-ttu-id="223a7-115">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="223a7-115">Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="223a7-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="223a7-116">HTTP request</span></span>

<!-- { "blockType": "request", "name": "search-sites", "scopes": "sites.readwrite.all", "tags": "service.sharepoint" } -->

```http
GET /sites?search={query}
```

## <a name="response"></a><span data-ttu-id="223a7-117">Resposta</span><span class="sxs-lookup"><span data-stu-id="223a7-117">Response</span></span>

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

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Sites/Search"
} -->
