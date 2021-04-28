---
title: Listar usados
description: 'Calcule e liste os documentos que um usuário exibiu ou modificou. '
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: ba9b5953f877a6dae825aea6bede63af18c55ffd
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52039542"
---
# <a name="list-used"></a><span data-ttu-id="64cbb-103">Listar usados</span><span class="sxs-lookup"><span data-stu-id="64cbb-103">List used</span></span>

<span data-ttu-id="64cbb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="64cbb-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="64cbb-105">Calcule e liste os documentos que um usuário exibiu ou modificou.</span><span class="sxs-lookup"><span data-stu-id="64cbb-105">Calculate and list the documents that a user has viewed or modified.</span></span> 

<span data-ttu-id="64cbb-106">Para o usuário conectado:</span><span class="sxs-lookup"><span data-stu-id="64cbb-106">For the signed-in user:</span></span>
- <span data-ttu-id="64cbb-107">Este método inclui documentos que o usuário modificou; consulte [o exemplo 1](#example-1-return-documents-that-user-has-modified).</span><span class="sxs-lookup"><span data-stu-id="64cbb-107">This method includes documents that the user has modified; see [example 1](#example-1-return-documents-that-user-has-modified).</span></span> 
- <span data-ttu-id="64cbb-108">Usar um parâmetro de consulta na propriedade `$orderby` **lastAccessedDateTime** retorna os documentos exibidos mais recentemente que o usuário pode ou não ter modificado; consulte [o exemplo 2](#example-2-return-the-most-recently-viewed-documents-that-the-signed-in-user-might-or-might-not-have-modified).</span><span class="sxs-lookup"><span data-stu-id="64cbb-108">Using an `$orderby` query parameter on the **lastAccessedDateTime** property returns the most recently viewed documents that the user might or might not not have modified; see [example 2](#example-2-return-the-most-recently-viewed-documents-that-the-signed-in-user-might-or-might-not-have-modified).</span></span>

<span data-ttu-id="64cbb-109">Para outros usuários, este método inclui apenas documentos que o usuário modificou.</span><span class="sxs-lookup"><span data-stu-id="64cbb-109">For other users, this method includes only documents that the user has modified.</span></span>


## <a name="permissions"></a><span data-ttu-id="64cbb-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="64cbb-110">Permissions</span></span>
<span data-ttu-id="64cbb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64cbb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="64cbb-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="64cbb-113">Permission type</span></span>      | <span data-ttu-id="64cbb-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="64cbb-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="64cbb-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="64cbb-115">Delegated (work or school account)</span></span> | <span data-ttu-id="64cbb-116">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64cbb-116">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="64cbb-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="64cbb-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="64cbb-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="64cbb-118">Not supported.</span></span>    |
|<span data-ttu-id="64cbb-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="64cbb-119">Application</span></span> | <span data-ttu-id="64cbb-120">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64cbb-120">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="64cbb-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="64cbb-121">HTTP request</span></span>

- <span data-ttu-id="64cbb-122">Obter uma lista de documentos que o usuário inscreveu modificou:</span><span class="sxs-lookup"><span data-stu-id="64cbb-122">Get a list of documents that the signed-in user has modified:</span></span>
  <!-- { "blockType": "ignored" } -->
  ```http
  GET /me/insights/used
  ```

- <span data-ttu-id="64cbb-123">Obter uma lista de documentos que o usuário especificado modificou:</span><span class="sxs-lookup"><span data-stu-id="64cbb-123">Get a list of documents that the specified user has modified:</span></span>
  <!-- { "blockType": "ignored" } -->
  ```http
  GET /users/{id | userPrincipalName}/insights/used
  ```
  ><span data-ttu-id="64cbb-124">**Observação**: Solicitar documentos usados **de** outro usuário retorna resultados classificação por **lastModifiedDateTime**.</span><span class="sxs-lookup"><span data-stu-id="64cbb-124">**Note**: Requesting another user's **used** documents returns results sorted by **lastModifiedDateTime**.</span></span> <span data-ttu-id="64cbb-125">**lastAccessedDateTime** é definido como **lastModifiedDateTime**.</span><span class="sxs-lookup"><span data-stu-id="64cbb-125">**lastAccessedDateTime** is then set to **lastModifiedDateTime**.</span></span>


- <span data-ttu-id="64cbb-126">Expanda o recurso referenciado por uma **visão usada:**</span><span class="sxs-lookup"><span data-stu-id="64cbb-126">Expand the resource referenced by a **used** insight:</span></span>
  <!-- { "blockType": "ignored" } -->
  ```http
  GET /me/insights/used/{id}/resource
  GET /users/{id | userPrincipalName}/insights/used/{id}/resource
  ```


## <a name="optional-query-parameters"></a><span data-ttu-id="64cbb-127">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="64cbb-127">Optional query parameters</span></span>
<span data-ttu-id="64cbb-128">Este método dá suporte aos [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta:</span><span class="sxs-lookup"><span data-stu-id="64cbb-128">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response:</span></span>

- <span data-ttu-id="64cbb-129">Use o `$filter` parâmetro de consulta para filtrar itens usados.</span><span class="sxs-lookup"><span data-stu-id="64cbb-129">Use the `$filter` query parameter to filter used items.</span></span> <span data-ttu-id="64cbb-130">Por exemplo, com base no **tipo**:</span><span class="sxs-lookup"><span data-stu-id="64cbb-130">For example, based on **type**:</span></span>
  <!-- { "blockType": "ignored" } -->
  `https://graph.microsoft.com/v1.0/me/insights/used?$filter=ResourceVisualization/Type eq 'PowerPoint'`

- <span data-ttu-id="64cbb-131">Use `$filter` para filtrar itens usados com base em  **containerType**:</span><span class="sxs-lookup"><span data-stu-id="64cbb-131">Use `$filter` to filter used items based on  **containerType**:</span></span>
  <!-- { "blockType": "ignored" } -->
  `https://graph.microsoft.com/v1.0/me/insights/used?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`

  <span data-ttu-id="64cbb-132">Consulte os tipos e tipos de contêiner disponíveis que você pode filtrar em [resourceVisualization](../resources/insights-resourcevisualization.md).</span><span class="sxs-lookup"><span data-stu-id="64cbb-132">See the available container types and types you can filter by in [resourceVisualization](../resources/insights-resourcevisualization.md).</span></span>

- <span data-ttu-id="64cbb-133">Use o parâmetro de consulta para classificar documentos exibidos ou modificados pela última vez pelo usuário in-loca , com base na propriedade `$orderBy` **lastAccessedDateTime:** </span><span class="sxs-lookup"><span data-stu-id="64cbb-133">Use the `$orderBy` query parameter to sort documents last viewed or modified _by the signed-in user_, based on the **lastAccessedDateTime** property:</span></span>
  <!-- { "blockType": "ignored" } -->
  `https://graph.microsoft.com/v1.0/me/insights/used?$orderby=LastUsed/LastAccessedDateTime desc`

  ><span data-ttu-id="64cbb-134">**Observação**: use essa opção de consulta _somente para o usuário de assinatura._</span><span class="sxs-lookup"><span data-stu-id="64cbb-134">**Note**: Use this query option _only for the signed-in user_.</span></span> <span data-ttu-id="64cbb-135">Você não pode usar essa API para obter documentos exibidos ou modificados por outro usuário.</span><span class="sxs-lookup"><span data-stu-id="64cbb-135">You cannot use this API to get documents viewed or modified by another user.</span></span> <span data-ttu-id="64cbb-136">Consulte [o exemplo 2](#example-2-return-the-most-recently-viewed-documents-that-the-signed-in-user-might-or-might-not-have-modified).</span><span class="sxs-lookup"><span data-stu-id="64cbb-136">See [example 2](#example-2-return-the-most-recently-viewed-documents-that-the-signed-in-user-might-or-might-not-have-modified).</span></span>


## <a name="request-headers"></a><span data-ttu-id="64cbb-137">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="64cbb-137">Request headers</span></span>
| <span data-ttu-id="64cbb-138">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="64cbb-138">Header</span></span>       |  <span data-ttu-id="64cbb-139">Valor</span><span class="sxs-lookup"><span data-stu-id="64cbb-139">Value</span></span>|
|:-------------|:------|
| <span data-ttu-id="64cbb-140">Autorização</span><span class="sxs-lookup"><span data-stu-id="64cbb-140">Authorization</span></span>  | <span data-ttu-id="64cbb-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="64cbb-p105">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="64cbb-143">Aceitar</span><span class="sxs-lookup"><span data-stu-id="64cbb-143">Accept</span></span>  | <span data-ttu-id="64cbb-144">application/json</span><span class="sxs-lookup"><span data-stu-id="64cbb-144">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="64cbb-145">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="64cbb-145">Request body</span></span>
<span data-ttu-id="64cbb-146">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="64cbb-146">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="64cbb-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="64cbb-147">Response</span></span>

<span data-ttu-id="64cbb-148">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` lista de itens usados no corpo da resposta. [](../resources/insights-used.md)</span><span class="sxs-lookup"><span data-stu-id="64cbb-148">If successful, this method returns a `200 OK` response code and a list of [used](../resources/insights-used.md) items in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="64cbb-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="64cbb-149">Example</span></span>

### <a name="example-1-return-documents-that-user-has-modified"></a><span data-ttu-id="64cbb-150">Exemplo 1: Retornar documentos modificados pelo usuário</span><span class="sxs-lookup"><span data-stu-id="64cbb-150">Example 1: Return documents that user has modified</span></span>

#### <a name="request"></a><span data-ttu-id="64cbb-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="64cbb-151">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="64cbb-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="64cbb-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_mymodifieddocuments"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/insights/used
```
# <a name="c"></a>[<span data-ttu-id="64cbb-153">C#</span><span class="sxs-lookup"><span data-stu-id="64cbb-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mymodifieddocuments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="64cbb-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="64cbb-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mymodifieddocuments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="64cbb-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="64cbb-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mymodifieddocuments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="64cbb-156">Java</span><span class="sxs-lookup"><span data-stu-id="64cbb-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-mymodifieddocuments-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="64cbb-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="64cbb-157">Response</span></span>

><span data-ttu-id="64cbb-158">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="64cbb-158">**Note:** The response object shown here might be shortened for readability.</span></span> 

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
                "previewImageUrl": "https://contoso.sharepoint.com/_api/v2.0/drives/b!uTdl5maWCEyFRUo_2bKAOg8Q9Rst52JPvFvtTIaQiSaOy9HgmWBFQYDbyM0zog0D/items/01JSNPH6EZHFDPJNKPRNHZTFEWRRLDKPC3/thumbnails/0/small/thumbnailContent",
                "previewText": "Page-1",
                "containerWebUrl": "https://contoso.sharepoint.com/sites/Retail/Shared Documents/NC460 Sales",
                "containerDisplayName": "Retail",
                "containerType": "Site"
            },
            "resourceReference": {
                "webUrl": "https://contoso.sharepoint.com/sites/Retail/_layouts/15/Doc.aspx?sourcedoc=%7BF4463999-4FB5-4F8B-9994-968C56353C5B%7D&file=Org%20Chart.vsdx&action=default&DefaultItemOpen=1",
                "id": "drives/b!uTdl5maWCEyFRUo_2bKAOg8Q9Rst52JPvFvtTIaQiSaOy9HgmWBFQYDbyM0zog0D/items/01JSNPH6EZHFDPJNKPRNHZTFEWRRLDKPC3",
                "type": "microsoft.graph.driveItem"
            }
        }
    ]
}
```

### <a name="example-2-return-the-most-recently-viewed-documents-that-the-signed-in-user-might-or-might-not-have-modified"></a><span data-ttu-id="64cbb-159">Exemplo 2: Retornar os documentos exibidos mais recentemente que o usuário inscreveu pode ou não ter modificado</span><span class="sxs-lookup"><span data-stu-id="64cbb-159">Example 2: Return the most recently viewed documents that the signed-in user might or might not have modified</span></span> 

#### <a name="request"></a><span data-ttu-id="64cbb-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="64cbb-160">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="64cbb-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="64cbb-161">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_mymodifiedandvieweddocuments"
}-->
  
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/insights/used?$orderby=LastUsed/LastAccessedDateTime desc
```
# <a name="c"></a>[<span data-ttu-id="64cbb-162">C#</span><span class="sxs-lookup"><span data-stu-id="64cbb-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mymodifiedandvieweddocuments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="64cbb-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="64cbb-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mymodifiedandvieweddocuments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="64cbb-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="64cbb-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mymodifiedandvieweddocuments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="64cbb-165">Java</span><span class="sxs-lookup"><span data-stu-id="64cbb-165">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-mymodifiedandvieweddocuments-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="64cbb-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="64cbb-166">Response</span></span>
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
            "id": "AWTmrUBYzTxMsvtILkUktIaN-sDnMnRRTYqBxeih4bUUAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAABk5q1AWM08TLL7SC5FJLSGBA",
            "lastUsed": {
                "lastAccessedDateTime": "2020-03-16T13:31:55Z",
                "lastModifiedDateTime": "0001-01-01T00:00:00Z"
            },
            "resourceVisualization": {
                "title": "Executive Corner",
                "type": "spsite",
                "mediaType": "application/octet-stream",
                "previewImageUrl": "https://contoso.sharepoint.com/_api/v2.0/drives/b!ZOatQFjNPEyy-0guRSS0ho36wOcydFFNioHF6KHhtRQAAAAAAAAAAAAAAAAAAAAA/items/01NTE4NPQAAAAAAAAAAAAAAAAAAAAAAAAA/thumbnails/0/small/thumbnailContent",
                "previewText": "",
                "containerDisplayName": "Executive Corner",
                "containerType": "Site"
            },
            "resourceReference": {
                "webUrl": "https://contoso.sharepoint.com/sites/Exec",
                "id": "sites/contoso.sharepoint.com,40ade664-cd58-4c3c-b2fb-482e4524b486,e7c0fa8d-7432-4d51-8a81-c5e8a1e1b514",
                "type": "microsoft.graph.siteItem"
            }
        }
    ]
}
```

