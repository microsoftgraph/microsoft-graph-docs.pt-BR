---
author: JeremyKelley
ms.author: jeremyke
title: Obter pacote
description: Obter um pacote de driveItems
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: f9deca81a99d36e91247ddd042fc875d0ffc1cad
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48960288"
---
# <a name="get-bundle"></a><span data-ttu-id="d106b-103">Obter pacote</span><span class="sxs-lookup"><span data-stu-id="d106b-103">Get bundle</span></span>

<span data-ttu-id="d106b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d106b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d106b-105">Recupere os metadados de um [pacote][] com base na ID exclusiva do pacote.</span><span class="sxs-lookup"><span data-stu-id="d106b-105">Retrieve the metadata for a [bundle][] based on the bundle's unique ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="d106b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d106b-106">Permissions</span></span>

<span data-ttu-id="d106b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d106b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d106b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d106b-109">Permission type</span></span>      | <span data-ttu-id="d106b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d106b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d106b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d106b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d106b-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d106b-112">Not supported.</span></span>                             |
|<span data-ttu-id="d106b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d106b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d106b-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d106b-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="d106b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d106b-115">Application</span></span>          | <span data-ttu-id="d106b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d106b-116">Not supported.</span></span>                                           |

## <a name="http-request"></a><span data-ttu-id="d106b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d106b-117">HTTP request</span></span>

```http
GET /drive/bundles/{bundle-id}
GET /drive/items/{bundle-id}
```

<span data-ttu-id="d106b-118">Como os pacotes são itens, você pode usar a coleção **Items** para retornar metadados sobre um pacote.</span><span class="sxs-lookup"><span data-stu-id="d106b-118">Because bundles are items, you can use the **items** collection to return metadata about a bundle.</span></span>
<span data-ttu-id="d106b-119">Você também pode usar a coleção de **pacotes** como uma conveniência para garantir que você esteja obtendo um pacote em resposta.</span><span class="sxs-lookup"><span data-stu-id="d106b-119">You can also use the **bundles** collection as a convenience to ensure you're getting a bundle in response.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="d106b-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d106b-120">Optional query parameters</span></span>

<span data-ttu-id="d106b-121">Você pode usar os [parâmetros de consulta OData][odata-parameters] para restringir a forma dos objetos retornados dessa chamada.</span><span class="sxs-lookup"><span data-stu-id="d106b-121">You can use the [OData query parameters][odata-parameters] to restrict the shape of the objects returned from this call.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d106b-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d106b-122">Request headers</span></span>
| <span data-ttu-id="d106b-123">Nome</span><span class="sxs-lookup"><span data-stu-id="d106b-123">Name</span></span>          | <span data-ttu-id="d106b-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="d106b-124">Description</span></span>  |
|:------------- |:------------ |
| <span data-ttu-id="d106b-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="d106b-125">Authorization</span></span> | <span data-ttu-id="d106b-126">\{token\} de portador.</span><span class="sxs-lookup"><span data-stu-id="d106b-126">Bearer \{token\}.</span></span> <span data-ttu-id="d106b-127">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d106b-127">Required.</span></span> |
| <span data-ttu-id="d106b-128">if-none-match</span><span class="sxs-lookup"><span data-stu-id="d106b-128">if-none-match</span></span> | <span data-ttu-id="d106b-129">ETag.</span><span class="sxs-lookup"><span data-stu-id="d106b-129">eTag.</span></span> <span data-ttu-id="d106b-130">Opcional.</span><span class="sxs-lookup"><span data-stu-id="d106b-130">Optional.</span></span> <span data-ttu-id="d106b-131">Se este cabeçalho de solicitação estiver incluso e a eTag (ou cTag) fornecida corresponder à marca atual do arquivo, uma resposta `HTTP 304 Not Modified` será retornada.</span><span class="sxs-lookup"><span data-stu-id="d106b-131">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span>

## <a name="request-body"></a><span data-ttu-id="d106b-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d106b-132">Request body</span></span>

<span data-ttu-id="d106b-133">Não forneça um corpo de solicitação com esse método.</span><span class="sxs-lookup"><span data-stu-id="d106b-133">Do not supply a request body with this method.</span></span>

## <a name="response"></a><span data-ttu-id="d106b-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="d106b-134">Response</span></span>

<span data-ttu-id="d106b-135">Se bem-sucedido, este método retorna um [driveItem][driveItem] resource with the [bundle][bundle] no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d106b-135">If successful, this method returns a [driveItem][driveItem] resource with the [bundle][bundle] in the response body.</span></span>

<span data-ttu-id="d106b-136">Leia o tópico [respostas de erro][error-response] para obter mais informações sobre como os erros são retornados.</span><span class="sxs-lookup"><span data-stu-id="d106b-136">Read the [Error Responses][error-response] topic for more info about how errors are returned.</span></span>

## <a name="examples"></a><span data-ttu-id="d106b-137">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d106b-137">Examples</span></span>

