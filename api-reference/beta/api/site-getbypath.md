---
author: JeremyKelley
description: Recupere as propriedades e as relações de um recurso do site.
ms.date: 09/10/2017
title: Obter site do SharePoint por caminho
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: f5b61c84146701782c1dbe5e8b24631ca30bbb79
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48013969"
---
# <a name="get-a-site-resource-by-path"></a><span data-ttu-id="ce7e0-103">Obter um recurso de site pelo caminho</span><span class="sxs-lookup"><span data-stu-id="ce7e0-103">Get a site resource by path</span></span>

<span data-ttu-id="ce7e0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ce7e0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ce7e0-p101">Recupere as propriedades e as relações de um recurso [site][]. Um recurso **site** representa um site de equipe no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="ce7e0-p101">Retrieve properties and relationships for a [site][] resource. A **site** resource represents a team site in SharePoint.</span></span>

[site]: ../resources/site.md

<span data-ttu-id="ce7e0-108">Além de recuperar um [site pelo ID](site-get.md), você pode recuperar um site com base no caminho da URL relativa ao servidor.</span><span class="sxs-lookup"><span data-stu-id="ce7e0-108">In addition to retrieving a [site by ID](site-get.md) you can retrieve a site based on server-relative URL path.</span></span>

* <span data-ttu-id="ce7e0-109">Hostname do conjunto de sites (contoso.sharepoint.com)</span><span class="sxs-lookup"><span data-stu-id="ce7e0-109">Site collection hostname (contoso.sharepoint.com)</span></span>
* <span data-ttu-id="ce7e0-110">Caminho do site, em relação ao nome de host do servidor.</span><span class="sxs-lookup"><span data-stu-id="ce7e0-110">Site path, relative to server hostname.</span></span>

<span data-ttu-id="ce7e0-111">Há também um identificador de site reservado, `root`, que sempre faz referência ao site raiz de um determinado destino da seguinte maneira:</span><span class="sxs-lookup"><span data-stu-id="ce7e0-111">There is also a reserved site identifier, `root`, which always references the root site for a given target, as follows:</span></span>

* <span data-ttu-id="ce7e0-112">`/sites/root`: O site raiz do locatário.</span><span class="sxs-lookup"><span data-stu-id="ce7e0-112">`/sites/root`: The tenant root site.</span></span>
* <span data-ttu-id="ce7e0-113">`/groups/{group-id}/sites/root`: O site da equipe do grupo.</span><span class="sxs-lookup"><span data-stu-id="ce7e0-113">`/groups/{group-id}/sites/root`: The group's team site.</span></span>

## <a name="permissions"></a><span data-ttu-id="ce7e0-114">Permissões</span><span class="sxs-lookup"><span data-stu-id="ce7e0-114">Permissions</span></span>

<span data-ttu-id="ce7e0-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ce7e0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ce7e0-117">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ce7e0-117">Permission type</span></span>      | <span data-ttu-id="ce7e0-118">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ce7e0-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ce7e0-119">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ce7e0-119">Delegated (work or school account)</span></span> | <span data-ttu-id="ce7e0-120">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce7e0-120">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="ce7e0-121">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ce7e0-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ce7e0-122">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ce7e0-122">Not supported.</span></span>    |
|<span data-ttu-id="ce7e0-123">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ce7e0-123">Application</span></span> | <span data-ttu-id="ce7e0-124">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce7e0-124">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ce7e0-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ce7e0-125">HTTP Request</span></span>

<span data-ttu-id="ce7e0-126">Para acessar o site raiz do SharePoint com um caminho relativo:</span><span class="sxs-lookup"><span data-stu-id="ce7e0-126">To access the root SharePoint site with a relative path:</span></span>

<!-- { "blockType": "request", "name": "get-site-by-hostname-and-path", "scopes": "service.sharepoint sites.read.all" } -->

```http
GET /sites/{hostname}:/{relative-path}
```

## <a name="response"></a><span data-ttu-id="ce7e0-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="ce7e0-127">Response</span></span>

<span data-ttu-id="ce7e0-128">Este método retorna um recurso de [site][] para o site referenciado pelo identificador exclusivo.</span><span class="sxs-lookup"><span data-stu-id="ce7e0-128">This method returns a [site][] resource for the site referenced by the unique identifier.</span></span>

<!-- { "blockType": "response", "truncated": true, "@odata.type": "microsoft.graph.site" } -->

```http
HTTP/1.1 200 OK

{
  "id": "contoso.sharepoint.com,2C712604-1370-44E7-A1F5-426573FDA80A,2D2244C3-251A-49EA-93A8-39E1C3A060FE",
  "owner": {
    "user": { 
      "displayName": "Daron Spektor",
      "id": "5280E7FE-DC7A-4486-9490-E790D81DFEB3"
    }
  },
  "displayName": "OneDrive Team Site",
  "name": "1drvteam",
  "createdDateTime": "2017-05-09T20:56:00Z",
  "lastModifiedDateTime": "2017-05-09T20:56:01Z",
  "webUrl": "https://contoso.sharepoint.com/teams/1drvteam"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Sites/Get by path",
  "suppressions": []
}
-->


