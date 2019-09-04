---
author: JeremyKelley
ms.author: jeremyke
title: Obter pacote
description: Obter um pacote de driveItems
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 495b4b5487ce413c682bbe81589f920132755c64
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36718790"
---
# <a name="get-bundle"></a><span data-ttu-id="def19-103">Obter pacote</span><span class="sxs-lookup"><span data-stu-id="def19-103">Get bundle</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="def19-104">Recupere os metadados de um [pacote][] com base na ID exclusiva do pacote.</span><span class="sxs-lookup"><span data-stu-id="def19-104">Retrieve the metadata for a [bundle][] based on the bundle's unique ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="def19-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="def19-105">Permissions</span></span>

<span data-ttu-id="def19-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="def19-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="def19-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="def19-108">Permission type</span></span>      | <span data-ttu-id="def19-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="def19-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="def19-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="def19-110">Delegated (work or school account)</span></span> | <span data-ttu-id="def19-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="def19-111">Not supported.</span></span>                             |
|<span data-ttu-id="def19-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="def19-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="def19-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="def19-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="def19-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="def19-114">Application</span></span>          | <span data-ttu-id="def19-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="def19-115">Not supported.</span></span>                                           |

## <a name="http-request"></a><span data-ttu-id="def19-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="def19-116">HTTP request</span></span>

```http
GET /drive/bundles/{bundle-id}
GET /drive/items/{bundle-id}
```

<span data-ttu-id="def19-117">Como os pacotes são itens, você pode usar a \*\*\*\* coleção Items para retornar metadados sobre um pacote.</span><span class="sxs-lookup"><span data-stu-id="def19-117">Because bundles are items, you can use the **items** collection to return metadata about a bundle.</span></span>
<span data-ttu-id="def19-118">Você também pode usar a coleção de **pacotes** como uma conveniência para garantir que você esteja obtendo um pacote em resposta.</span><span class="sxs-lookup"><span data-stu-id="def19-118">You can also use the **bundles** collection as a convenience to ensure you're getting a bundle in response.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="def19-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="def19-119">Optional query parameters</span></span>

<span data-ttu-id="def19-120">Você pode usar os [parâmetros de consulta OData][odata-parameters] para restringir a forma dos objetos retornados dessa chamada.</span><span class="sxs-lookup"><span data-stu-id="def19-120">You can use the [OData query parameters][odata-parameters] to restrict the shape of the objects returned from this call.</span></span>

## <a name="request-headers"></a><span data-ttu-id="def19-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="def19-121">Request headers</span></span>
| <span data-ttu-id="def19-122">Nome</span><span class="sxs-lookup"><span data-stu-id="def19-122">Name</span></span>          | <span data-ttu-id="def19-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="def19-123">Description</span></span>  |
|:------------- |:------------ |
| <span data-ttu-id="def19-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="def19-124">Authorization</span></span> | <span data-ttu-id="def19-125">\{token\} de portador.</span><span class="sxs-lookup"><span data-stu-id="def19-125">Bearer \{token\}.</span></span> <span data-ttu-id="def19-126">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="def19-126">Required.</span></span> |
| <span data-ttu-id="def19-127">if-none-match</span><span class="sxs-lookup"><span data-stu-id="def19-127">if-none-match</span></span> | <span data-ttu-id="def19-128">ETag.</span><span class="sxs-lookup"><span data-stu-id="def19-128">eTag.</span></span> <span data-ttu-id="def19-129">Opcional.</span><span class="sxs-lookup"><span data-stu-id="def19-129">Optional.</span></span> <span data-ttu-id="def19-130">Se este cabeçalho de solicitação estiver incluso e a eTag (ou cTag) fornecida corresponder à marca atual do arquivo, uma resposta `HTTP 304 Not Modified` será retornada.</span><span class="sxs-lookup"><span data-stu-id="def19-130">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span>

## <a name="request-body"></a><span data-ttu-id="def19-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="def19-131">Request body</span></span>

<span data-ttu-id="def19-132">Não forneça um corpo de solicitação com esse método.</span><span class="sxs-lookup"><span data-stu-id="def19-132">Do not supply a request body with this method.</span></span>

