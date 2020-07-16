---
author: learafa
description: Liste os sites que foram seguidos pelo usuário conectado.
title: Listar sites seguidos
localization_priority: Normal
ms.prod: SharePoint
doc_type: apiPageType
ms.openlocfilehash: e1f1d781897802eab62674d4bbed18507ec4d2c6
ms.sourcegitcommit: e20c113409836115f338dcfe3162342ef3bd6a4a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/01/2020
ms.locfileid: "45006668"
---
# <a name="list-followed-sites"></a><span data-ttu-id="d5d5d-103">Listar sites seguidos</span><span class="sxs-lookup"><span data-stu-id="d5d5d-103">List followed sites</span></span>

<span data-ttu-id="d5d5d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d5d5d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d5d5d-105">Listar os [sites](../resources/site.md) que foram seguidos pelo usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="d5d5d-105">List the [sites](../resources/site.md) that have been followed by the signed in user.</span></span>

## <a name="permissions"></a><span data-ttu-id="d5d5d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d5d5d-106">Permissions</span></span>

<span data-ttu-id="d5d5d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d5d5d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d5d5d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d5d5d-109">Permission type</span></span>      | <span data-ttu-id="d5d5d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d5d5d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d5d5d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d5d5d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d5d5d-112">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5d5d-112">Sites.Read.All, Sites.ReadWrite.All</span></span>  |
|<span data-ttu-id="d5d5d-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d5d5d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d5d5d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d5d5d-114">Not supported.</span></span>    |
|<span data-ttu-id="d5d5d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d5d5d-115">Application</span></span> | <span data-ttu-id="d5d5d-116">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5d5d-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d5d5d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d5d5d-117">HTTP request</span></span>

<span data-ttu-id="d5d5d-118">Este método é acessível apenas por meio do OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="d5d5d-118">This method is accessible only through OneDrive for Business.</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/followedSites
```
<span data-ttu-id="d5d5d-119">Obter uma lista dos sites seguidos por um usuário de destino com base em sua ID.</span><span class="sxs-lookup"><span data-stu-id="d5d5d-119">Get a list of the sites followed by a target user, based on its ID.</span></span>

```http
GET /users/{user-id}/followedSites
```
<span data-ttu-id="d5d5d-120">**Observação:** Para acessar a lista de sites seguidos de outro usuário direcionado, você precisa de permissões de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d5d5d-120">**Note:** To access another targeted user's list of followed sites, you need application permissions.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="d5d5d-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d5d5d-121">Optional query parameters</span></span>
<span data-ttu-id="d5d5d-122">Este método dá suporte a [Parâmetros de consulta OData](/graph/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d5d5d-122">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d5d5d-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d5d5d-123">Request headers</span></span>

| <span data-ttu-id="d5d5d-124">Nome</span><span class="sxs-lookup"><span data-stu-id="d5d5d-124">Name</span></span>      |<span data-ttu-id="d5d5d-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5d5d-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d5d5d-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="d5d5d-126">Authorization</span></span>  | <span data-ttu-id="d5d5d-127">Portador {código}.</span><span class="sxs-lookup"><span data-stu-id="d5d5d-127">Bearer {code}.</span></span> <span data-ttu-id="d5d5d-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d5d5d-128">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d5d5d-129">Corpo da Solicitação</span><span class="sxs-lookup"><span data-stu-id="d5d5d-129">Request Body</span></span>

<span data-ttu-id="d5d5d-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d5d5d-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d5d5d-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="d5d5d-131">Response</span></span>

<span data-ttu-id="d5d5d-132">Este método retorna uma coleção de recursos do [site](../resources/site.md) que o usuário está seguindo.</span><span class="sxs-lookup"><span data-stu-id="d5d5d-132">This method returns a collection of [site](../resources/site.md) resources that the user is following.</span></span>
<span data-ttu-id="d5d5d-133">Se nenhum site for encontrado, uma coleção vazia será retornada.</span><span class="sxs-lookup"><span data-stu-id="d5d5d-133">If no sites were found, an empty collection is returned.</span></span>

## <a name="example"></a><span data-ttu-id="d5d5d-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d5d5d-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="d5d5d-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d5d5d-135">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="d5d5d-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="d5d5d-136">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "sites-list-followed", "scopes": "sites.readwrite.all" } -->

```msgraph-interactive
GET /me/followedSites
```
# <a name="javascript"></a>[<span data-ttu-id="d5d5d-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d5d5d-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/sites-list-followed-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d5d5d-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d5d5d-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/sites-list-followed-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="d5d5d-139">C#</span><span class="sxs-lookup"><span data-stu-id="d5d5d-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/sites-list-followed-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d5d5d-140">Java</span><span class="sxs-lookup"><span data-stu-id="d5d5d-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/sites-list-followed-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d5d5d-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="d5d5d-141">Response</span></span>
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
