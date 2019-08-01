---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Obter site do SharePoint por caminho
localization_priority: Normal
ms.prod: sharepoint
description: Recupere as propriedades e as relações de um recurso de site.
doc_type: apiPageType
ms.openlocfilehash: 5e6195ddb90578d31d4cf68f081aafebbd004e24
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36021470"
---
# <a name="get-a-site-resource-by-path"></a><span data-ttu-id="2815c-103">Obter um recurso de site pelo caminho</span><span class="sxs-lookup"><span data-stu-id="2815c-103">Get a site resource by path</span></span>

<span data-ttu-id="2815c-p101">Recupere as propriedades e as relações de um recurso [site][]. Um recurso **site** representa um site de equipe no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="2815c-p101">Retrieve properties and relationships for a [site][] resource. A **site** resource represents a team site in SharePoint.</span></span>

[site]: ../resources/site.md

<span data-ttu-id="2815c-107">Além de recuperar um [site pelo ID](site-get.md), você pode recuperar um site com base no caminho da URL relativa ao servidor.</span><span class="sxs-lookup"><span data-stu-id="2815c-107">In addition to retrieving a [site by ID](site-get.md) you can retrieve a site based on server-relative URL path.</span></span>

* <span data-ttu-id="2815c-108">Hostname do conjunto de sites (contoso.sharepoint.com)</span><span class="sxs-lookup"><span data-stu-id="2815c-108">Site collection hostname (contoso.sharepoint.com)</span></span>
* <span data-ttu-id="2815c-109">Caminho do site, em relação ao nome de host do servidor.</span><span class="sxs-lookup"><span data-stu-id="2815c-109">Site path, relative to server hostname.</span></span>

<span data-ttu-id="2815c-110">Há também um identificador de site reservado, `root`, que sempre faz referência ao site raiz de um determinado destino da seguinte maneira:</span><span class="sxs-lookup"><span data-stu-id="2815c-110">There is also a reserved site identifier, `root`, which always references the root site for a given target, as follows:</span></span>

* <span data-ttu-id="2815c-111">`/sites/root`: O site raiz do locatário.</span><span class="sxs-lookup"><span data-stu-id="2815c-111">`/sites/root`: The tenant root site.</span></span>
* <span data-ttu-id="2815c-112">`/groups/{group-id}/sites/root`: O site da equipe do grupo.</span><span class="sxs-lookup"><span data-stu-id="2815c-112">`/groups/{group-id}/sites/root`: The group's team site.</span></span>

## <a name="permissions"></a><span data-ttu-id="2815c-113">Permissões</span><span class="sxs-lookup"><span data-stu-id="2815c-113">Permissions</span></span>

<span data-ttu-id="2815c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2815c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2815c-116">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2815c-116">Permission type</span></span>      | <span data-ttu-id="2815c-117">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2815c-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2815c-118">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2815c-118">Delegated (work or school account)</span></span> | <span data-ttu-id="2815c-119">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2815c-119">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="2815c-120">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2815c-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2815c-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2815c-121">Not supported.</span></span>    |
|<span data-ttu-id="2815c-122">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2815c-122">Application</span></span> | <span data-ttu-id="2815c-123">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2815c-123">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2815c-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2815c-124">HTTP Request</span></span>

<span data-ttu-id="2815c-125">Para acessar o site raiz do SharePoint com um caminho relativo:</span><span class="sxs-lookup"><span data-stu-id="2815c-125">To access the root SharePoint site with a relative path:</span></span>

<!-- { "blockType": "request", "name": "get-site-by-hostname-and-path", "scopes": "sites.read.all", "tags": "service.sharepoint" } -->

```http
GET /sites/{hostname}:/{relative-path}
```

## <a name="response"></a><span data-ttu-id="2815c-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="2815c-126">Response</span></span>

<span data-ttu-id="2815c-127">Este método retorna um recurso de [site][] para o site referenciado pelo identificador exclusivo.</span><span class="sxs-lookup"><span data-stu-id="2815c-127">This method returns a [site][] resource for the site referenced by the unique identifier.</span></span>

<!-- { "blockType": "response", "truncated": true, "@odata.type": "microsoft.graph.site" } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "contoso.sharepoint.com,2C712604-1370-44E7-A1F5-426573FDA80A,2D2244C3-251A-49EA-93A8-39E1C3A060FE",
  "displayName": "OneDrive Team Site",
  "name": "1drvteam",
  "createdDateTime": "2017-05-09T20:56:00Z",
  "lastModifiedDateTime": "2017-05-09T20:56:01Z",
  "webUrl": "https://contoso.sharepoint.com/teams/1drvteam"
}
```

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Warning: Couldn't serialize request for path /sites/{var}/children/{var} into EDMX: System.InvalidOperationException: Uri path requires navigating into unknown object hierarchy: missing property 'children' on 'site'. Possible issues:
         1) Doc bug where 'children' isn't defined on the resource.      2) Doc bug where 'children' is an example key and should instead be replaced with a placeholder like {item-id} or declared in the sampleKeys annotation.       3) Doc bug where 'site' is supposed to be an entity type, but is being treated as a complex because it (and its ancestors) are missing the keyProperty annotation
     at ApiDocs.Publishing.CSDL.CsdlWriter.ParseRequestTargetType(String requestPath, MethodCollection requestMethodCollection, EntityFramework edmx, IssueLogger issues) in D:/src/mds2/ApiDocs.Publishing/CSDL/CsdlWriter.cs:line 982
     at ApiDocs.Publishing.CSDL.CsdlWriter.ProcessRestRequestPaths(EntityFramework edmx, String[] baseUrlsToRemove, IssueLogger issues) in D:/src/mds2/ApiDocs.Publishing/CSDL/CsdlWriter.cs:line 653"
  ],
  "tocPath": "Sites/Get by path"
} -->