## <a name="response"></a><span data-ttu-id="def19-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="def19-133">Response</span></span>

<span data-ttu-id="def19-134">Se bem-sucedido, este método retorna um [driveItem][driveItem] resource with the [bundle][bundle] no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="def19-134">If successful, this method returns a [driveItem][driveItem] resource with the [bundle][bundle] in the response body.</span></span>

<span data-ttu-id="def19-135">Leia o tópico [respostas de erro][error-response] para obter mais informações sobre como os erros são retornados.</span><span class="sxs-lookup"><span data-stu-id="def19-135">Read the [Error Responses][error-response] topic for more info about how errors are returned.</span></span>

## <a name="examples"></a><span data-ttu-id="def19-136">Exemplos</span><span class="sxs-lookup"><span data-stu-id="def19-136">Examples</span></span>

### <a name="example-1-get-a-bundle"></a><span data-ttu-id="def19-137">Exemplo 1: obter um pacote</span><span class="sxs-lookup"><span data-stu-id="def19-137">Example 1: Get a bundle</span></span>

#### <a name="request"></a><span data-ttu-id="def19-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="def19-138">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="def19-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="def19-139">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-bundle-metadata" } -->

```msgraph-interactive
GET https://graph.microsoft.com/beta/drive/bundles/{bundle-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="def19-140">C#</span><span class="sxs-lookup"><span data-stu-id="def19-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bundle-metadata-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="def19-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="def19-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bundle-metadata-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="def19-142">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="def19-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bundle-metadata-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="def19-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="def19-143">Response</span></span>

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

<span data-ttu-id="def19-144">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="def19-144">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="def19-145">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="def19-145">All the properties will be returned from an actual call.</span></span>

### <a name="example-2-get-a-bundle-and-its-children-in-a-single-call"></a><span data-ttu-id="def19-146">Exemplo 2: obter um pacote e seus filhos em uma única chamada</span><span class="sxs-lookup"><span data-stu-id="def19-146">Example 2: Get a bundle and its children in a single call</span></span>

<span data-ttu-id="def19-147">Você pode usar o [`expand`](/graph/query-parameters) parâmetro de cadeia de caracteres de consulta para incluir os filhos de um pacote na mesma chamada que recupera os metadados de um pacote.</span><span class="sxs-lookup"><span data-stu-id="def19-147">You can use the [`expand`](/graph/query-parameters) query string parameter to include the children of a bundle in the same call as retrieving the metadata of a bundle.</span></span>

#### <a name="request"></a><span data-ttu-id="def19-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="def19-148">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="def19-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="def19-149">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-bundle-and-children" } -->

```msgraph-interactive
GET https://graph.microsoft.com/beta/drive/items/{bundle-id}?expand=children
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="def19-150">C#</span><span class="sxs-lookup"><span data-stu-id="def19-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bundle-and-children-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="def19-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="def19-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bundle-and-children-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="def19-152">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="def19-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bundle-and-children-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="def19-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="def19-153">Response</span></span>

<span data-ttu-id="def19-154">Essa chamada retornará os metadados do pacote e uma lista de filhos do pacote.</span><span class="sxs-lookup"><span data-stu-id="def19-154">This call will return the bundle metadata and a list of children of the bundle.</span></span>
<span data-ttu-id="def19-155">Se o pacote não tiver filhos, retornará uma coleção vazia.</span><span class="sxs-lookup"><span data-stu-id="def19-155">If the bundle has no children, it will return an empty collection.</span></span>

<span data-ttu-id="def19-156">Se o número de filhos no pacote for maior que o tamanho de página padrão, a propriedade **Children @ OData. nextLink** será retornada com uma URL que pode ser usada para solicitar a próxima página de filhos no pacote.</span><span class="sxs-lookup"><span data-stu-id="def19-156">If the number of children in the bundle is greater than the default page size, the **children@odata.nextLink** property will be returned with a URL that can be used to request the next page of children in the bundle.</span></span>

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

<span data-ttu-id="def19-157">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="def19-157">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="def19-158">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="def19-158">All the properties will be returned from an actual call.</span></span>


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
