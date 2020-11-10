---
author: learafa
title: Deixar de seguir site
description: Não acompanhar o site de um usuário
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 167a45619edf0f867a3a83835a8a194027bab3c8
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48973219"
---
# <a name="unfollow-site"></a><span data-ttu-id="fd013-103">Deixar de seguir site</span><span class="sxs-lookup"><span data-stu-id="fd013-103">Unfollow site</span></span> 

<span data-ttu-id="fd013-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fd013-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fd013-105">Não acompanhar o [site](../resources/site.md) de um usuário ou vários sites.</span><span class="sxs-lookup"><span data-stu-id="fd013-105">Unfollow a user's [site](../resources/site.md) or multiple sites.</span></span>

## <a name="permissions"></a><span data-ttu-id="fd013-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="fd013-106">Permissions</span></span>

<span data-ttu-id="fd013-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fd013-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="fd013-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fd013-109">Permission type</span></span>             | <span data-ttu-id="fd013-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fd013-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="fd013-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fd013-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="fd013-112">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fd013-112">Sites.ReadWrite.All</span></span>                         |
| <span data-ttu-id="fd013-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fd013-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fd013-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fd013-114">Not supported.</span></span>                              |
| <span data-ttu-id="fd013-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fd013-115">Application</span></span>                            | <span data-ttu-id="fd013-116">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fd013-116">Sites.ReadWrite.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="fd013-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fd013-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /users/{user-id}/followedSites/remove
```

## <a name="request-body"></a><span data-ttu-id="fd013-118">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fd013-118">Request body</span></span>

<span data-ttu-id="fd013-119">No corpo da solicitação, forneça uma matriz de objetos JSON com o parâmetro ID mencionado na tabela abaixo.</span><span class="sxs-lookup"><span data-stu-id="fd013-119">In the request body, supply an array of JSON objects with the id parameter mentioned in the table below.</span></span> 


| <span data-ttu-id="fd013-120">Nome</span><span class="sxs-lookup"><span data-stu-id="fd013-120">Name</span></span>                 | <span data-ttu-id="fd013-121">Valor</span><span class="sxs-lookup"><span data-stu-id="fd013-121">Value</span></span>  | <span data-ttu-id="fd013-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="fd013-122">Description</span></span>                                                            |
|:---------------------|:-------|:-----------------------------------------------------------------------|
|   <span data-ttu-id="fd013-123">id</span><span class="sxs-lookup"><span data-stu-id="fd013-123">id</span></span>                 | <span data-ttu-id="fd013-124">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fd013-124">string</span></span> | <span data-ttu-id="fd013-125">O [identificador exclusivo](../resources/site.md#id-property) do item.</span><span class="sxs-lookup"><span data-stu-id="fd013-125">The [unique identifier](../resources/site.md#id-property) of the item.</span></span> |

## <a name="response"></a><span data-ttu-id="fd013-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="fd013-126">Response</span></span>

* <span data-ttu-id="fd013-127">Se a solicitação for bem-sucedida, este método retornará um `204` código de status sem conteúdo.</span><span class="sxs-lookup"><span data-stu-id="fd013-127">If the request is successful, this method returns a `204` status code with no content.</span></span>  
* <span data-ttu-id="fd013-128">Se ocorreu um erro durante a despróximação de qualquer um dos sites especificados, este método retornará um `207` código de status e o corpo da resposta conterá uma matriz de entradas contendo objetos [Error](/graph/errors) e siteIds indicando quais sites não podem ser seguidos.</span><span class="sxs-lookup"><span data-stu-id="fd013-128">If an error occured while unfollowing any of the specified sites, this method returns a `207` status code and the response body will contain an array of entries containing [error](/graph/errors) objects and siteIds indicating which sites unable to be unfollowed.</span></span>

## <a name="example"></a><span data-ttu-id="fd013-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fd013-129">Example</span></span>

<span data-ttu-id="fd013-130">O exemplo a seguir mostra como desacompanhar vários sites.</span><span class="sxs-lookup"><span data-stu-id="fd013-130">The following example shows how to unfollow multiple sites.</span></span>

### <a name="request"></a><span data-ttu-id="fd013-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fd013-131">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="fd013-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="fd013-132">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="fd013-133">C#</span><span class="sxs-lookup"><span data-stu-id="fd013-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/unfollow-site-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fd013-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fd013-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/unfollow-site-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fd013-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fd013-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/unfollow-site-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fd013-136">Java</span><span class="sxs-lookup"><span data-stu-id="fd013-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/unfollow-site-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="fd013-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="fd013-137">Response</span></span>

<span data-ttu-id="fd013-138">Se tiver êxito, retornará a seguinte resposta JSON.</span><span class="sxs-lookup"><span data-stu-id="fd013-138">If successful, it returns the following JSON response.</span></span> 

<!-- { "blockType": "response", "@type": "microsoft.graph.site", "isCollection": true, "truncated": true } -->

```json
HTTP/1.1 204 No Content
```

<span data-ttu-id="fd013-139">Se ocorreu um erro, ele retornará a seguinte resposta JSON</span><span class="sxs-lookup"><span data-stu-id="fd013-139">If an error occured, it returns the following JSON response</span></span> 

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


