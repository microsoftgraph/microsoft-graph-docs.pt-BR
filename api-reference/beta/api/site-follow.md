---
author: learafa
title: Siga o site
description: Siga o site/sites de um usuário.
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 91b331787a1c8e54856b8ac62818eef2581c29e6
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35271586"
---
# <a name="follow-site"></a><span data-ttu-id="c7929-103">Siga o site</span><span class="sxs-lookup"><span data-stu-id="c7929-103">Follow site</span></span> 

<span data-ttu-id="c7929-104">Siga o [site](../resources/site.md) de um usuário ou vários sites.</span><span class="sxs-lookup"><span data-stu-id="c7929-104">Follow a user's [site](../resources/site.md) or multiple sites.</span></span>

## <a name="permissions"></a><span data-ttu-id="c7929-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="c7929-105">Permissions</span></span>

<span data-ttu-id="c7929-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c7929-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="c7929-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c7929-108">Permission type</span></span>             | <span data-ttu-id="c7929-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c7929-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="c7929-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c7929-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="c7929-111">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7929-111">Sites.ReadWrite.All</span></span>                         |
| <span data-ttu-id="c7929-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c7929-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c7929-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c7929-113">Not supported.</span></span>                              |
| <span data-ttu-id="c7929-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c7929-114">Application</span></span>                            | <span data-ttu-id="c7929-115">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7929-115">Sites.ReadWrite.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="c7929-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c7929-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /users/{user-id}/followedSites/add
```

## <a name="request-body"></a><span data-ttu-id="c7929-117">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c7929-117">Request body</span></span>

<span data-ttu-id="c7929-118">No corpo da solicitação, forneça uma matriz de objetos JSON com o parâmetro ID mencionado na tabela abaixo.</span><span class="sxs-lookup"><span data-stu-id="c7929-118">In the request body, supply an array of JSON objects with the id parameter mentioned in the table below.</span></span> 


| <span data-ttu-id="c7929-119">Nome</span><span class="sxs-lookup"><span data-stu-id="c7929-119">Name</span></span>                 | <span data-ttu-id="c7929-120">Valor</span><span class="sxs-lookup"><span data-stu-id="c7929-120">Value</span></span>  | <span data-ttu-id="c7929-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="c7929-121">Description</span></span>                                                            |
|:---------------------|:-------|:-----------------------------------------------------------------------|
|   <span data-ttu-id="c7929-122">id</span><span class="sxs-lookup"><span data-stu-id="c7929-122">id</span></span>                 | <span data-ttu-id="c7929-123">string</span><span class="sxs-lookup"><span data-stu-id="c7929-123">string</span></span> | <span data-ttu-id="c7929-124">O [identificador exclusivo](../resources/site.md#id-property) do item.</span><span class="sxs-lookup"><span data-stu-id="c7929-124">The [unique identifier](../resources/site.md#id-property) of the item.</span></span> |


## <a name="response"></a><span data-ttu-id="c7929-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="c7929-125">Response</span></span> 

* <span data-ttu-id="c7929-126">Se a solicitação for bem-sucedida, este método retornará uma matriz de sites que foram visitados.</span><span class="sxs-lookup"><span data-stu-id="c7929-126">If the request is successful, this method returns an array of sites that were followed.</span></span>  
* <span data-ttu-id="c7929-127">Se ocorreu um erro ao seguir qualquer um dos sites especificados, este método retornará um `207` código de status e o corpo da resposta conterá uma matriz de entradas contendo objetos [Error](/graph/errors) e siteIds indicando quais sites não puderam ser seguidos.</span><span class="sxs-lookup"><span data-stu-id="c7929-127">If an error occured while following any of the specified sites, this method returns a `207` status code and the response body will contain an array of entries containing [error](/graph/errors) objects and siteIds indicating which sites were unable to be followed.</span></span>

## <a name="example"></a><span data-ttu-id="c7929-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c7929-128">Example</span></span>

<span data-ttu-id="c7929-129">O exemplo a seguir mostra como seguir vários sites.</span><span class="sxs-lookup"><span data-stu-id="c7929-129">The following example shows how to follow multiple sites.</span></span> 

### <a name="request"></a><span data-ttu-id="c7929-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c7929-130">Request</span></span>

<!-- { "blockType": "request", "name": "follow-site", "scopes": "sites.readwrite.all" } -->

```http
POST /users/{user-id}/followedSites/add
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
### <a name="response"></a><span data-ttu-id="c7929-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="c7929-131">Response</span></span>

