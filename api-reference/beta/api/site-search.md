---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Localizar sites do SharePoint por palavra-chave
ms.openlocfilehash: c3c5ba005521e3405018e9b9403976297046f242
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041166"
---
# <a name="search-for-sites"></a><span data-ttu-id="fc4c7-102">Procurar sites</span><span class="sxs-lookup"><span data-stu-id="fc4c7-102">Search for sites</span></span>

> <span data-ttu-id="fc4c7-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="fc4c7-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fc4c7-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="fc4c7-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fc4c7-105">Pesquise em um locatário do SharePoint por [sites][] que correspondam a palavras-chave fornecidas.</span><span class="sxs-lookup"><span data-stu-id="fc4c7-105">Search across a SharePoint tenant for [sites][] that match provided keywords.</span></span>

[sites]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="fc4c7-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="fc4c7-107">Permissions</span></span>

<span data-ttu-id="fc4c7-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fc4c7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fc4c7-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fc4c7-110">Permission type</span></span>                        | <span data-ttu-id="fc4c7-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fc4c7-111">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="fc4c7-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fc4c7-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="fc4c7-113">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc4c7-113">Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="fc4c7-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fc4c7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fc4c7-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fc4c7-115">Not supported.</span></span>
|<span data-ttu-id="fc4c7-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fc4c7-116">Application</span></span>                            | <span data-ttu-id="fc4c7-117">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc4c7-117">Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="fc4c7-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fc4c7-118">HTTP request</span></span>

<!-- { "blockType": "request", "name": "search-sites", "scopes": "service.sharepoint sites.readwrite.all" } -->

```http
GET https://graph.microsoft.com/beta/sites?search={query}
```

## <a name="response"></a><span data-ttu-id="fc4c7-119">Resposta</span><span class="sxs-lookup"><span data-stu-id="fc4c7-119">Response</span></span>

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