### <a name="example-1-get-a-bundle"></a><span data-ttu-id="d106b-138">Exemplo 1: obter um pacote</span><span class="sxs-lookup"><span data-stu-id="d106b-138">Example 1: Get a bundle</span></span>

#### <a name="request"></a><span data-ttu-id="d106b-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d106b-139">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="d106b-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="d106b-140">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-bundle-metadata" } -->

```msgraph-interactive
GET https://graph.microsoft.com/beta/drive/bundles/{bundle-id}
```
# <a name="c"></a>[<span data-ttu-id="d106b-141">C#</span><span class="sxs-lookup"><span data-stu-id="d106b-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bundle-metadata-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d106b-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d106b-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bundle-metadata-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d106b-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d106b-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bundle-metadata-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d106b-144">Java</span><span class="sxs-lookup"><span data-stu-id="d106b-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-bundle-metadata-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d106b-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="d106b-145">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "0123456789abc",
  "name": "My Photo Album Bundle",
  "eTag": "etag",
  "cTag": "etag",
  "createdBy": { "user": { "id": "1234", "displayName": "Ryan Gregg" } },
  "createdDateTime": "datetime",
  "lastModifiedBy": { "user": { "id": "1234", "displayName": "Ryan Gregg" } },
  "lastModifiedDateTime": "datetime",
  "size": 1234,
  "webUrl": "http://onedrive.com/...",
  "bundle": {
    "childCount": 4,
     "album": { }
  }
}
```

<span data-ttu-id="d106b-146">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d106b-146">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d106b-147">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d106b-147">All the properties will be returned from an actual call.</span></span>

### <a name="example-2-get-a-bundle-and-its-children-in-a-single-call"></a><span data-ttu-id="d106b-148">Exemplo 2: obter um pacote e seus filhos em uma única chamada</span><span class="sxs-lookup"><span data-stu-id="d106b-148">Example 2: Get a bundle and its children in a single call</span></span>

<span data-ttu-id="d106b-149">Você pode usar o [`expand`](/graph/query-parameters) parâmetro de cadeia de caracteres de consulta para incluir os filhos de um pacote na mesma chamada que recupera os metadados de um pacote.</span><span class="sxs-lookup"><span data-stu-id="d106b-149">You can use the [`expand`](/graph/query-parameters) query string parameter to include the children of a bundle in the same call as retrieving the metadata of a bundle.</span></span>

#### <a name="request"></a><span data-ttu-id="d106b-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d106b-150">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="d106b-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="d106b-151">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-bundle-and-children" } -->

```msgraph-interactive
GET https://graph.microsoft.com/beta/drive/items/{bundle-id}?expand=children
```
# <a name="c"></a>[<span data-ttu-id="d106b-152">C#</span><span class="sxs-lookup"><span data-stu-id="d106b-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bundle-and-children-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d106b-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d106b-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bundle-and-children-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d106b-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d106b-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bundle-and-children-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d106b-155">Java</span><span class="sxs-lookup"><span data-stu-id="d106b-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-bundle-and-children-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d106b-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="d106b-156">Response</span></span>

<span data-ttu-id="d106b-157">Essa chamada retornará os metadados do pacote e uma lista de filhos do pacote.</span><span class="sxs-lookup"><span data-stu-id="d106b-157">This call will return the bundle metadata and a list of children of the bundle.</span></span>
<span data-ttu-id="d106b-158">Se o pacote não tiver filhos, retornará uma coleção vazia.</span><span class="sxs-lookup"><span data-stu-id="d106b-158">If the bundle has no children, it will return an empty collection.</span></span>

<span data-ttu-id="d106b-159">Se o número de filhos no pacote for maior que o tamanho de página padrão, a propriedade **Children@odata. nextLink** será retornada com uma URL que pode ser usada para solicitar a próxima página de filhos no pacote.</span><span class="sxs-lookup"><span data-stu-id="d106b-159">If the number of children in the bundle is greater than the default page size, the **children@odata.nextLink** property will be returned with a URL that can be used to request the next page of children in the bundle.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "101230100alkc",
  "name": "My Cool Day at the Beach",
  "children": [
    { "id": "120100abab", "name": "image1.jpg", "file": {} },
    { "id": "120100abo1", "name": "image2.jpg", "file": {} }
  ],
  "children@odata.nextLink": "https://api.onedrive.com/v1.0/..."
}
```

<span data-ttu-id="d106b-160">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d106b-160">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d106b-161">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d106b-161">All the properties will be returned from an actual call.</span></span>


[pacote]: ../resources/bundle.md
[bundle]: ../resources/bundle.md
[driveItem]: ../resources/driveItem.md
[error-response]: /graph/errors
[odata-parameters]: /graph/query-parameters


<!-- {
  "type": "#page.annotation",
  "description": "Retrieve metadata about a bundle and its children in OneDrive",
  "keywords": "retrieve,item,bundle,metadata",
  "section": "documentation",
  "tocPath": "Bundles/Get Bundle Metadata"
} -->


