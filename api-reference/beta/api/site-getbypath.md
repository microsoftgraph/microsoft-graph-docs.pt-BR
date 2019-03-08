---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Obter site do SharePoint por caminho
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 574b6537fd218b2337f63f5966b267aa60f0f458
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2019
ms.locfileid: "30481087"
---
# <a name="get-a-site-resource-by-path"></a><span data-ttu-id="7d5f2-102">Obter um recurso de site pelo caminho</span><span class="sxs-lookup"><span data-stu-id="7d5f2-102">Get a site resource by path</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7d5f2-p101">Recupere as propriedades e as relações de um recurso [site][]. Um recurso **site** representa um site de equipe no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="7d5f2-p101">Retrieve properties and relationships for a [site][] resource. A **site** resource represents a team site in SharePoint.</span></span>

[site]: ../resources/site.md

<span data-ttu-id="7d5f2-106">Além de recuperar um [site pelo ID](site-get.md), você pode recuperar um site com base no caminho da URL relativa ao servidor.</span><span class="sxs-lookup"><span data-stu-id="7d5f2-106">In addition to retrieving a [site by ID](site-get.md) you can retrieve a site based on server-relative URL path.</span></span>

* <span data-ttu-id="7d5f2-107">Hostname do conjunto de sites (contoso.sharepoint.com)</span><span class="sxs-lookup"><span data-stu-id="7d5f2-107">Site collection hostname (contoso.sharepoint.com)</span></span>
* <span data-ttu-id="7d5f2-108">Caminho do site, em relação ao nome de host do servidor.</span><span class="sxs-lookup"><span data-stu-id="7d5f2-108">Site path, relative to server hostname.</span></span>

<span data-ttu-id="7d5f2-109">Há também um identificador de site reservado, `root`, que sempre faz referência ao site raiz de um determinado destino da seguinte maneira:</span><span class="sxs-lookup"><span data-stu-id="7d5f2-109">There is also a reserved site identifier, `root`, which always references the root site for a given target, as follows:</span></span>

* <span data-ttu-id="7d5f2-110">`/sites/root`: O site raiz do locatário.</span><span class="sxs-lookup"><span data-stu-id="7d5f2-110">`/sites/root`: The tenant root site.</span></span>
* <span data-ttu-id="7d5f2-111">`/groups/{group-id}/sites/root`: O site da equipe do grupo.</span><span class="sxs-lookup"><span data-stu-id="7d5f2-111">`/groups/{group-id}/sites/root`: The group's team site.</span></span>

## <a name="permissions"></a><span data-ttu-id="7d5f2-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="7d5f2-112">Permissions</span></span>

<span data-ttu-id="7d5f2-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7d5f2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7d5f2-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7d5f2-115">Permission type</span></span>      | <span data-ttu-id="7d5f2-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7d5f2-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7d5f2-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7d5f2-117">Delegated (work or school account)</span></span> | <span data-ttu-id="7d5f2-118">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d5f2-118">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="7d5f2-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7d5f2-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7d5f2-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7d5f2-120">Not supported.</span></span>    |
|<span data-ttu-id="7d5f2-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7d5f2-121">Application</span></span> | <span data-ttu-id="7d5f2-122">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d5f2-122">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7d5f2-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7d5f2-123">HTTP Request</span></span>

<span data-ttu-id="7d5f2-124">Para acessar o site raiz do SharePoint com um caminho relativo:</span><span class="sxs-lookup"><span data-stu-id="7d5f2-124">To access the root SharePoint site with a relative path:</span></span>

<!-- { "blockType": "request", "name": "get-site-by-hostname-and-path", "scopes": "service.sharepoint sites.read.all" } -->

```http
GET /sites/{hostname}:/{relative-path}
```

## <a name="response"></a><span data-ttu-id="7d5f2-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="7d5f2-125">Response</span></span>

<span data-ttu-id="7d5f2-126">Este método retorna um recurso de [site][] para o site referenciado pelo identificador exclusivo.</span><span class="sxs-lookup"><span data-stu-id="7d5f2-126">This method returns a [site][] resource for the site referenced by the unique identifier.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/api/site-getbypath.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
