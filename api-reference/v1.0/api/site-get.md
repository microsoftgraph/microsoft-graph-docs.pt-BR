---
author: JeremyKelley
ms.date: 09/10/2017
title: Obter um Site do SharePoint
localization_priority: Priority
ms.prod: sharepoint
description: Recupere as propriedades e as relações de um recurso do site.
doc_type: apiPageType
ms.openlocfilehash: cb95e5c4568a982529a04adccac11d458efa7cd2
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/14/2021
ms.locfileid: "50239300"
---
# <a name="get-a-site-resource"></a><span data-ttu-id="adc98-103">Obter um recurso de site</span><span class="sxs-lookup"><span data-stu-id="adc98-103">Get a site resource</span></span>

<span data-ttu-id="adc98-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="adc98-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="adc98-p101">Recupere as propriedades e as relações de um recurso [site][]. Um recurso **site** representa um site de equipe no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="adc98-p101">Retrieve properties and relationships for a [site][] resource. A **site** resource represents a team site in SharePoint.</span></span>

[site]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="adc98-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="adc98-108">Permissions</span></span>

<span data-ttu-id="adc98-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="adc98-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="adc98-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="adc98-111">Permission type</span></span>      | <span data-ttu-id="adc98-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="adc98-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="adc98-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="adc98-113">Delegated (work or school account)</span></span> | <span data-ttu-id="adc98-114">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="adc98-114">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="adc98-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="adc98-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="adc98-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="adc98-116">Not supported.</span></span>    |
|<span data-ttu-id="adc98-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="adc98-117">Application</span></span> | <span data-ttu-id="adc98-118">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="adc98-118">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="get-the-tenants-root-site"></a><span data-ttu-id="adc98-119">Obter o site raiz do locatário</span><span class="sxs-lookup"><span data-stu-id="adc98-119">Get the tenant's root site</span></span>

<span data-ttu-id="adc98-120">Para acessar o site raiz do SharePoint dentro de um locatário:</span><span class="sxs-lookup"><span data-stu-id="adc98-120">To access the root SharePoint site within a tenant:</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /sites/root
GET /sites/contoso.sharepoint.com
```

## <a name="access-a-site-by-server-relative-url"></a><span data-ttu-id="adc98-121">Acesse um site pela URL relativa do servidor</span><span class="sxs-lookup"><span data-stu-id="adc98-121">Access a site by server-relative URL</span></span>

<span data-ttu-id="adc98-122">Se você tiver a URL relativa do servidor para um recurso **site**, crie uma solicitação da seguinte maneira:</span><span class="sxs-lookup"><span data-stu-id="adc98-122">If you have the server-relative URL for a **site** resource, you can construct a request as follows:</span></span>

```http
GET /sites/{hostname}:/{server-relative-path}
```

## <a name="access-a-group-team-site"></a><span data-ttu-id="adc98-123">Acesse um site de equipe do grupo</span><span class="sxs-lookup"><span data-stu-id="adc98-123">Access a group team site</span></span>

<span data-ttu-id="adc98-124">Para acessar o site de equipe de um grupo:</span><span class="sxs-lookup"><span data-stu-id="adc98-124">To access the team site for a group:</span></span>

```http
GET /groups/{group-id}/sites/root
```

## <a name="example"></a><span data-ttu-id="adc98-125">Exemplo</span><span class="sxs-lookup"><span data-stu-id="adc98-125">Example</span></span>

### <a name="request"></a><span data-ttu-id="adc98-126">Solicitação</span><span class="sxs-lookup"><span data-stu-id="adc98-126">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="adc98-127">HTTP</span><span class="sxs-lookup"><span data-stu-id="adc98-127">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-site", "scopes": "sites.read.all" } -->

```msgraph-interactive
GET /sites/{site-id}
```
# <a name="c"></a>[<span data-ttu-id="adc98-128">C#</span><span class="sxs-lookup"><span data-stu-id="adc98-128">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-site-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="adc98-129">JavaScript</span><span class="sxs-lookup"><span data-stu-id="adc98-129">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-site-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="adc98-130">Objective-C</span><span class="sxs-lookup"><span data-stu-id="adc98-130">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-site-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="adc98-131">Java</span><span class="sxs-lookup"><span data-stu-id="adc98-131">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-site-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="adc98-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="adc98-132">Response</span></span>

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

