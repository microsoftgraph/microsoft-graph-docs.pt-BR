---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Obter um Site do SharePoint
localization_priority: Priority
ms.prod: sharepoint
description: Recupere as propriedades e as relações de um recurso do site.
doc_type: apiPageType
ms.openlocfilehash: af50b2eae0287ad31e75c6373b6dedb4c67bd42b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42509798"
---
# <a name="get-a-site-resource"></a><span data-ttu-id="2df42-103">Obter um recurso de site</span><span class="sxs-lookup"><span data-stu-id="2df42-103">Get a site resource</span></span>

<span data-ttu-id="2df42-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2df42-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2df42-p101">Recupere as propriedades e as relações de um recurso [site][]. Um recurso **site** representa um site de equipe no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="2df42-p101">Retrieve properties and relationships for a [site][] resource. A **site** resource represents a team site in SharePoint.</span></span>

[site]: ../resources/site.md

<span data-ttu-id="2df42-108">Um **site** é endereçado para ser um identificador exclusivo que é uma ID composta dos seguintes valores:</span><span class="sxs-lookup"><span data-stu-id="2df42-108">A **site** is addressed by a unique identifier which is a composite ID of the following values:</span></span>

* <span data-ttu-id="2df42-109">Hostname do conjunto de sites (contoso.sharepoint.com)</span><span class="sxs-lookup"><span data-stu-id="2df42-109">Site collection hostname (contoso.sharepoint.com)</span></span>
* <span data-ttu-id="2df42-110">ID exclusiva do conjunto de sites (GUID)</span><span class="sxs-lookup"><span data-stu-id="2df42-110">Site collection unique ID (GUID)</span></span>
* <span data-ttu-id="2df42-111">ID exclusiva do site (GUID)</span><span class="sxs-lookup"><span data-stu-id="2df42-111">Site unique ID (GUID)</span></span>

<span data-ttu-id="2df42-112">Há também um identificador de site reservado, `root`, que sempre faz referência ao site raiz de um determinado destino da seguinte maneira:</span><span class="sxs-lookup"><span data-stu-id="2df42-112">There is also a reserved site identifier, `root`, which always references the root site for a given target, as follows:</span></span>

* <span data-ttu-id="2df42-113">`/sites/root`: O site raiz do locatário.</span><span class="sxs-lookup"><span data-stu-id="2df42-113">`/sites/root`: The tenant root site.</span></span>
* <span data-ttu-id="2df42-114">`/groups/{group-id}/sites/root`: O site da equipe do grupo.</span><span class="sxs-lookup"><span data-stu-id="2df42-114">`/groups/{group-id}/sites/root`: The group's team site.</span></span>

## <a name="permissions"></a><span data-ttu-id="2df42-115">Permissões</span><span class="sxs-lookup"><span data-stu-id="2df42-115">Permissions</span></span>

<span data-ttu-id="2df42-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2df42-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2df42-118">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2df42-118">Permission type</span></span>      | <span data-ttu-id="2df42-119">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2df42-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2df42-120">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2df42-120">Delegated (work or school account)</span></span> | <span data-ttu-id="2df42-121">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2df42-121">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="2df42-122">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2df42-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2df42-123">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2df42-123">Not supported.</span></span>    |
|<span data-ttu-id="2df42-124">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2df42-124">Application</span></span> | <span data-ttu-id="2df42-125">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2df42-125">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="get-the-tenants-root-site"></a><span data-ttu-id="2df42-126">Obter o site raiz do locatário</span><span class="sxs-lookup"><span data-stu-id="2df42-126">Get the tenant's root site</span></span>

<span data-ttu-id="2df42-127">Para acessar o site raiz do SharePoint dentro de um locatário:</span><span class="sxs-lookup"><span data-stu-id="2df42-127">To access the root SharePoint site within a tenant:</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /sites/root
GET /sites/contoso.sharepoint.com
```

## <a name="access-a-site-by-server-relative-url"></a><span data-ttu-id="2df42-128">Acesse um site pela URL relativa do servidor</span><span class="sxs-lookup"><span data-stu-id="2df42-128">Access a site by server-relative URL</span></span>

<span data-ttu-id="2df42-129">Se você tiver a URL relativa do servidor para um recurso **site**, crie uma solicitação da seguinte maneira:</span><span class="sxs-lookup"><span data-stu-id="2df42-129">If you have the server-relative URL for a **site** resource, you can construct a request as follows:</span></span>

```http
GET /sites/{hostname}:/{server-relative-path}
```

## <a name="access-a-group-team-site"></a><span data-ttu-id="2df42-130">Acesse um site de equipe do grupo</span><span class="sxs-lookup"><span data-stu-id="2df42-130">Access a group team site</span></span>

<span data-ttu-id="2df42-131">Para acessar o site de equipe de um grupo:</span><span class="sxs-lookup"><span data-stu-id="2df42-131">To access the team site for a group:</span></span>

```http
GET /groups/{group-id}/sites/root
```

## <a name="example"></a><span data-ttu-id="2df42-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2df42-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="2df42-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2df42-133">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="2df42-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="2df42-134">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-site", "scopes": "sites.read.all" } -->

```msgraph-interactive
GET /sites/{site-id}
```
# <a name="c"></a>[<span data-ttu-id="2df42-135">C#</span><span class="sxs-lookup"><span data-stu-id="2df42-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-site-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2df42-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2df42-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-site-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2df42-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2df42-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-site-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2df42-138">Java</span><span class="sxs-lookup"><span data-stu-id="2df42-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-site-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2df42-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="2df42-139">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.site", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

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
  "tocPath": "Sites/Get by ID",
  "suppressions": [
  ]
} -->
