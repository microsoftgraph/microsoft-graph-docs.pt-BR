---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Obter um Site do SharePoint
localization_priority: Normal
ms.openlocfilehash: 72a99b1768486da792a401cea4b8dfde5a25a153
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27872853"
---
# <a name="get-a-site-resource"></a><span data-ttu-id="eed9d-102">Obter um recurso de site</span><span class="sxs-lookup"><span data-stu-id="eed9d-102">Get a site resource</span></span>

> <span data-ttu-id="eed9d-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="eed9d-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="eed9d-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="eed9d-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="eed9d-p102">Recupere as propriedades e as relações de um recurso [site][]. Um recurso **site** representa um site de equipe no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="eed9d-p102">Retrieve properties and relationships for a [site][] resource. A **site** resource represents a team site in SharePoint.</span></span>

[site]: ../resources/site.md

<span data-ttu-id="eed9d-108">Um **site** é endereçado para ser um identificador exclusivo que é uma ID composta dos seguintes valores:</span><span class="sxs-lookup"><span data-stu-id="eed9d-108">A **site** is addressed be a unique identifier which is a composite ID of the following values:</span></span>

* <span data-ttu-id="eed9d-109">Nome do host do conjunto de sites (contoso.sharepoint.com)</span><span class="sxs-lookup"><span data-stu-id="eed9d-109">Site collection hostname (contoso.sharepoint.com)</span></span>
* <span data-ttu-id="eed9d-110">ID exclusiva do conjunto de sites (GUID)</span><span class="sxs-lookup"><span data-stu-id="eed9d-110">Site collection unique ID (GUID)</span></span>
* <span data-ttu-id="eed9d-111">ID exclusiva do site (GUID)</span><span class="sxs-lookup"><span data-stu-id="eed9d-111">Site unique ID (GUID)</span></span>

<span data-ttu-id="eed9d-112">Há também um identificador de site reservado, `root`, que sempre faz referência ao site raiz de um determinado destino da seguinte maneira:</span><span class="sxs-lookup"><span data-stu-id="eed9d-112">There is also a reserved site identifier, `root`, which always references the root site for a given target, as follows:</span></span>

* <span data-ttu-id="eed9d-113">`/sites/root`: O site raiz do locatário.</span><span class="sxs-lookup"><span data-stu-id="eed9d-113">`/sites/root`: The tenant root site.</span></span>
* <span data-ttu-id="eed9d-114">`/groups/{group-id}/sites/root`: O site da equipe do grupo.</span><span class="sxs-lookup"><span data-stu-id="eed9d-114">`/groups/{group-id}/sites/root`: The group's team site.</span></span>

## <a name="permissions"></a><span data-ttu-id="eed9d-115">Permissões</span><span class="sxs-lookup"><span data-stu-id="eed9d-115">Permissions</span></span>

<span data-ttu-id="eed9d-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eed9d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eed9d-118">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eed9d-118">Permission type</span></span>      | <span data-ttu-id="eed9d-119">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="eed9d-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eed9d-120">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eed9d-120">Delegated (work or school account)</span></span> | <span data-ttu-id="eed9d-121">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eed9d-121">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="eed9d-122">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eed9d-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eed9d-123">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eed9d-123">Not supported.</span></span>    |
|<span data-ttu-id="eed9d-124">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eed9d-124">Application</span></span> | <span data-ttu-id="eed9d-125">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eed9d-125">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="get-the-tenants-root-site"></a><span data-ttu-id="eed9d-126">Obter o site raiz do locatário</span><span class="sxs-lookup"><span data-stu-id="eed9d-126">Get the tenant's root site</span></span>

<span data-ttu-id="eed9d-127">Para acessar o site raiz do SharePoint dentro de um locatário:</span><span class="sxs-lookup"><span data-stu-id="eed9d-127">To access the root SharePoint site within a tenant:</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /sites/root
GET /sites/contoso.sharepoint.com
```

## <a name="access-a-site-by-server-relative-url"></a><span data-ttu-id="eed9d-128">Acesse um site pela URL relativa do servidor</span><span class="sxs-lookup"><span data-stu-id="eed9d-128">Access a site by server-relative URL</span></span>

<span data-ttu-id="eed9d-129">Se você tiver a URL relativa do servidor para um recurso **site**, crie uma solicitação da seguinte maneira:</span><span class="sxs-lookup"><span data-stu-id="eed9d-129">If you have the server-relative URL for a **site** resource, you can construct a request as follows:</span></span>

```http
GET /sites/{hostname}:/{server-relative-path}
```

## <a name="access-a-group-team-site"></a><span data-ttu-id="eed9d-130">Acesse um site de equipe do grupo</span><span class="sxs-lookup"><span data-stu-id="eed9d-130">Access a group team site</span></span>

<span data-ttu-id="eed9d-131">Para acessar o site de equipe de um grupo:</span><span class="sxs-lookup"><span data-stu-id="eed9d-131">To access the team site for a group:</span></span>

```http
GET /groups/{group-id}/sites/root
```

## <a name="example"></a><span data-ttu-id="eed9d-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="eed9d-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="eed9d-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eed9d-133">Request</span></span>

<!-- { "blockType": "request", "name": "get-site" } -->

```http
GET /sites/{site-id}
```

### <a name="response"></a><span data-ttu-id="eed9d-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="eed9d-134">Response</span></span>

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

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Sites/Get by ID"
} -->
