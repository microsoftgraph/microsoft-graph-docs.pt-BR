---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Obter um Site do SharePoint
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 89efbcd3853e767316cc4b369a861476e7d30a76
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35457118"
---
# <a name="get-a-site-resource"></a><span data-ttu-id="af4e8-102">Obter um recurso de site</span><span class="sxs-lookup"><span data-stu-id="af4e8-102">Get a site resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="af4e8-p101">Recupere as propriedades e as relações de um recurso [site][]. Um recurso **site** representa um site de equipe no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="af4e8-p101">Retrieve properties and relationships for a [site][] resource. A **site** resource represents a team site in SharePoint.</span></span>

[site]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="af4e8-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="af4e8-106">Permissions</span></span>

<span data-ttu-id="af4e8-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="af4e8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="af4e8-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="af4e8-109">Permission type</span></span>      | <span data-ttu-id="af4e8-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="af4e8-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="af4e8-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="af4e8-111">Delegated (work or school account)</span></span> | <span data-ttu-id="af4e8-112">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af4e8-112">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="af4e8-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="af4e8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="af4e8-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="af4e8-114">Not supported.</span></span>    |
|<span data-ttu-id="af4e8-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="af4e8-115">Application</span></span> | <span data-ttu-id="af4e8-116">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af4e8-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="get-the-tenants-root-site"></a><span data-ttu-id="af4e8-117">Obter o site raiz do locatário</span><span class="sxs-lookup"><span data-stu-id="af4e8-117">Get the tenant's root site</span></span>

<span data-ttu-id="af4e8-118">Para acessar o site raiz do SharePoint dentro de um locatário:</span><span class="sxs-lookup"><span data-stu-id="af4e8-118">To access the root SharePoint site within a tenant:</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /sites/root
GET /sites/contoso.sharepoint.com
```

## <a name="access-a-site-by-server-relative-url"></a><span data-ttu-id="af4e8-119">Acesse um site pela URL relativa do servidor</span><span class="sxs-lookup"><span data-stu-id="af4e8-119">Access a site by server-relative URL</span></span>

<span data-ttu-id="af4e8-120">Se você tiver a URL relativa do servidor para um recurso **site**, crie uma solicitação da seguinte maneira:</span><span class="sxs-lookup"><span data-stu-id="af4e8-120">If you have the server-relative URL for a **site** resource, you can construct a request as follows:</span></span>

```http
GET /sites/{hostname}:/{server-relative-path}
```

## <a name="access-a-group-team-site"></a><span data-ttu-id="af4e8-121">Acesse um site de equipe do grupo</span><span class="sxs-lookup"><span data-stu-id="af4e8-121">Access a group team site</span></span>

<span data-ttu-id="af4e8-122">Para acessar o site de equipe de um grupo:</span><span class="sxs-lookup"><span data-stu-id="af4e8-122">To access the team site for a group:</span></span>

```http
GET /groups/{group-id}/sites/root
```

## <a name="example"></a><span data-ttu-id="af4e8-123">Exemplo</span><span class="sxs-lookup"><span data-stu-id="af4e8-123">Example</span></span>

### <a name="request"></a><span data-ttu-id="af4e8-124">Solicitação</span><span class="sxs-lookup"><span data-stu-id="af4e8-124">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="af4e8-125">HTTP</span><span class="sxs-lookup"><span data-stu-id="af4e8-125">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-site" } -->

```http
GET /sites/{site-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="af4e8-126">C#</span><span class="sxs-lookup"><span data-stu-id="af4e8-126">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-site-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="af4e8-127">Javascript</span><span class="sxs-lookup"><span data-stu-id="af4e8-127">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-site-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="af4e8-128">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="af4e8-128">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-site-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="af4e8-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="af4e8-129">Response</span></span>

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
