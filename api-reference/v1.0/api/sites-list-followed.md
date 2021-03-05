---
author: learafa
description: Liste os sites que foram seguidos pelo usuário conectado.
title: Listar sites seguidos
localization_priority: Normal
ms.prod: SharePoint
doc_type: apiPageType
ms.openlocfilehash: 4520d428511601ad2fa17c4d993a6ab373566eb0
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50473676"
---
# <a name="list-followed-sites"></a><span data-ttu-id="7ceb8-103">Listar sites seguidos</span><span class="sxs-lookup"><span data-stu-id="7ceb8-103">List followed sites</span></span>

<span data-ttu-id="7ceb8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7ceb8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7ceb8-105">Listar [os sites](../resources/site.md) que foram seguidos pelo usuário assinado.</span><span class="sxs-lookup"><span data-stu-id="7ceb8-105">List the [sites](../resources/site.md) that have been followed by the signed in user.</span></span>

## <a name="permissions"></a><span data-ttu-id="7ceb8-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="7ceb8-106">Permissions</span></span>

<span data-ttu-id="7ceb8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7ceb8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7ceb8-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7ceb8-109">Permission type</span></span>      | <span data-ttu-id="7ceb8-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7ceb8-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7ceb8-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7ceb8-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7ceb8-112">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ceb8-112">Sites.Read.All, Sites.ReadWrite.All</span></span>  |
|<span data-ttu-id="7ceb8-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7ceb8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7ceb8-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7ceb8-114">Not supported.</span></span>    |
|<span data-ttu-id="7ceb8-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7ceb8-115">Application</span></span> | <span data-ttu-id="7ceb8-116">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ceb8-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7ceb8-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7ceb8-117">HTTP request</span></span>

<span data-ttu-id="7ceb8-118">Esse método só pode ser acessado por meio do OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="7ceb8-118">This method is accessible only through OneDrive for Business.</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/followedSites
```
<span data-ttu-id="7ceb8-119">Obter uma lista dos sites seguidos por um usuário de destino, com base em sua ID.</span><span class="sxs-lookup"><span data-stu-id="7ceb8-119">Get a list of the sites followed by a target user, based on its ID.</span></span>

```http
GET /users/{user-id}/followedSites
```
<span data-ttu-id="7ceb8-120">**Observação:** Para acessar a lista de sites seguidos de outro usuário direcionado, você precisa de permissões de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7ceb8-120">**Note:** To access another targeted user's list of followed sites, you need application permissions.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="7ceb8-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7ceb8-121">Optional query parameters</span></span>
<span data-ttu-id="7ceb8-122">Este método dá suporte a [Parâmetros de consulta OData](/graph/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7ceb8-122">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7ceb8-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7ceb8-123">Request headers</span></span>

| <span data-ttu-id="7ceb8-124">Nome</span><span class="sxs-lookup"><span data-stu-id="7ceb8-124">Name</span></span>      |<span data-ttu-id="7ceb8-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="7ceb8-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7ceb8-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="7ceb8-126">Authorization</span></span>  | <span data-ttu-id="7ceb8-127">Portador {código}.</span><span class="sxs-lookup"><span data-stu-id="7ceb8-127">Bearer {code}.</span></span> <span data-ttu-id="7ceb8-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7ceb8-128">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7ceb8-129">Corpo da Solicitação</span><span class="sxs-lookup"><span data-stu-id="7ceb8-129">Request Body</span></span>

<span data-ttu-id="7ceb8-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7ceb8-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7ceb8-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="7ceb8-131">Response</span></span>

<span data-ttu-id="7ceb8-132">Este método retorna um conjunto de [recursos de site](../resources/site.md) que o usuário está seguindo.</span><span class="sxs-lookup"><span data-stu-id="7ceb8-132">This method returns a collection of [site](../resources/site.md) resources that the user is following.</span></span>
<span data-ttu-id="7ceb8-133">Se nenhum site for encontrado, uma coleção vazia será retornada.</span><span class="sxs-lookup"><span data-stu-id="7ceb8-133">If no sites were found, an empty collection is returned.</span></span>

## <a name="example"></a><span data-ttu-id="7ceb8-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7ceb8-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="7ceb8-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7ceb8-135">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="7ceb8-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="7ceb8-136">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "sites-list-followed", "scopes": "sites.readwrite.all" } -->

```msgraph-interactive
GET /me/followedSites
```
# <a name="javascript"></a>[<span data-ttu-id="7ceb8-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7ceb8-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/sites-list-followed-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7ceb8-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7ceb8-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/sites-list-followed-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="7ceb8-139">C#</span><span class="sxs-lookup"><span data-stu-id="7ceb8-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/sites-list-followed-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7ceb8-140">Java</span><span class="sxs-lookup"><span data-stu-id="7ceb8-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/sites-list-followed-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7ceb8-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="7ceb8-141">Response</span></span>
<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.site)", "truncated": true } -->

```http
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

