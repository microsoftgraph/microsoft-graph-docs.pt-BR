---
author: learafa
title: Seguir site
description: Siga o site/sites de um usuário.
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 1f643671f9d9ccb744974f278007ce26186b2c97
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50473711"
---
# <a name="follow-site"></a><span data-ttu-id="6a9cc-103">Seguir site</span><span class="sxs-lookup"><span data-stu-id="6a9cc-103">Follow site</span></span> 

<span data-ttu-id="6a9cc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6a9cc-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6a9cc-105">Siga o site de um [usuário ou](../resources/site.md) vários sites.</span><span class="sxs-lookup"><span data-stu-id="6a9cc-105">Follow a user's [site](../resources/site.md) or multiple sites.</span></span>

## <a name="permissions"></a><span data-ttu-id="6a9cc-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="6a9cc-106">Permissions</span></span>

<span data-ttu-id="6a9cc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6a9cc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="6a9cc-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6a9cc-109">Permission type</span></span>             | <span data-ttu-id="6a9cc-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6a9cc-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="6a9cc-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6a9cc-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6a9cc-112">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a9cc-112">Sites.ReadWrite.All</span></span>                         |
| <span data-ttu-id="6a9cc-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6a9cc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6a9cc-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6a9cc-114">Not supported.</span></span>                              |
| <span data-ttu-id="6a9cc-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6a9cc-115">Application</span></span>                            | <span data-ttu-id="6a9cc-116">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a9cc-116">Sites.ReadWrite.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="6a9cc-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6a9cc-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /users/{user-id}/followedSites/add
```

## <a name="request-body"></a><span data-ttu-id="6a9cc-118">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6a9cc-118">Request body</span></span>

<span data-ttu-id="6a9cc-119">No corpo da solicitação, fornece uma matriz de objetos JSON com o parâmetro id mencionado na tabela abaixo.</span><span class="sxs-lookup"><span data-stu-id="6a9cc-119">In the request body, supply an array of JSON objects with the id parameter mentioned in the table below.</span></span> 


| <span data-ttu-id="6a9cc-120">Nome</span><span class="sxs-lookup"><span data-stu-id="6a9cc-120">Name</span></span>                 | <span data-ttu-id="6a9cc-121">Valor</span><span class="sxs-lookup"><span data-stu-id="6a9cc-121">Value</span></span>  | <span data-ttu-id="6a9cc-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="6a9cc-122">Description</span></span>                                                            |
|:---------------------|:-------|:-----------------------------------------------------------------------|
|   <span data-ttu-id="6a9cc-123">id</span><span class="sxs-lookup"><span data-stu-id="6a9cc-123">id</span></span>                 | <span data-ttu-id="6a9cc-124">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6a9cc-124">string</span></span> | <span data-ttu-id="6a9cc-125">O [identificador exclusivo](../resources/site.md#id-property) do item.</span><span class="sxs-lookup"><span data-stu-id="6a9cc-125">The [unique identifier](../resources/site.md#id-property) of the item.</span></span> |


## <a name="response"></a><span data-ttu-id="6a9cc-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="6a9cc-126">Response</span></span> 

* <span data-ttu-id="6a9cc-127">Se a solicitação for bem-sucedida, este método retornará uma matriz de sites que foram seguidos.</span><span class="sxs-lookup"><span data-stu-id="6a9cc-127">If the request is successful, this method returns an array of sites that were followed.</span></span>  
* <span data-ttu-id="6a9cc-128">Se ocorrer um erro ao seguir qualquer um dos sites especificados, este método retornará um código de status e o corpo da resposta conterá uma matriz de entradas contendo objetos de erro e siteIds indicando quais sites não puderam ser `207` seguidos. [](/graph/errors)</span><span class="sxs-lookup"><span data-stu-id="6a9cc-128">If an error occurred while following any of the specified sites, this method returns a `207` status code and the response body will contain an array of entries containing [error](/graph/errors) objects and siteIds indicating which sites were unable to be followed.</span></span>

## <a name="example"></a><span data-ttu-id="6a9cc-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6a9cc-129">Example</span></span>

<span data-ttu-id="6a9cc-130">O exemplo a seguir mostra como seguir vários sites.</span><span class="sxs-lookup"><span data-stu-id="6a9cc-130">The following example shows how to follow multiple sites.</span></span> 

### <a name="request"></a><span data-ttu-id="6a9cc-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6a9cc-131">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="6a9cc-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="6a9cc-132">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="6a9cc-133">C#</span><span class="sxs-lookup"><span data-stu-id="6a9cc-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/follow-site-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6a9cc-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6a9cc-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/follow-site-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6a9cc-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6a9cc-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/follow-site-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6a9cc-136">Java</span><span class="sxs-lookup"><span data-stu-id="6a9cc-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/follow-site-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="6a9cc-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="6a9cc-137">Response</span></span>

<span data-ttu-id="6a9cc-138">Se tiver êxito, retornará a seguinte resposta JSON.</span><span class="sxs-lookup"><span data-stu-id="6a9cc-138">If successful, it returns the following JSON response.</span></span> 

<!-- { "blockType": "response", "@type": "microsoft.graph.site", "isCollection": true, "truncated": true } -->

```http
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

<span data-ttu-id="6a9cc-139">Se ocorrer um erro, ele retornará a seguinte resposta JSON</span><span class="sxs-lookup"><span data-stu-id="6a9cc-139">If an error occured, it returns the following JSON response</span></span> 

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

