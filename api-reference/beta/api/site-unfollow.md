---
author: learafa
title: Site da seguinte
description: Não acompanhar o site de um usuário
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: efb5862b38a5e8f0da651383aa935295dbc3dac1
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35271558"
---
# <a name="unfollow-site"></a><span data-ttu-id="37b31-103">Site da seguinte</span><span class="sxs-lookup"><span data-stu-id="37b31-103">Unfollow site</span></span> 

<span data-ttu-id="37b31-104">Não acompanhar o [site](../resources/site.md) de um usuário ou vários sites.</span><span class="sxs-lookup"><span data-stu-id="37b31-104">Unfollow a user's [site](../resources/site.md) or multiple sites.</span></span>

## <a name="permissions"></a><span data-ttu-id="37b31-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="37b31-105">Permissions</span></span>

<span data-ttu-id="37b31-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="37b31-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="37b31-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="37b31-108">Permission type</span></span>             | <span data-ttu-id="37b31-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="37b31-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="37b31-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="37b31-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="37b31-111">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37b31-111">Sites.ReadWrite.All</span></span>                         |
| <span data-ttu-id="37b31-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="37b31-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="37b31-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="37b31-113">Not supported.</span></span>                              |
| <span data-ttu-id="37b31-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="37b31-114">Application</span></span>                            | <span data-ttu-id="37b31-115">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37b31-115">Sites.ReadWrite.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="37b31-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="37b31-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /users/{user-id}/followedSites/remove
```

## <a name="request-body"></a><span data-ttu-id="37b31-117">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="37b31-117">Request body</span></span>

<span data-ttu-id="37b31-118">No corpo da solicitação, forneça uma matriz de objetos JSON com o parâmetro ID mencionado na tabela abaixo.</span><span class="sxs-lookup"><span data-stu-id="37b31-118">In the request body, supply an array of JSON objects with the id parameter mentioned in the table below.</span></span> 


| <span data-ttu-id="37b31-119">Nome</span><span class="sxs-lookup"><span data-stu-id="37b31-119">Name</span></span>                 | <span data-ttu-id="37b31-120">Valor</span><span class="sxs-lookup"><span data-stu-id="37b31-120">Value</span></span>  | <span data-ttu-id="37b31-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="37b31-121">Description</span></span>                                                            |
|:---------------------|:-------|:-----------------------------------------------------------------------|
|   <span data-ttu-id="37b31-122">id</span><span class="sxs-lookup"><span data-stu-id="37b31-122">id</span></span>                 | <span data-ttu-id="37b31-123">string</span><span class="sxs-lookup"><span data-stu-id="37b31-123">string</span></span> | <span data-ttu-id="37b31-124">O [identificador exclusivo](../resources/site.md#id-property) do item.</span><span class="sxs-lookup"><span data-stu-id="37b31-124">The [unique identifier](../resources/site.md#id-property) of the item.</span></span> |

## <a name="response"></a><span data-ttu-id="37b31-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="37b31-125">Response</span></span>

* <span data-ttu-id="37b31-126">Se a solicitação for bem-sucedida, este método retornará um `204` código de status sem conteúdo.</span><span class="sxs-lookup"><span data-stu-id="37b31-126">If the request is successful, this method returns a `204` status code with no content.</span></span>  
* <span data-ttu-id="37b31-127">Se ocorreu um erro durante a despróximação de qualquer um dos sites especificados, este `207` método retornará um código de status e o corpo da resposta conterá uma matriz de entradas contendo objetos [Error](/graph/errors) e siteIds indicando quais sites não podem ser seguidos.</span><span class="sxs-lookup"><span data-stu-id="37b31-127">If an error occured while unfollowing any of the specified sites, this method returns a `207` status code and the response body will contain an array of entries containing [error](/graph/errors) objects and siteIds indicating which sites unable to be unfollowed.</span></span>

## <a name="example"></a><span data-ttu-id="37b31-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="37b31-128">Example</span></span>

<span data-ttu-id="37b31-129">O exemplo a seguir mostra como desacompanhar vários sites.</span><span class="sxs-lookup"><span data-stu-id="37b31-129">The following example shows how to unfollow multiple sites.</span></span>

### <a name="request"></a><span data-ttu-id="37b31-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="37b31-130">Request</span></span>

<!-- { "blockType": "request", "name": "unfollow-site", "scopes": "sites.readwrite.all" } -->

```http
POST /users/{user-id}/followedSites/remove
Content-Type: application/json

{
    "value":
    [
        {
            "id": "contoso.sharepoint.com,da60e844-ba1d-49bc-b4d4-d5e36bae9019,712a596e-90a1-49e3-9b48-bfa80bee8740"
        },
        {
            "id": "contoso.sharepoint.com,da60e844-ba1d-49bc-b4d4-d5e36bae9019,0271110f-634f-4300-a841-3a8a2e851851"
        }
    ] 
}
```
### <a name="response"></a><span data-ttu-id="37b31-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="37b31-131">Response</span></span>

<span data-ttu-id="37b31-132">Se tiver êxito, retornará a seguinte resposta JSON.</span><span class="sxs-lookup"><span data-stu-id="37b31-132">If successful, it returns the following JSON response.</span></span> 

<!-- { "blockType": "response", "@type": "microsoft.graph.site", "isCollection": true, "truncated": true } -->

```json
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="37b31-133">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="37b31-133">SDK sample code</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="37b31-134">C#</span><span class="sxs-lookup"><span data-stu-id="37b31-134">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/unfollow-site-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="37b31-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="37b31-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/unfollow-site-Javascript-snippets.md)]
# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="37b31-136">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="37b31-136">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/unfollow-site-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="37b31-137">Se ocorreu um erro, ele retornará a seguinte resposta JSON</span><span class="sxs-lookup"><span data-stu-id="37b31-137">If an error occured, it returns the following JSON response</span></span> 

<!-- { "blockType": "response", "@type": "microsoft.graph.site", "isCollection": true, "truncated": true } -->

```json
HTTP/1.1 207 Multi-Status
Content-type: application/json

{
    "value": [
        {
            "id": "contoso.sharepoint.com,da60e844-ba1d-49bc-b4d4-d5e36bae9019,512a596e-90a1-49e3-9b48-bfa80bee8740",
            "error": {
                "@odata.type": "#oneDrive.error",
                "code": "invalidRequest",
                "message": "The site Id information that is provided in the request is incorrect",
                "innerError": {
                    "code": "invalidRequest",
                    "errorType": "expected",
                    "message": "The site Id information that is provided in the request is incorrect",
                    "stackTrace": "",
                    "throwSite": ""
                }
            }
        }
    ]
}
```  

<!-- {
  "type": "#page.annotation",
  "description": "Unfollow sharepoint site/sites for a user.",
  "keywords": "unfollow site",
  "section": "documentation",
  "tocPath": "Sites/Unfollow site",
  "suppressions": [
    "Error: /api-reference/beta/api/site-unfollow.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/site-unfollow.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/site-unfollow.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)"
  ]
} -->
