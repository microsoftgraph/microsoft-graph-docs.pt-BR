---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Acessar site do SharePoint pelo caminho
localization_priority: Normal
ms.openlocfilehash: 4dab98e342c012884232cca21cd532b63b450ea8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27867834"
---
# <a name="get-a-site-resource-by-path"></a><span data-ttu-id="18dd9-102">Obter um recurso de site pelo caminho</span><span class="sxs-lookup"><span data-stu-id="18dd9-102">Get a site resource by path</span></span>

<span data-ttu-id="18dd9-p101">Recupere as propriedades e as relações de um recurso [site][]. Um recurso **site** representa um site de equipe no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="18dd9-p101">Retrieve properties and relationships for a [site][] resource. A **site** resource represents a team site in SharePoint.</span></span>

[site]: ../resources/site.md

<span data-ttu-id="18dd9-106">Além de recuperar um [site pelo ID](site-get.md), você pode recuperar um site com base no caminho da URL relativa ao servidor.</span><span class="sxs-lookup"><span data-stu-id="18dd9-106">In addition to retrieving a [site by ID](site-get.md) you can retrieve a site based on server-relative URL path.</span></span>

* <span data-ttu-id="18dd9-107">Nome do host do conjunto de sites (contoso.sharepoint.com)</span><span class="sxs-lookup"><span data-stu-id="18dd9-107">Site collection hostname (contoso.sharepoint.com)</span></span>
* <span data-ttu-id="18dd9-108">Caminho do site, em relação ao nome de host do servidor.</span><span class="sxs-lookup"><span data-stu-id="18dd9-108">Site path, relative to server hostname.</span></span>

<span data-ttu-id="18dd9-109">Há também um identificador de site reservado, `root`, que sempre faz referência ao site raiz de um determinado destino da seguinte maneira:</span><span class="sxs-lookup"><span data-stu-id="18dd9-109">There is also a reserved site identifier, `root`, which always references the root site for a given target, as follows:</span></span>

* <span data-ttu-id="18dd9-110">`/sites/root`: O site raiz do locatário.</span><span class="sxs-lookup"><span data-stu-id="18dd9-110">`/sites/root`: The tenant root site.</span></span>
* <span data-ttu-id="18dd9-111">`/groups/{group-id}/sites/root`: O site da equipe do grupo.</span><span class="sxs-lookup"><span data-stu-id="18dd9-111">`/groups/{group-id}/sites/root`: The group's team site.</span></span>

## <a name="permissions"></a><span data-ttu-id="18dd9-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="18dd9-112">Permissions</span></span>

<span data-ttu-id="18dd9-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="18dd9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18dd9-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="18dd9-115">Permission type</span></span>      | <span data-ttu-id="18dd9-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="18dd9-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="18dd9-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="18dd9-117">Delegated (work or school account)</span></span> | <span data-ttu-id="18dd9-118">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18dd9-118">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="18dd9-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="18dd9-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="18dd9-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="18dd9-120">Not supported.</span></span>    |
|<span data-ttu-id="18dd9-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="18dd9-121">Application</span></span> | <span data-ttu-id="18dd9-122">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18dd9-122">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="18dd9-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="18dd9-123">HTTP Request</span></span>

<span data-ttu-id="18dd9-124">Para acessar o site raiz do SharePoint com um caminho relativo:</span><span class="sxs-lookup"><span data-stu-id="18dd9-124">To access the root SharePoint site with a relative path:</span></span>

<!-- { "blockType": "request", "name": "get-site-by-hostname-and-path", "scopes": "sites.read.all", "tags": "service.sharepoint" } -->

```http
GET /sites/{hostname}:/{relative-path}
```

## <a name="response"></a><span data-ttu-id="18dd9-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="18dd9-125">Response</span></span>

<span data-ttu-id="18dd9-126">Este método retorna um recurso de [site][] para o site referenciado pelo identificador exclusivo.</span><span class="sxs-lookup"><span data-stu-id="18dd9-126">This method returns a [site][] resource for the site referenced by the unique identifier.</span></span>

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
