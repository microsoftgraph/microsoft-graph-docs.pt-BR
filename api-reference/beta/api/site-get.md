---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Obter um Site do SharePoint
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 69845652cef0f726ae466a093bf504320c0fdd50
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508570"
---
# <a name="get-a-site-resource"></a><span data-ttu-id="2ef38-102">Obter um recurso de site</span><span class="sxs-lookup"><span data-stu-id="2ef38-102">Get a site resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2ef38-p101">Recupere as propriedades e as relações de um recurso [site][]. Um recurso **site** representa um site de equipe no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="2ef38-p101">Retrieve properties and relationships for a [site][] resource. A **site** resource represents a team site in SharePoint.</span></span>

[site]: ../resources/site.md

<span data-ttu-id="2ef38-106">Um **site** é endereçado para ser um identificador exclusivo que é uma ID composta dos seguintes valores:</span><span class="sxs-lookup"><span data-stu-id="2ef38-106">A **site** is addressed be a unique identifier which is a composite ID of the following values:</span></span>

* <span data-ttu-id="2ef38-107">Nome do host do conjunto de sites (contoso.sharepoint.com)</span><span class="sxs-lookup"><span data-stu-id="2ef38-107">Site collection hostname (contoso.sharepoint.com)</span></span>
* <span data-ttu-id="2ef38-108">ID exclusiva do conjunto de sites (GUID)</span><span class="sxs-lookup"><span data-stu-id="2ef38-108">Site collection unique ID (GUID)</span></span>
* <span data-ttu-id="2ef38-109">ID exclusiva do site (GUID)</span><span class="sxs-lookup"><span data-stu-id="2ef38-109">Site unique ID (GUID)</span></span>

<span data-ttu-id="2ef38-110">Há também um identificador de site reservado, `root`, que sempre faz referência ao site raiz de um determinado destino da seguinte maneira:</span><span class="sxs-lookup"><span data-stu-id="2ef38-110">There is also a reserved site identifier, `root`, which always references the root site for a given target, as follows:</span></span>

* <span data-ttu-id="2ef38-111">`/sites/root`: O site raiz do locatário.</span><span class="sxs-lookup"><span data-stu-id="2ef38-111">`/sites/root`: The tenant root site.</span></span>
* <span data-ttu-id="2ef38-112">`/groups/{group-id}/sites/root`: O site da equipe do grupo.</span><span class="sxs-lookup"><span data-stu-id="2ef38-112">`/groups/{group-id}/sites/root`: The group's team site.</span></span>

## <a name="permissions"></a><span data-ttu-id="2ef38-113">Permissões</span><span class="sxs-lookup"><span data-stu-id="2ef38-113">Permissions</span></span>

<span data-ttu-id="2ef38-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2ef38-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2ef38-116">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2ef38-116">Permission type</span></span>      | <span data-ttu-id="2ef38-117">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2ef38-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2ef38-118">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2ef38-118">Delegated (work or school account)</span></span> | <span data-ttu-id="2ef38-119">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ef38-119">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="2ef38-120">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2ef38-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2ef38-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2ef38-121">Not supported.</span></span>    |
|<span data-ttu-id="2ef38-122">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2ef38-122">Application</span></span> | <span data-ttu-id="2ef38-123">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ef38-123">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="get-the-tenants-root-site"></a><span data-ttu-id="2ef38-124">Obter o site raiz do locatário</span><span class="sxs-lookup"><span data-stu-id="2ef38-124">Get the tenant's root site</span></span>

<span data-ttu-id="2ef38-125">Para acessar o site raiz do SharePoint dentro de um locatário:</span><span class="sxs-lookup"><span data-stu-id="2ef38-125">To access the root SharePoint site within a tenant:</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /sites/root
GET /sites/contoso.sharepoint.com
```

## <a name="access-a-site-by-server-relative-url"></a><span data-ttu-id="2ef38-126">Acesse um site pela URL relativa do servidor</span><span class="sxs-lookup"><span data-stu-id="2ef38-126">Access a site by server-relative URL</span></span>

<span data-ttu-id="2ef38-127">Se você tiver a URL relativa do servidor para um recurso **site**, crie uma solicitação da seguinte maneira:</span><span class="sxs-lookup"><span data-stu-id="2ef38-127">If you have the server-relative URL for a **site** resource, you can construct a request as follows:</span></span>

```http
GET /sites/{hostname}:/{server-relative-path}
```

## <a name="access-a-group-team-site"></a><span data-ttu-id="2ef38-128">Acesse um site de equipe do grupo</span><span class="sxs-lookup"><span data-stu-id="2ef38-128">Access a group team site</span></span>

<span data-ttu-id="2ef38-129">Para acessar o site de equipe de um grupo:</span><span class="sxs-lookup"><span data-stu-id="2ef38-129">To access the team site for a group:</span></span>

```http
GET /groups/{group-id}/sites/root
```

## <a name="example"></a><span data-ttu-id="2ef38-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2ef38-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="2ef38-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2ef38-131">Request</span></span>

<!-- { "blockType": "request", "name": "get-site" } -->

```http
GET /sites/{site-id}
```

### <a name="response"></a><span data-ttu-id="2ef38-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="2ef38-132">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.site", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

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
  "tocPath": "Sites/Get by ID",
  "suppressions": [
    "Error: /api-reference/beta/api/site-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
