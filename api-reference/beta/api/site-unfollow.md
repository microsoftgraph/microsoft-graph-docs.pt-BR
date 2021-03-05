---
author: learafa
title: Deixar de seguir site
description: Desa seguir o site de um usuário
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 6d938fc0c02cfc876449edd5bf656770df9190c4
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50475749"
---
# <a name="unfollow-site"></a><span data-ttu-id="2a2bc-103">Deixar de seguir site</span><span class="sxs-lookup"><span data-stu-id="2a2bc-103">Unfollow site</span></span> 

<span data-ttu-id="2a2bc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2a2bc-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2a2bc-105">Desa siga o site de um [usuário ou](../resources/site.md) vários sites.</span><span class="sxs-lookup"><span data-stu-id="2a2bc-105">Unfollow a user's [site](../resources/site.md) or multiple sites.</span></span>

## <a name="permissions"></a><span data-ttu-id="2a2bc-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="2a2bc-106">Permissions</span></span>

<span data-ttu-id="2a2bc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2a2bc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="2a2bc-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2a2bc-109">Permission type</span></span>             | <span data-ttu-id="2a2bc-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2a2bc-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="2a2bc-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2a2bc-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="2a2bc-112">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a2bc-112">Sites.ReadWrite.All</span></span>                         |
| <span data-ttu-id="2a2bc-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2a2bc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2a2bc-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2a2bc-114">Not supported.</span></span>                              |
| <span data-ttu-id="2a2bc-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2a2bc-115">Application</span></span>                            | <span data-ttu-id="2a2bc-116">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a2bc-116">Sites.ReadWrite.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="2a2bc-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2a2bc-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /users/{user-id}/followedSites/remove
```

## <a name="request-body"></a><span data-ttu-id="2a2bc-118">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2a2bc-118">Request body</span></span>

<span data-ttu-id="2a2bc-119">No corpo da solicitação, fornece uma matriz de objetos JSON com o parâmetro id mencionado na tabela abaixo.</span><span class="sxs-lookup"><span data-stu-id="2a2bc-119">In the request body, supply an array of JSON objects with the id parameter mentioned in the table below.</span></span> 


| <span data-ttu-id="2a2bc-120">Nome</span><span class="sxs-lookup"><span data-stu-id="2a2bc-120">Name</span></span>                 | <span data-ttu-id="2a2bc-121">Valor</span><span class="sxs-lookup"><span data-stu-id="2a2bc-121">Value</span></span>  | <span data-ttu-id="2a2bc-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="2a2bc-122">Description</span></span>                                                            |
|:---------------------|:-------|:-----------------------------------------------------------------------|
|   <span data-ttu-id="2a2bc-123">id</span><span class="sxs-lookup"><span data-stu-id="2a2bc-123">id</span></span>                 | <span data-ttu-id="2a2bc-124">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2a2bc-124">string</span></span> | <span data-ttu-id="2a2bc-125">O [identificador exclusivo](../resources/site.md#id-property) do item.</span><span class="sxs-lookup"><span data-stu-id="2a2bc-125">The [unique identifier](../resources/site.md#id-property) of the item.</span></span> |

## <a name="response"></a><span data-ttu-id="2a2bc-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="2a2bc-126">Response</span></span>

* <span data-ttu-id="2a2bc-127">Se a solicitação for bem-sucedida, este método retornará um `204` código de status sem conteúdo.</span><span class="sxs-lookup"><span data-stu-id="2a2bc-127">If the request is successful, this method returns a `204` status code with no content.</span></span>  
* <span data-ttu-id="2a2bc-128">Se ocorreu um erro ao não seguir nenhum dos sites especificados, este método retornará um código de status e o corpo da resposta conterá uma matriz de entradas contendo objetos de erro e siteIds indicando quais sites não podem ser `207` seguidos. [](/graph/errors)</span><span class="sxs-lookup"><span data-stu-id="2a2bc-128">If an error occured while unfollowing any of the specified sites, this method returns a `207` status code and the response body will contain an array of entries containing [error](/graph/errors) objects and siteIds indicating which sites unable to be unfollowed.</span></span>

## <a name="example"></a><span data-ttu-id="2a2bc-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2a2bc-129">Example</span></span>

<span data-ttu-id="2a2bc-130">O exemplo a seguir mostra como desa seguir vários sites.</span><span class="sxs-lookup"><span data-stu-id="2a2bc-130">The following example shows how to unfollow multiple sites.</span></span>

### <a name="request"></a><span data-ttu-id="2a2bc-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2a2bc-131">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="2a2bc-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="2a2bc-132">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="2a2bc-133">C#</span><span class="sxs-lookup"><span data-stu-id="2a2bc-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/unfollow-site-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2a2bc-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2a2bc-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/unfollow-site-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2a2bc-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2a2bc-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/unfollow-site-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2a2bc-136">Java</span><span class="sxs-lookup"><span data-stu-id="2a2bc-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/unfollow-site-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="2a2bc-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="2a2bc-137">Response</span></span>

<span data-ttu-id="2a2bc-138">Se tiver êxito, retornará a seguinte resposta JSON.</span><span class="sxs-lookup"><span data-stu-id="2a2bc-138">If successful, it returns the following JSON response.</span></span> 

<!-- { "blockType": "response", "@type": "microsoft.graph.site", "isCollection": true, "truncated": true } -->

```http
HTTP/1.1 204 No Content
```

<span data-ttu-id="2a2bc-139">Se ocorrer um erro, ele retornará a seguinte resposta JSON</span><span class="sxs-lookup"><span data-stu-id="2a2bc-139">If an error occured, it returns the following JSON response</span></span> 

<!-- { "blockType": "response", "@type": "microsoft.graph.site", "isCollection": true, "truncated": true } -->

```http
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


