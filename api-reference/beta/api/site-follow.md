---
author: learafa
title: Siga o site
description: Siga o site/sites de um usuário.
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 8ba6766305970d3dc2cf040e8a274039a2f6da34
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35869697"
---
# <a name="follow-site"></a><span data-ttu-id="c9db8-103">Siga o site</span><span class="sxs-lookup"><span data-stu-id="c9db8-103">Follow site</span></span> 

<span data-ttu-id="c9db8-104">Siga o [site](../resources/site.md) de um usuário ou vários sites.</span><span class="sxs-lookup"><span data-stu-id="c9db8-104">Follow a user's [site](../resources/site.md) or multiple sites.</span></span>

## <a name="permissions"></a><span data-ttu-id="c9db8-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="c9db8-105">Permissions</span></span>

<span data-ttu-id="c9db8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c9db8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="c9db8-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c9db8-108">Permission type</span></span>             | <span data-ttu-id="c9db8-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c9db8-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="c9db8-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c9db8-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="c9db8-111">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9db8-111">Sites.ReadWrite.All</span></span>                         |
| <span data-ttu-id="c9db8-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c9db8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c9db8-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c9db8-113">Not supported.</span></span>                              |
| <span data-ttu-id="c9db8-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c9db8-114">Application</span></span>                            | <span data-ttu-id="c9db8-115">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9db8-115">Sites.ReadWrite.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="c9db8-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c9db8-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /users/{user-id}/followedSites/add
```

## <a name="request-body"></a><span data-ttu-id="c9db8-117">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c9db8-117">Request body</span></span>

<span data-ttu-id="c9db8-118">No corpo da solicitação, forneça uma matriz de objetos JSON com o parâmetro ID mencionado na tabela abaixo.</span><span class="sxs-lookup"><span data-stu-id="c9db8-118">In the request body, supply an array of JSON objects with the id parameter mentioned in the table below.</span></span> 


| <span data-ttu-id="c9db8-119">Nome</span><span class="sxs-lookup"><span data-stu-id="c9db8-119">Name</span></span>                 | <span data-ttu-id="c9db8-120">Valor</span><span class="sxs-lookup"><span data-stu-id="c9db8-120">Value</span></span>  | <span data-ttu-id="c9db8-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="c9db8-121">Description</span></span>                                                            |
|:---------------------|:-------|:-----------------------------------------------------------------------|
|   <span data-ttu-id="c9db8-122">id</span><span class="sxs-lookup"><span data-stu-id="c9db8-122">id</span></span>                 | <span data-ttu-id="c9db8-123">string</span><span class="sxs-lookup"><span data-stu-id="c9db8-123">string</span></span> | <span data-ttu-id="c9db8-124">O [identificador exclusivo](../resources/site.md#id-property) do item.</span><span class="sxs-lookup"><span data-stu-id="c9db8-124">The [unique identifier](../resources/site.md#id-property) of the item.</span></span> |


## <a name="response"></a><span data-ttu-id="c9db8-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="c9db8-125">Response</span></span> 

* <span data-ttu-id="c9db8-126">Se a solicitação for bem-sucedida, este método retornará uma matriz de sites que foram visitados.</span><span class="sxs-lookup"><span data-stu-id="c9db8-126">If the request is successful, this method returns an array of sites that were followed.</span></span>  
* <span data-ttu-id="c9db8-127">Se ocorreu um erro ao seguir qualquer um dos sites especificados, este método retornará um `207` código de status e o corpo da resposta conterá uma matriz de entradas contendo objetos [Error](/graph/errors) e siteIds indicando quais sites não puderam ser seguidos.</span><span class="sxs-lookup"><span data-stu-id="c9db8-127">If an error occured while following any of the specified sites, this method returns a `207` status code and the response body will contain an array of entries containing [error](/graph/errors) objects and siteIds indicating which sites were unable to be followed.</span></span>

## <a name="example"></a><span data-ttu-id="c9db8-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c9db8-128">Example</span></span>

<span data-ttu-id="c9db8-129">O exemplo a seguir mostra como seguir vários sites.</span><span class="sxs-lookup"><span data-stu-id="c9db8-129">The following example shows how to follow multiple sites.</span></span> 

### <a name="request"></a><span data-ttu-id="c9db8-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c9db8-130">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="c9db8-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="c9db8-131">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="c9db8-132">C#</span><span class="sxs-lookup"><span data-stu-id="c9db8-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/follow-site-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c9db8-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="c9db8-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/follow-site-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c9db8-134">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="c9db8-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/follow-site-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c9db8-135">Java</span><span class="sxs-lookup"><span data-stu-id="c9db8-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/follow-site-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="c9db8-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="c9db8-136">Response</span></span>

<span data-ttu-id="c9db8-137">Se tiver êxito, retornará a seguinte resposta JSON.</span><span class="sxs-lookup"><span data-stu-id="c9db8-137">If successful, it returns the following JSON response.</span></span> 

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

<span data-ttu-id="c9db8-138">Se ocorreu um erro, ele retornará a seguinte resposta JSON</span><span class="sxs-lookup"><span data-stu-id="c9db8-138">If an error occured, it returns the following JSON response</span></span> 

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
  ]
} -->