<span data-ttu-id="c7929-132">Se tiver êxito, retornará a seguinte resposta JSON.</span><span class="sxs-lookup"><span data-stu-id="c7929-132">If successful, it returns the following JSON response.</span></span> 

<!-- { "blockType": "response", "@type": "microsoft.graph.site", "isCollection": true, "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "id": "contoso.sharepoint.com,da60e844-ba1d-49bc-b4d4-d5e36bae9019,712a596e-90a1-49e3-9b48-bfa80bee8740",
            "webUrl": "http://contoso.sharepoint.com/sites/SiteFollowed1",
            "name": "SiteFollowed1",
            "sharepointIds": {
                "siteId": "da60e844-ba1d-49bc-b4d4-d5e36bae9019",
                "siteUrl": "http://contoso.sharepoint.com/sites/SiteFollowed1",
                "webId": "712a596e-90a1-49e3-9b48-bfa80bee8740"
            },
            "siteCollection": {
                "hostname": "contoso.sharepoint.com"
            }
        },
        {
            "id": "contoso.sharepoint.com,da60e844-ba1d-49bc-b4d4-d5e36bae9019,0271110f-634f-4300-a841-3a8a2e851851",
            "webUrl": "http://contoso.sharepoint.com/sites/SiteFollowed2",
            "name": "SiteFollowed2",
            "sharepointIds": {
                "siteId": "da60e844-ba1d-49bc-b4d4-d5e36bae9019",
                "siteUrl": "http://contoso.sharepoint.com/sites/SiteFollowed2",
                "webId": "0271110f-634f-4300-a841-3a8a2e851851"
            },
            "siteCollection": {
                "hostname": "contoso.sharepoint.com"
            }
        }
    ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="c7929-133">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="c7929-133">SDK sample code</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="c7929-134">C#</span><span class="sxs-lookup"><span data-stu-id="c7929-134">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/follow-site-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c7929-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="c7929-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/follow-site-Javascript-snippets.md)]
# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="c7929-136">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="c7929-136">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/follow-site-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="c7929-137">Se ocorreu um erro, ele retornará a seguinte resposta JSON</span><span class="sxs-lookup"><span data-stu-id="c7929-137">If an error occured, it returns the following JSON response</span></span> 

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
        },
        {
            "id": "contoso.sharepoint.com,da60e844-ba1d-49bc-b4d4-d5e36bae9019,0271110f-634f-4300-a841-3a8a2e851851",
            "webUrl": "http://contoso.sharepoint.com/sites/SiteFollowed2",
            "name": "SiteFollowed2",
            "sharepointIds": {
                "siteId": "da60e844-ba1d-49bc-b4d4-d5e36bae9019",
                "siteUrl": "http://contoso.sharepoint.com/sites/SiteFollowed2",
                "webId": "0271110f-634f-4300-a841-3a8a2e851851"
            },
            "siteCollection": {
                "hostname": "contoso.sharepoint.com"
            }
        }
    ]
}
```  

<!-- {
  "type": "#page.annotation",
  "description": "Follow sharepoint site for a user.",
  "keywords": "follow site",
  "section": "documentation",
  "tocPath": "Sites/Follow site",
  "suppressions": [
    "Error: /api-reference/beta/api/site-follow.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/site-follow.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/site-follow.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)"
  ]
} -->
