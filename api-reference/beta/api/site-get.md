---
author: JeremyKelley
description: Recupere as propriedades e as relações de um recurso de site.
ms.date: 09/10/2017
title: Obter um Site do SharePoint
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: aab284d6ae15bf42e2e33621248e0b809c8c1089
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35977871"
---
# <a name="get-a-site-resource"></a><span data-ttu-id="8962c-103">Obter um recurso de site</span><span class="sxs-lookup"><span data-stu-id="8962c-103">Get a site resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8962c-p101">Recupere as propriedades e as relações de um recurso [site][]. Um recurso **site** representa um site de equipe no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="8962c-p101">Retrieve properties and relationships for a [site][] resource. A **site** resource represents a team site in SharePoint.</span></span>

[site]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="8962c-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="8962c-107">Permissions</span></span>

<span data-ttu-id="8962c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8962c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8962c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8962c-110">Permission type</span></span>      | <span data-ttu-id="8962c-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8962c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8962c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8962c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8962c-113">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8962c-113">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="8962c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8962c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8962c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8962c-115">Not supported.</span></span>    |
|<span data-ttu-id="8962c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8962c-116">Application</span></span> | <span data-ttu-id="8962c-117">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8962c-117">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="get-the-tenants-root-site"></a><span data-ttu-id="8962c-118">Obter o site raiz do locatário</span><span class="sxs-lookup"><span data-stu-id="8962c-118">Get the tenant's root site</span></span>

<span data-ttu-id="8962c-119">Para acessar o site raiz do SharePoint dentro de um locatário:</span><span class="sxs-lookup"><span data-stu-id="8962c-119">To access the root SharePoint site within a tenant:</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /sites/root
GET /sites/contoso.sharepoint.com
```

## <a name="access-a-site-by-server-relative-url"></a><span data-ttu-id="8962c-120">Acesse um site pela URL relativa do servidor</span><span class="sxs-lookup"><span data-stu-id="8962c-120">Access a site by server-relative URL</span></span>

<span data-ttu-id="8962c-121">Se você tiver a URL relativa do servidor para um recurso **site**, crie uma solicitação da seguinte maneira:</span><span class="sxs-lookup"><span data-stu-id="8962c-121">If you have the server-relative URL for a **site** resource, you can construct a request as follows:</span></span>

```http
GET /sites/{hostname}:/{server-relative-path}
```

## <a name="access-a-group-team-site"></a><span data-ttu-id="8962c-122">Acesse um site de equipe do grupo</span><span class="sxs-lookup"><span data-stu-id="8962c-122">Access a group team site</span></span>

<span data-ttu-id="8962c-123">Para acessar o site de equipe de um grupo:</span><span class="sxs-lookup"><span data-stu-id="8962c-123">To access the team site for a group:</span></span>

```http
GET /groups/{group-id}/sites/root
```

## <a name="example"></a><span data-ttu-id="8962c-124">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8962c-124">Example</span></span>

### <a name="request"></a><span data-ttu-id="8962c-125">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8962c-125">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="8962c-126">HTTP</span><span class="sxs-lookup"><span data-stu-id="8962c-126">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-site" } -->

```http
GET /sites/{site-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8962c-127">C#</span><span class="sxs-lookup"><span data-stu-id="8962c-127">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-site-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8962c-128">Javascript</span><span class="sxs-lookup"><span data-stu-id="8962c-128">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-site-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8962c-129">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="8962c-129">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-site-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="8962c-130">Java</span><span class="sxs-lookup"><span data-stu-id="8962c-130">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-site-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8962c-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="8962c-131">Response</span></span>

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
  ]
}
-->
