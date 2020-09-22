---
author: learafa
title: Seguir site
description: Siga o site/sites de um usuário.
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 218efae00703e452df1f9a8fd4f0ad73727b4c10
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48014011"
---
# <a name="follow-site"></a><span data-ttu-id="51aec-103">Seguir site</span><span class="sxs-lookup"><span data-stu-id="51aec-103">Follow site</span></span> 

<span data-ttu-id="51aec-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="51aec-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="51aec-105">Siga o [site](../resources/site.md) de um usuário ou vários sites.</span><span class="sxs-lookup"><span data-stu-id="51aec-105">Follow a user's [site](../resources/site.md) or multiple sites.</span></span>

## <a name="permissions"></a><span data-ttu-id="51aec-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="51aec-106">Permissions</span></span>

<span data-ttu-id="51aec-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="51aec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="51aec-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="51aec-109">Permission type</span></span>             | <span data-ttu-id="51aec-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="51aec-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="51aec-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="51aec-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="51aec-112">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51aec-112">Sites.ReadWrite.All</span></span>                         |
| <span data-ttu-id="51aec-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="51aec-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="51aec-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="51aec-114">Not supported.</span></span>                              |
| <span data-ttu-id="51aec-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="51aec-115">Application</span></span>                            | <span data-ttu-id="51aec-116">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51aec-116">Sites.ReadWrite.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="51aec-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="51aec-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /users/{user-id}/followedSites/add
```

## <a name="request-body"></a><span data-ttu-id="51aec-118">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="51aec-118">Request body</span></span>

<span data-ttu-id="51aec-119">No corpo da solicitação, forneça uma matriz de objetos JSON com o parâmetro ID mencionado na tabela abaixo.</span><span class="sxs-lookup"><span data-stu-id="51aec-119">In the request body, supply an array of JSON objects with the id parameter mentioned in the table below.</span></span> 


| <span data-ttu-id="51aec-120">Nome</span><span class="sxs-lookup"><span data-stu-id="51aec-120">Name</span></span>                 | <span data-ttu-id="51aec-121">Valor</span><span class="sxs-lookup"><span data-stu-id="51aec-121">Value</span></span>  | <span data-ttu-id="51aec-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="51aec-122">Description</span></span>                                                            |
|:---------------------|:-------|:-----------------------------------------------------------------------|
|   <span data-ttu-id="51aec-123">id</span><span class="sxs-lookup"><span data-stu-id="51aec-123">id</span></span>                 | <span data-ttu-id="51aec-124">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="51aec-124">string</span></span> | <span data-ttu-id="51aec-125">O [identificador exclusivo](../resources/site.md#id-property) do item.</span><span class="sxs-lookup"><span data-stu-id="51aec-125">The [unique identifier](../resources/site.md#id-property) of the item.</span></span> |


## <a name="response"></a><span data-ttu-id="51aec-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="51aec-126">Response</span></span> 

* <span data-ttu-id="51aec-127">Se a solicitação for bem-sucedida, este método retornará uma matriz de sites que foram visitados.</span><span class="sxs-lookup"><span data-stu-id="51aec-127">If the request is successful, this method returns an array of sites that were followed.</span></span>  
* <span data-ttu-id="51aec-128">Se ocorreu um erro ao seguir qualquer um dos sites especificados, este método retornará um `207` código de status e o corpo da resposta conterá uma matriz de entradas contendo objetos [Error](/graph/errors) e siteIds indicando quais sites não puderam ser seguidos.</span><span class="sxs-lookup"><span data-stu-id="51aec-128">If an error occurred while following any of the specified sites, this method returns a `207` status code and the response body will contain an array of entries containing [error](/graph/errors) objects and siteIds indicating which sites were unable to be followed.</span></span>

## <a name="example"></a><span data-ttu-id="51aec-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="51aec-129">Example</span></span>

<span data-ttu-id="51aec-130">O exemplo a seguir mostra como seguir vários sites.</span><span class="sxs-lookup"><span data-stu-id="51aec-130">The following example shows how to follow multiple sites.</span></span> 

### <a name="request"></a><span data-ttu-id="51aec-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="51aec-131">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="51aec-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="51aec-132">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="51aec-133">C#</span><span class="sxs-lookup"><span data-stu-id="51aec-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/follow-site-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="51aec-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="51aec-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/follow-site-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="51aec-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="51aec-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/follow-site-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="51aec-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="51aec-136">Response</span></span>

<span data-ttu-id="51aec-137">Se tiver êxito, retornará a seguinte resposta JSON.</span><span class="sxs-lookup"><span data-stu-id="51aec-137">If successful, it returns the following JSON response.</span></span> 

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

<span data-ttu-id="51aec-138">Se ocorreu um erro, ele retornará a seguinte resposta JSON</span><span class="sxs-lookup"><span data-stu-id="51aec-138">If an error occured, it returns the following JSON response</span></span> 

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


