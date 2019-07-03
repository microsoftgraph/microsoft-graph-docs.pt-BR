---
author: learafa
title: Site da seguinte
description: Não acompanhar o site de um usuário
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 1233def7ebec0f5702deb00f6f986e317835c6ca
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35457125"
---
# <a name="unfollow-site"></a><span data-ttu-id="ff42c-103">Site da seguinte</span><span class="sxs-lookup"><span data-stu-id="ff42c-103">Unfollow site</span></span> 

<span data-ttu-id="ff42c-104">Não acompanhar o [site](../resources/site.md) de um usuário ou vários sites.</span><span class="sxs-lookup"><span data-stu-id="ff42c-104">Unfollow a user's [site](../resources/site.md) or multiple sites.</span></span>

## <a name="permissions"></a><span data-ttu-id="ff42c-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="ff42c-105">Permissions</span></span>

<span data-ttu-id="ff42c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ff42c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="ff42c-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ff42c-108">Permission type</span></span>             | <span data-ttu-id="ff42c-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ff42c-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="ff42c-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ff42c-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="ff42c-111">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff42c-111">Sites.ReadWrite.All</span></span>                         |
| <span data-ttu-id="ff42c-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ff42c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ff42c-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ff42c-113">Not supported.</span></span>                              |
| <span data-ttu-id="ff42c-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ff42c-114">Application</span></span>                            | <span data-ttu-id="ff42c-115">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff42c-115">Sites.ReadWrite.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="ff42c-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ff42c-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /users/{user-id}/followedSites/remove
```

## <a name="request-body"></a><span data-ttu-id="ff42c-117">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ff42c-117">Request body</span></span>

<span data-ttu-id="ff42c-118">No corpo da solicitação, forneça uma matriz de objetos JSON com o parâmetro ID mencionado na tabela abaixo.</span><span class="sxs-lookup"><span data-stu-id="ff42c-118">In the request body, supply an array of JSON objects with the id parameter mentioned in the table below.</span></span> 


| <span data-ttu-id="ff42c-119">Nome</span><span class="sxs-lookup"><span data-stu-id="ff42c-119">Name</span></span>                 | <span data-ttu-id="ff42c-120">Valor</span><span class="sxs-lookup"><span data-stu-id="ff42c-120">Value</span></span>  | <span data-ttu-id="ff42c-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="ff42c-121">Description</span></span>                                                            |
|:---------------------|:-------|:-----------------------------------------------------------------------|
|   <span data-ttu-id="ff42c-122">id</span><span class="sxs-lookup"><span data-stu-id="ff42c-122">id</span></span>                 | <span data-ttu-id="ff42c-123">string</span><span class="sxs-lookup"><span data-stu-id="ff42c-123">string</span></span> | <span data-ttu-id="ff42c-124">O [identificador exclusivo](../resources/site.md#id-property) do item.</span><span class="sxs-lookup"><span data-stu-id="ff42c-124">The [unique identifier](../resources/site.md#id-property) of the item.</span></span> |

## <a name="response"></a><span data-ttu-id="ff42c-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="ff42c-125">Response</span></span>

* <span data-ttu-id="ff42c-126">Se a solicitação for bem-sucedida, este método retornará um `204` código de status sem conteúdo.</span><span class="sxs-lookup"><span data-stu-id="ff42c-126">If the request is successful, this method returns a `204` status code with no content.</span></span>  
* <span data-ttu-id="ff42c-127">Se ocorreu um erro durante a despróximação de qualquer um dos sites especificados, este `207` método retornará um código de status e o corpo da resposta conterá uma matriz de entradas contendo objetos [Error](/graph/errors) e siteIds indicando quais sites não podem ser seguidos.</span><span class="sxs-lookup"><span data-stu-id="ff42c-127">If an error occured while unfollowing any of the specified sites, this method returns a `207` status code and the response body will contain an array of entries containing [error](/graph/errors) objects and siteIds indicating which sites unable to be unfollowed.</span></span>

## <a name="example"></a><span data-ttu-id="ff42c-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ff42c-128">Example</span></span>

<span data-ttu-id="ff42c-129">O exemplo a seguir mostra como desacompanhar vários sites.</span><span class="sxs-lookup"><span data-stu-id="ff42c-129">The following example shows how to unfollow multiple sites.</span></span>

### <a name="request"></a><span data-ttu-id="ff42c-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ff42c-130">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="ff42c-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="ff42c-131">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="ff42c-132">C#</span><span class="sxs-lookup"><span data-stu-id="ff42c-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/unfollow-site-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ff42c-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="ff42c-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/unfollow-site-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ff42c-134">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="ff42c-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/unfollow-site-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="ff42c-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="ff42c-135">Response</span></span>

<span data-ttu-id="ff42c-136">Se tiver êxito, retornará a seguinte resposta JSON.</span><span class="sxs-lookup"><span data-stu-id="ff42c-136">If successful, it returns the following JSON response.</span></span> 

<!-- { "blockType": "response", "@type": "microsoft.graph.site", "isCollection": true, "truncated": true } -->

```json
HTTP/1.1 204 No Content
```

<span data-ttu-id="ff42c-137">Se ocorreu um erro, ele retornará a seguinte resposta JSON</span><span class="sxs-lookup"><span data-stu-id="ff42c-137">If an error occured, it returns the following JSON response</span></span> 

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
  ]
} -->
