---
author: learafa
description: Liste os sites que foram seguidos pelo usuário conectado.
title: Listar sites seguidos
localization_priority: Normal
ms.prod: SharePoint
doc_type: apiPageType
ms.openlocfilehash: c08def6b72869cdc1886a71d1083dfdef51dbebd
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2020
ms.locfileid: "44052313"
---
# <a name="list-followed-sites"></a><span data-ttu-id="170ef-103">Listar sites seguidos</span><span class="sxs-lookup"><span data-stu-id="170ef-103">List followed sites</span></span>

<span data-ttu-id="170ef-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="170ef-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="170ef-105">Listar os [sites](../resources/site.md) que foram seguidos pelo usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="170ef-105">List the [sites](../resources/site.md) that have been followed by the signed in user.</span></span>

## <a name="permissions"></a><span data-ttu-id="170ef-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="170ef-106">Permissions</span></span>

<span data-ttu-id="170ef-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="170ef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="170ef-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="170ef-109">Permission type</span></span>      | <span data-ttu-id="170ef-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="170ef-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="170ef-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="170ef-111">Delegated (work or school account)</span></span> | <span data-ttu-id="170ef-112">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="170ef-112">Sites.Read.All, Sites.ReadWrite.All</span></span>  |
|<span data-ttu-id="170ef-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="170ef-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="170ef-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="170ef-114">Not supported.</span></span>    |
|<span data-ttu-id="170ef-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="170ef-115">Application</span></span> | <span data-ttu-id="170ef-116">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="170ef-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="170ef-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="170ef-117">HTTP request</span></span>

<span data-ttu-id="170ef-118">Este método é acessível apenas por meio do OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="170ef-118">This method is accessible only through OneDrive for Business.</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/followedSites
```

## <a name="optional-query-parameters"></a><span data-ttu-id="170ef-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="170ef-119">Optional query parameters</span></span>
<span data-ttu-id="170ef-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="170ef-120">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="170ef-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="170ef-121">Request headers</span></span>

| <span data-ttu-id="170ef-122">Nome</span><span class="sxs-lookup"><span data-stu-id="170ef-122">Name</span></span>      |<span data-ttu-id="170ef-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="170ef-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="170ef-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="170ef-124">Authorization</span></span>  | <span data-ttu-id="170ef-125">Portador {código}.</span><span class="sxs-lookup"><span data-stu-id="170ef-125">Bearer {code}.</span></span> <span data-ttu-id="170ef-126">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="170ef-126">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="170ef-127">Corpo da Solicitação</span><span class="sxs-lookup"><span data-stu-id="170ef-127">Request Body</span></span>

<span data-ttu-id="170ef-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="170ef-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="170ef-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="170ef-129">Response</span></span>

<span data-ttu-id="170ef-130">Este método retorna uma coleção de recursos do [site](../resources/site.md) que o usuário está seguindo.</span><span class="sxs-lookup"><span data-stu-id="170ef-130">This method returns a collection of [site](../resources/site.md) resources that the user is following.</span></span>
<span data-ttu-id="170ef-131">Se nenhum site for encontrado, uma coleção vazia será retornada.</span><span class="sxs-lookup"><span data-stu-id="170ef-131">If no sites were found, an empty collection is returned.</span></span>

## <a name="example"></a><span data-ttu-id="170ef-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="170ef-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="170ef-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="170ef-133">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="170ef-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="170ef-134">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-analytics" } -->

```msgraph-interactive
POST /me/followedSites
```
# <a name="javascript"></a>[<span data-ttu-id="170ef-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="170ef-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-analytics-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="170ef-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="170ef-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-analytics-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="170ef-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="170ef-137">Response</span></span>
<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.site)", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
        {
            "id": "contoso.sharepoint.com,2C712604-1370-44E7-A1F5-426573FDA80A,2D2244C3-251A-49EA-93A8-39E1C3A060FE",
            "displayName": "OneDrive Team Site",
            "webUrl": "https://contoso.sharepoint.com/teams/1drvteam",
            "sharepointIds": {
                "listItemId": "1",
                "siteId": "2C712604-1370-44E7-A1F5-426573FDA80A",
                "siteUrl": "https://contoso.sharepoint.com/teams/1drvteam",
                "webId": "2D2244C3-251A-49EA-93A8-39E1C3A060FE"
            },
            "siteCollection": {
                "hostname": "contoso.sharepoint.com"
            }
        },
        {
            "id": "contoso.sharepoint.com,1C712604-1370-44E7-A1F5-426573FDA80A,1D2244C3-251A-49EA-93A8-39E1C3A060FE",
            "displayName": "OneDrive Team Site1",
            "webUrl": "https://contoso.sharepoint.com/teams/2drvteam",
            "sharepointIds": {
                "listItemId": "1",
                "siteId": "1C712604-1370-44E7-A1F5-426573FDA80A",
                "siteUrl": "https://contoso.sharepoint.com/teams/2drvteam",
                "webId": "1D2244C3-251A-49EA-93A8-39E1C3A060FE"
            },
            "siteCollection": {
                "hostname": "contoso.sharepoint.com"
            }
        }
  ]
}
```

<!--
{
  "type": "#page.annotation",
  "description": "List the sites a user is following.",
  "keywords": "site,onedrive.site,list followed sites, followedSites",
  "section": "documentation",
  "tocPath": "Sites/List followed sites",
  "suppressions": [
  ]
}
-->
