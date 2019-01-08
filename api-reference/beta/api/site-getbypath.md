---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Acessar site do SharePoint pelo caminho
ms.openlocfilehash: 7d63fd3651ab870318af46a298d6b945f331eda8
ms.sourcegitcommit: 37591c2299c80e7675cd2b5f781e1eeeba628a60
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/08/2019
ms.locfileid: "27748273"
---
# <a name="get-a-site-resource-by-path"></a><span data-ttu-id="1fc02-102">Obter um recurso de site pelo caminho</span><span class="sxs-lookup"><span data-stu-id="1fc02-102">Get a site resource by path</span></span>

> <span data-ttu-id="1fc02-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="1fc02-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1fc02-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="1fc02-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1fc02-p102">Recupere as propriedades e as relações de um recurso [site][]. Um recurso **site** representa um site de equipe no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="1fc02-p102">Retrieve properties and relationships for a [site][] resource. A **site** resource represents a team site in SharePoint.</span></span>

[site]: ../resources/site.md

<span data-ttu-id="1fc02-108">Além de recuperar um [site pelo ID](site-get.md), você pode recuperar um site com base no caminho da URL relativa ao servidor.</span><span class="sxs-lookup"><span data-stu-id="1fc02-108">In addition to retrieving a [site by ID](site-get.md) you can retrieve a site based on server-relative URL path.</span></span>

* <span data-ttu-id="1fc02-109">Nome do host do conjunto de sites (contoso.sharepoint.com)</span><span class="sxs-lookup"><span data-stu-id="1fc02-109">Site collection hostname (contoso.sharepoint.com)</span></span>
* <span data-ttu-id="1fc02-110">Caminho do site, em relação ao nome de host do servidor.</span><span class="sxs-lookup"><span data-stu-id="1fc02-110">Site path, relative to server hostname.</span></span>

<span data-ttu-id="1fc02-111">Há também um identificador de site reservado, `root`, que sempre faz referência ao site raiz de um determinado destino da seguinte maneira:</span><span class="sxs-lookup"><span data-stu-id="1fc02-111">There is also a reserved site identifier, `root`, which always references the root site for a given target, as follows:</span></span>

* <span data-ttu-id="1fc02-112">`/sites/root`: O site raiz do locatário.</span><span class="sxs-lookup"><span data-stu-id="1fc02-112">`/sites/root`: The tenant root site.</span></span>
* <span data-ttu-id="1fc02-113">`/groups/{group-id}/sites/root`: O site da equipe do grupo.</span><span class="sxs-lookup"><span data-stu-id="1fc02-113">`/groups/{group-id}/sites/root`: The group's team site.</span></span>

## <a name="permissions"></a><span data-ttu-id="1fc02-114">Permissões</span><span class="sxs-lookup"><span data-stu-id="1fc02-114">Permissions</span></span>

<span data-ttu-id="1fc02-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1fc02-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1fc02-117">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1fc02-117">Permission type</span></span>      | <span data-ttu-id="1fc02-118">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1fc02-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1fc02-119">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1fc02-119">Delegated (work or school account)</span></span> | <span data-ttu-id="1fc02-120">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1fc02-120">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="1fc02-121">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1fc02-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1fc02-122">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1fc02-122">Not supported.</span></span>    |
|<span data-ttu-id="1fc02-123">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1fc02-123">Application</span></span> | <span data-ttu-id="1fc02-124">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1fc02-124">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1fc02-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1fc02-125">HTTP Request</span></span>

<span data-ttu-id="1fc02-126">Para acessar o site raiz do SharePoint com um caminho relativo:</span><span class="sxs-lookup"><span data-stu-id="1fc02-126">To access the root SharePoint site with a relative path:</span></span>

<!-- { "blockType": "request", "name": "get-site-by-hostname-and-path", "scopes": "service.sharepoint sites.read.all" } -->

```http
GET /sites/{hostname}:/{relative-path}
```

## <a name="response"></a><span data-ttu-id="1fc02-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="1fc02-127">Response</span></span>

<span data-ttu-id="1fc02-128">Este método retorna um recurso de [site][] para o site referenciado pelo identificador exclusivo.</span><span class="sxs-lookup"><span data-stu-id="1fc02-128">This method returns a [site][] resource for the site referenced by the unique identifier.</span></span>

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

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Sites/Get by path"
} -->
