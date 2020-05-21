---
title: Listar usados
description: Calcular e listar os documentos exibidos ou modificados pelo usuário.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: b045ae3d66dded3ed6a85e59282a768b22d9f7fe
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/21/2020
ms.locfileid: "44332680"
---
# <a name="list-used"></a><span data-ttu-id="4e6d0-103">Listar usados</span><span class="sxs-lookup"><span data-stu-id="4e6d0-103">List used</span></span>

<span data-ttu-id="4e6d0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4e6d0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4e6d0-105">Calcular e listar os documentos que um usuário tenha exibido ou modificado.</span><span class="sxs-lookup"><span data-stu-id="4e6d0-105">Calculate and list the documents that a user has viewed or modified.</span></span> 

<span data-ttu-id="4e6d0-106">Para o usuário conectado:</span><span class="sxs-lookup"><span data-stu-id="4e6d0-106">For the signed-in user:</span></span>
- <span data-ttu-id="4e6d0-107">Este método inclui documentos que o usuário modificou; Confira o [exemplo 1](#example-1-return-documents-that-user-has-modified).</span><span class="sxs-lookup"><span data-stu-id="4e6d0-107">This method includes documents that the user has modified; see [example 1](#example-1-return-documents-that-user-has-modified).</span></span> 
- <span data-ttu-id="4e6d0-108">O uso de um `$orderby` parâmetro de consulta na propriedade **lastAccessedDateTime** retorna os documentos exibidos mais recentemente que o usuário pode ou não tenha modificado; Veja o [exemplo 2](#example-2-return-the-most-recently-viewed-documents-that-the-signed-in-user-might-or-might-not-have-modified).</span><span class="sxs-lookup"><span data-stu-id="4e6d0-108">Using an `$orderby` query parameter on the **lastAccessedDateTime** property returns the most recently viewed documents that the user might or might not have modified; see [example 2](#example-2-return-the-most-recently-viewed-documents-that-the-signed-in-user-might-or-might-not-have-modified).</span></span>

<span data-ttu-id="4e6d0-109">Para outros usuários, esse método inclui apenas os documentos que o usuário modificou.</span><span class="sxs-lookup"><span data-stu-id="4e6d0-109">For other users, this method includes only documents that the user has modified.</span></span>


## <a name="permissions"></a><span data-ttu-id="4e6d0-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="4e6d0-110">Permissions</span></span>
<span data-ttu-id="4e6d0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4e6d0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4e6d0-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4e6d0-113">Permission type</span></span>      | <span data-ttu-id="4e6d0-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4e6d0-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4e6d0-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4e6d0-115">Delegated (work or school account)</span></span> | <span data-ttu-id="4e6d0-116">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e6d0-116">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="4e6d0-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4e6d0-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4e6d0-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4e6d0-118">Not supported.</span></span>    |
|<span data-ttu-id="4e6d0-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4e6d0-119">Application</span></span> | <span data-ttu-id="4e6d0-120">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e6d0-120">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4e6d0-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4e6d0-121">HTTP request</span></span>

- <span data-ttu-id="4e6d0-122">Obter uma lista de documentos que o usuário conectado modificou:</span><span class="sxs-lookup"><span data-stu-id="4e6d0-122">Get a list of documents that the signed-in user has modified:</span></span>
  <!-- { "blockType": "ignored" } -->
  ```http
  GET /me/insights/used
  ```

- <span data-ttu-id="4e6d0-123">Obtenha uma lista de documentos que o usuário especificado modificou:</span><span class="sxs-lookup"><span data-stu-id="4e6d0-123">Get a list of documents that the specified user has modified:</span></span>
  <!-- { "blockType": "ignored" } -->
  ```http
  GET /users/{id | userPrincipalName}/insights/used
  ```
  ><span data-ttu-id="4e6d0-124">**Observação**: a solicitação de documentos **usados** por outro usuário retorna resultados classificados por **lastModifiedDateTime**.</span><span class="sxs-lookup"><span data-stu-id="4e6d0-124">**Note**: Requesting another user's **used** documents returns results sorted by **lastModifiedDateTime**.</span></span> <span data-ttu-id="4e6d0-125">**lastAccessedDateTime** é então definido como **lastModifiedDateTime**.</span><span class="sxs-lookup"><span data-stu-id="4e6d0-125">**lastAccessedDateTime** is then set to **lastModifiedDateTime**.</span></span>


- <span data-ttu-id="4e6d0-126">Expanda o recurso mencionado por uma percepção **usada** :</span><span class="sxs-lookup"><span data-stu-id="4e6d0-126">Expand the resource referenced by a **used** insight:</span></span>
  <!-- { "blockType": "ignored" } -->
  ```http
  GET /me/insights/used/{id}/resource
  GET /users/{id | userPrincipalName}/insights/used/{id}/resource
  ```


## <a name="optional-query-parameters"></a><span data-ttu-id="4e6d0-127">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="4e6d0-127">Optional query parameters</span></span>
<span data-ttu-id="4e6d0-128">Este método oferece suporte aos [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta:</span><span class="sxs-lookup"><span data-stu-id="4e6d0-128">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response:</span></span>

- <span data-ttu-id="4e6d0-129">Use o `$filter` parâmetro de consulta para filtrar itens usados.</span><span class="sxs-lookup"><span data-stu-id="4e6d0-129">Use the `$filter` query parameter to filter used items.</span></span> <span data-ttu-id="4e6d0-130">Por exemplo, com base no **tipo**:</span><span class="sxs-lookup"><span data-stu-id="4e6d0-130">For example, based on **type**:</span></span>

  <!-- { "blockType": "ignored" } -->
  `https://graph.microsoft.com/beta/me/insights/used?$filter=ResourceVisualization/Type eq 'PowerPoint'`

- <span data-ttu-id="4e6d0-131">Use `$filter` para filtrar itens usados com base no **ContainerType**:</span><span class="sxs-lookup"><span data-stu-id="4e6d0-131">Use `$filter` to filter used items based on  **containerType**:</span></span>
  <!-- { "blockType": "ignored" } -->
  `https://graph.microsoft.com/beta/me/insights/used?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`

  <span data-ttu-id="4e6d0-132">Confira os tipos e tipos de contêiner disponíveis que você pode filtrar no [resourceVisualization](../resources/insights-resourcevisualization.md).</span><span class="sxs-lookup"><span data-stu-id="4e6d0-132">See the available container types and types you can filter by in [resourceVisualization](../resources/insights-resourcevisualization.md).</span></span>

- <span data-ttu-id="4e6d0-133">Use o `$orderBy` parâmetro de consulta para classificar documentos que foram exibidos pela última vez ou modificados _pelo usuário conectado_, com base na propriedade **lastAccessedDateTime** :</span><span class="sxs-lookup"><span data-stu-id="4e6d0-133">Use the `$orderBy` query parameter to sort documents last viewed or modified _by the signed-in user_, based on the **lastAccessedDateTime** property:</span></span>
  <!-- { "blockType": "ignored" } -->
  `https://graph.microsoft.com/beta/me/insights/used?$orderby=LastUsed/LastAccessedDateTime desc`

  ><span data-ttu-id="4e6d0-134">**Observação**: Use esta opção _de consulta somente para o usuário conectado_.</span><span class="sxs-lookup"><span data-stu-id="4e6d0-134">**Note**: Use this query option _only for the signed-in user_.</span></span> <span data-ttu-id="4e6d0-135">Você não pode usar essa API para obter documentos exibidos ou modificados por outro usuário.</span><span class="sxs-lookup"><span data-stu-id="4e6d0-135">You cannot use this API to get documents viewed or modified by another user.</span></span> <span data-ttu-id="4e6d0-136">Confira o [exemplo 2](#example-2-return-the-most-recently-viewed-documents-that-the-signed-in-user-might-or-might-not-have-modified).</span><span class="sxs-lookup"><span data-stu-id="4e6d0-136">See [example 2](#example-2-return-the-most-recently-viewed-documents-that-the-signed-in-user-might-or-might-not-have-modified).</span></span>


## <a name="request-headers"></a><span data-ttu-id="4e6d0-137">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4e6d0-137">Request headers</span></span>
| <span data-ttu-id="4e6d0-138">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4e6d0-138">Header</span></span>       |  <span data-ttu-id="4e6d0-139">Valor</span><span class="sxs-lookup"><span data-stu-id="4e6d0-139">Value</span></span>|
|:-------------|:------|
| <span data-ttu-id="4e6d0-140">Autorização</span><span class="sxs-lookup"><span data-stu-id="4e6d0-140">Authorization</span></span>  | <span data-ttu-id="4e6d0-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4e6d0-p105">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="4e6d0-143">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4e6d0-143">Accept</span></span>  | <span data-ttu-id="4e6d0-144">application/json</span><span class="sxs-lookup"><span data-stu-id="4e6d0-144">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4e6d0-145">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4e6d0-145">Request body</span></span>
<span data-ttu-id="4e6d0-146">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4e6d0-146">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4e6d0-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="4e6d0-147">Response</span></span>

<span data-ttu-id="4e6d0-148">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma lista de itens [usados](../resources/insights-used.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4e6d0-148">If successful, this method returns a `200 OK` response code and a list of [used](../resources/insights-used.md) items in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4e6d0-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4e6d0-149">Example</span></span>

### <a name="example-1-return-documents-that-user-has-modified"></a><span data-ttu-id="4e6d0-150">Exemplo 1: retornar documentos modificados pelo usuário</span><span class="sxs-lookup"><span data-stu-id="4e6d0-150">Example 1: Return documents that user has modified</span></span>

#### <a name="request"></a><span data-ttu-id="4e6d0-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4e6d0-151">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="4e6d0-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="4e6d0-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_mymodifieddocuments"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/insights/used
```
# <a name="c"></a>[<span data-ttu-id="4e6d0-153">C#</span><span class="sxs-lookup"><span data-stu-id="4e6d0-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mymodifieddocuments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4e6d0-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4e6d0-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mymodifieddocuments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4e6d0-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4e6d0-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mymodifieddocuments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="4e6d0-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="4e6d0-156">Response</span></span>

><span data-ttu-id="4e6d0-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4e6d0-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.usedInsight"
}-->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('c74dcd16-d8af-4df8-9621-d123b58de3e6')/insights/used",
    "value": [
        {
            "id": "Abk3ZeZmlghMhUVKP9mygDoPEPUbLediT7xb7UyGkIkmjsvR4JlgRUGA28jNM6INA5k5RvS1T4tPmZSWjFY1PFu5N2XmZpYITIVFSj_ZsoA6BQ",
            "lastUsed": {
                "lastAccessedDateTime": "2019-05-25T07:12:38Z",
                "lastModifiedDateTime": "2019-05-25T07:12:37Z"
            },
            "resourceVisualization": {
                "title": "Org Chart",
                "type": "Visio",
                "mediaType": "application/vnd.visio",
                "previewImageUrl": "https://m365x887078.sharepoint.com/_api/v2.0/drives/b!uTdl5maWCEyFRUo_2bKAOg8Q9Rst52JPvFvtTIaQiSaOy9HgmWBFQYDbyM0zog0D/items/01JSNPH6EZHFDPJNKPRNHZTFEWRRLDKPC3/thumbnails/0/small/thumbnailContent",
                "previewText": "Page-1",
                "containerWebUrl": "https://m365x887078.sharepoint.com/sites/Retail/Shared Documents/NC460 Sales",
                "containerDisplayName": "Retail",
                "containerType": "Site"
            },
            "resourceReference": {
                "webUrl": "https://m365x887078.sharepoint.com/sites/Retail/_layouts/15/Doc.aspx?sourcedoc=%7BF4463999-4FB5-4F8B-9994-968C56353C5B%7D&file=Org%20Chart.vsdx&action=default&DefaultItemOpen=1",
                "id": "drives/b!uTdl5maWCEyFRUo_2bKAOg8Q9Rst52JPvFvtTIaQiSaOy9HgmWBFQYDbyM0zog0D/items/01JSNPH6EZHFDPJNKPRNHZTFEWRRLDKPC3",
                "type": "microsoft.graph.driveItem"
            }
        },
        {
            "id": "AaVI6n5KqI5FjDqNnB_O-IwPEPUbLediT7xb7UyGkIkmjsvR4JlgRUGA28jNM6INA5T7emOJwqlCit_j9Q5CpWSlSOp-SqiORYw6jZwfzviMBQ",
            "lastUsed": {
                "lastAccessedDateTime": "2019-05-25T07:12:26Z",
                "lastModifiedDateTime": "2019-05-25T07:12:26Z"
            },
            "resourceVisualization": {
                "title": "USA Sales",
                "type": "Excel",
                "mediaType": "application/vnd.openxmlformats-officedocument.spreadsheetml.sheet",
                "previewImageUrl": "https://m365x887078.sharepoint.com/_api/v2.0/drives/b!pUjqfkqojkWMOo2cH874jA8Q9Rst52JPvFvtTIaQiSaOy9HgmWBFQYDbyM0zog0D/items/01YAUTJM4U7N5GHCOCVFBIVX7D6UHEFJLE/thumbnails/0/small/thumbnailContent",
                "previewText": "Product Category Product  Product Category - Product Target Revenue TY YTD Revenue Variance to Target Revenue COGS List Price % of List Price Actual Margin Target Margin Audio Car Audio Audio - Car Audio 4910000 4664500 245500 3928000 4320800 -736500 Audi",
                "containerWebUrl": "https://m365x887078.sharepoint.com/sites/SalesAndMarketing/Shared Documents/Monthly Reports",
                "containerDisplayName": "Sales and Marketing",
                "containerType": "Site"
            },
            "resourceReference": {
                "webUrl": "https://m365x887078.sharepoint.com/sites/SalesAndMarketing/_layouts/15/Doc.aspx?sourcedoc=%7B637AFB94-C289-42A9-8ADF-E3F50E42A564%7D&file=USA%20Sales.xlsx&action=default&mobileredirect=true&DefaultItemOpen=1",
                "id": "drives/b!pUjqfkqojkWMOo2cH874jA8Q9Rst52JPvFvtTIaQiSaOy9HgmWBFQYDbyM0zog0D/items/01YAUTJM4U7N5GHCOCVFBIVX7D6UHEFJLE",
                "type": "microsoft.graph.driveItem"
            }
        },
        {
            "id": "AaVI6n5KqI5FjDqNnB_O-IwPEPUbLediT7xb7UyGkIkmjsvR4JlgRUGA28jNM6INAy6LlBcXfAJCmOiEWgBJjh-lSOp-SqiORYw6jZwfzviMBQ",
            "lastUsed": {
                "lastAccessedDateTime": "2019-05-25T07:11:49Z",
                "lastModifiedDateTime": "2019-05-25T07:11:48Z"
            },
            "resourceVisualization": {
                "title": "UK Sales",
                "type": "Excel",
                "mediaType": "application/vnd.openxmlformats-officedocument.spreadsheetml.sheet",
                "previewImageUrl": "https://m365x887078.sharepoint.com/_api/v2.0/drives/b!pUjqfkqojkWMOo2cH874jA8Q9Rst52JPvFvtTIaQiSaOy9HgmWBFQYDbyM0zog0D/items/01YAUTJMZOROKBOF34AJBJR2EELIAETDQ7/thumbnails/0/small/thumbnailContent",
                "previewText": "Product Category Product  Product Category - Product Target Revenue TY YTD Revenue Variance to Target Revenue COGS List Price % of List Price Actual Margin Target Margin Electronics Wearable Technology Electronics - Wearable Technology 2226000 2114700 111",
                "containerWebUrl": "https://m365x887078.sharepoint.com/sites/SalesAndMarketing/Shared Documents/Monthly Reports",
                "containerDisplayName": "Sales and Marketing",
                "containerType": "Site"
            },
            "resourceReference": {
                "webUrl": "https://m365x887078.sharepoint.com/sites/SalesAndMarketing/_layouts/15/Doc.aspx?sourcedoc=%7B17948B2E-7C17-4202-98E8-845A00498E1F%7D&file=UK%20Sales.xlsx&action=default&mobileredirect=true&DefaultItemOpen=1",
                "id": "drives/b!pUjqfkqojkWMOo2cH874jA8Q9Rst52JPvFvtTIaQiSaOy9HgmWBFQYDbyM0zog0D/items/01YAUTJMZOROKBOF34AJBJR2EELIAETDQ7",
                "type": "microsoft.graph.driveItem"
            }
        }
    ]
}
```

### <a name="example-2-return-the-most-recently-viewed-documents-that-the-signed-in-user-might-or-might-not-have-modified"></a><span data-ttu-id="4e6d0-159">Exemplo 2: retornar os documentos exibidos mais recentemente que o usuário conectado pode ou não tenha modificado</span><span class="sxs-lookup"><span data-stu-id="4e6d0-159">Example 2: Return the most recently viewed documents that the signed-in user might or might not have modified</span></span> 

#### <a name="request"></a><span data-ttu-id="4e6d0-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4e6d0-160">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="4e6d0-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="4e6d0-161">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_mymodifiedandvieweddocuments"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/insights/used?$orderby=LastUsed/LastAccessedDateTime desc
```
# <a name="c"></a>[<span data-ttu-id="4e6d0-162">C#</span><span class="sxs-lookup"><span data-stu-id="4e6d0-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mymodifiedandvieweddocuments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4e6d0-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4e6d0-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mymodifiedandvieweddocuments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4e6d0-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4e6d0-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mymodifiedandvieweddocuments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="4e6d0-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="4e6d0-165">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.usedInsight"
}-->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('c74dcd16-d8af-4df8-9621-d123b58de3e6')/insights/used",
    "value": [
        {
            "id": "AWTmrUBYzTxMsvtILkUktIaN-sDnMnRRTYqBxeih4bUUAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAABk5q1AWM08TLL7SC5FJLSGBA",
            "lastUsed": {
                "lastAccessedDateTime": "2020-03-16T13:31:55Z",
                "lastModifiedDateTime": "0001-01-01T00:00:00Z"
            },
            "resourceVisualization": {
                "title": "Executive Corner",
                "type": "spsite",
                "mediaType": "application/octet-stream",
                "previewImageUrl": "https://m365x887078.sharepoint.com/_api/v2.0/drives/b!ZOatQFjNPEyy-0guRSS0ho36wOcydFFNioHF6KHhtRQAAAAAAAAAAAAAAAAAAAAA/items/01NTE4NPQAAAAAAAAAAAAAAAAAAAAAAAAA/thumbnails/0/small/thumbnailContent",
                "previewText": "",
                "containerDisplayName": "Executive Corner",
                "containerType": "Site"
            },
            "resourceReference": {
                "webUrl": "https://m365x887078.sharepoint.com/sites/Exec",
                "id": "sites/m365x887078.sharepoint.com,40ade664-cd58-4c3c-b2fb-482e4524b486,e7c0fa8d-7432-4d51-8a81-c5e8a1e1b514",
                "type": "microsoft.graph.siteItem"
            }
        },
        {
            "id": "AahdFRA14_FMrGLq9V4WmyiN-sDnMnRRTYqBxeih4bUUAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAACoXRUQNePxTKxi6vVeFpsoBA",
            "lastUsed": {
                "lastAccessedDateTime": "2020-03-16T13:31:55Z",
                "lastModifiedDateTime": "0001-01-01T00:00:00Z"
            },
            "resourceVisualization": {
                "title": "Contoso Landings",
                "type": "spsite",
                "mediaType": "application/octet-stream",
                "previewImageUrl": "https://m365x887078.sharepoint.com/_api/v2.0/drives/b!qF0VEDXj8UysYur1XhabKI36wOcydFFNioHF6KHhtRQAAAAAAAAAAAAAAAAAAAAA/items/01UHO6LBAAAAAAAAAAAAAAAAAAAAAAAAAA/thumbnails/0/small/thumbnailContent",
                "previewText": "",
                "containerDisplayName": "Contoso Landings",
                "containerType": "Site"
            },
            "resourceReference": {
                "webUrl": "https://m365x887078.sharepoint.com/sites/ContosoLandings",
                "id": "sites/m365x887078.sharepoint.com,10155da8-e335-4cf1-ac62-eaf55e169b28,e7c0fa8d-7432-4d51-8a81-c5e8a1e1b514",
                "type": "microsoft.graph.siteItem"
            }
        },
        {
            "id": "AaVI6n5KqI5FjDqNnB_O-IztQAKAS6acR7HFoIKDqOPE6bjkeoHWtEu7LoUIsZkHSkzLaA_67htEozMGRwifyaqlSOp-SqiORYw6jZwfzviMBQ",
            "lastUsed": {
                "lastAccessedDateTime": "2020-03-16T13:31:54Z",
                "lastModifiedDateTime": "0001-01-01T00:00:00Z"
            },
            "resourceVisualization": {
                "title": "Media Preview Packages",
                "type": "Web",
                "mediaType": "text/html",
                "previewImageUrl": "https://m365x887078.sharepoint.com/_api/v2.0/drives/b!pUjqfkqojkWMOo2cH874jO1AAoBLppxHscWggoOo48TpuOR6gda0S7suhQixmQdK/items/01RGQ6XKCMZNUA76XODNCKGMYGI4EJ7SNK/thumbnails/0/small/thumbnailContent",
                "previewText": "",
                "containerWebUrl": "https://m365x887078.sharepoint.com/sites/SalesAndMarketing/CampaignsEvents/SitePages/Forms/ByAuthor.aspx",
                "containerDisplayName": "Campaigns - Events"
            },
            "resourceReference": {
                "webUrl": "https://m365x887078.sharepoint.com/sites/SalesAndMarketing/CampaignsEvents/SitePages/Media-Preview-Packages.aspx"
            }
        }
    ]
}
```
