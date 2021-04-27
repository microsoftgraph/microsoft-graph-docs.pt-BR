---
author: JeremyKelley
title: Obter pacote
description: Obter um pacote de driveItems
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: b6f1619bbb169a92841d3999c43603860c0038fd
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047788"
---
# <a name="get-bundle"></a><span data-ttu-id="c2960-103">Obter pacote</span><span class="sxs-lookup"><span data-stu-id="c2960-103">Get bundle</span></span>

<span data-ttu-id="c2960-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c2960-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c2960-105">Recupere os metadados de [um pacote][] com base na ID exclusiva do pacote.</span><span class="sxs-lookup"><span data-stu-id="c2960-105">Retrieve the metadata for a [bundle][] based on the bundle's unique ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="c2960-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c2960-106">Permissions</span></span>

<span data-ttu-id="c2960-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c2960-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c2960-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c2960-109">Permission type</span></span>      | <span data-ttu-id="c2960-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c2960-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c2960-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c2960-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c2960-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c2960-112">Not supported.</span></span>                             |
|<span data-ttu-id="c2960-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c2960-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c2960-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2960-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="c2960-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c2960-115">Application</span></span>          | <span data-ttu-id="c2960-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c2960-116">Not supported.</span></span>                                           |

## <a name="http-request"></a><span data-ttu-id="c2960-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c2960-117">HTTP request</span></span>

```http
GET /drive/bundles/{bundle-id}
GET /drive/items/{bundle-id}
```

<span data-ttu-id="c2960-118">Como os pacotes são itens, você pode usar a coleção **items** para retornar metadados sobre um pacote.</span><span class="sxs-lookup"><span data-stu-id="c2960-118">Because bundles are items, you can use the **items** collection to return metadata about a bundle.</span></span>
<span data-ttu-id="c2960-119">Você também pode usar a coleção **bundles** como uma conveniência para garantir que você está recebendo um pacote em resposta.</span><span class="sxs-lookup"><span data-stu-id="c2960-119">You can also use the **bundles** collection as a convenience to ensure you're getting a bundle in response.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="c2960-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c2960-120">Optional query parameters</span></span>

<span data-ttu-id="c2960-121">Você pode usar os [parâmetros de consulta OData][odata-parameters] para restringir a forma dos objetos retornados dessa chamada.</span><span class="sxs-lookup"><span data-stu-id="c2960-121">You can use the [OData query parameters][odata-parameters] to restrict the shape of the objects returned from this call.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c2960-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c2960-122">Request headers</span></span>
| <span data-ttu-id="c2960-123">Nome</span><span class="sxs-lookup"><span data-stu-id="c2960-123">Name</span></span>          | <span data-ttu-id="c2960-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="c2960-124">Description</span></span>  |
|:------------- |:------------ |
| <span data-ttu-id="c2960-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="c2960-125">Authorization</span></span> | <span data-ttu-id="c2960-p103">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c2960-p103">Bearer \{token\}. Required.</span></span> |
| <span data-ttu-id="c2960-128">if-none-match</span><span class="sxs-lookup"><span data-stu-id="c2960-128">if-none-match</span></span> | <span data-ttu-id="c2960-129">eTag.</span><span class="sxs-lookup"><span data-stu-id="c2960-129">eTag.</span></span> <span data-ttu-id="c2960-130">Opcional.</span><span class="sxs-lookup"><span data-stu-id="c2960-130">Optional.</span></span> <span data-ttu-id="c2960-131">Se este cabeçalho de solicitação estiver incluso e a eTag (ou cTag) fornecida corresponder à marca atual do arquivo, uma resposta `HTTP 304 Not Modified` será retornada.</span><span class="sxs-lookup"><span data-stu-id="c2960-131">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span>

## <a name="request-body"></a><span data-ttu-id="c2960-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c2960-132">Request body</span></span>

<span data-ttu-id="c2960-133">Não forneça um corpo de solicitação com esse método.</span><span class="sxs-lookup"><span data-stu-id="c2960-133">Do not supply a request body with this method.</span></span>

## <a name="response"></a><span data-ttu-id="c2960-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="c2960-134">Response</span></span>

<span data-ttu-id="c2960-135">Se tiver êxito, este método retornará [um driveItem][driveItem] resource with the [bundle][bundle] no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c2960-135">If successful, this method returns a [driveItem][driveItem] resource with the [bundle][bundle] in the response body.</span></span>

<span data-ttu-id="c2960-136">Leia o tópico [Respostas de erro][error-response] para obter mais informações sobre como os erros são retornados.</span><span class="sxs-lookup"><span data-stu-id="c2960-136">Read the [Error Responses][error-response] topic for more info about how errors are returned.</span></span>

## <a name="examples"></a><span data-ttu-id="c2960-137">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c2960-137">Examples</span></span>

### <a name="example-1-get-a-bundle"></a><span data-ttu-id="c2960-138">Exemplo 1: Obter um pacote</span><span class="sxs-lookup"><span data-stu-id="c2960-138">Example 1: Get a bundle</span></span>

#### <a name="request"></a><span data-ttu-id="c2960-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c2960-139">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="c2960-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="c2960-140">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-bundle-metadata" } -->

```msgraph-interactive
GET https://graph.microsoft.com/beta/drive/bundles/{bundle-id}
```
# <a name="c"></a>[<span data-ttu-id="c2960-141">C#</span><span class="sxs-lookup"><span data-stu-id="c2960-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bundle-metadata-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c2960-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c2960-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bundle-metadata-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c2960-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c2960-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bundle-metadata-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c2960-144">Java</span><span class="sxs-lookup"><span data-stu-id="c2960-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-bundle-metadata-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c2960-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="c2960-145">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```http
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

<span data-ttu-id="c2960-146">O objeto de resposta mostrado aqui pode ser reduzido para facilitar a leitura.</span><span class="sxs-lookup"><span data-stu-id="c2960-146">The response object shown here might be shortened for readability.</span></span>

### <a name="example-2-get-a-bundle-and-its-children-in-a-single-call"></a><span data-ttu-id="c2960-147">Exemplo 2: Obter um pacote e seus filhos em uma única chamada</span><span class="sxs-lookup"><span data-stu-id="c2960-147">Example 2: Get a bundle and its children in a single call</span></span>

<span data-ttu-id="c2960-148">Você pode usar o parâmetro de cadeia de caracteres de consulta para incluir os filhos de um pacote na mesma chamada que recuperar os [`expand`](/graph/query-parameters) metadados de um pacote.</span><span class="sxs-lookup"><span data-stu-id="c2960-148">You can use the [`expand`](/graph/query-parameters) query string parameter to include the children of a bundle in the same call as retrieving the metadata of a bundle.</span></span>

#### <a name="request"></a><span data-ttu-id="c2960-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c2960-149">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="c2960-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="c2960-150">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-bundle-and-children" } -->

```msgraph-interactive
GET https://graph.microsoft.com/beta/drive/items/{bundle-id}?expand=children
```
# <a name="c"></a>[<span data-ttu-id="c2960-151">C#</span><span class="sxs-lookup"><span data-stu-id="c2960-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bundle-and-children-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c2960-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c2960-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bundle-and-children-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c2960-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c2960-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bundle-and-children-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c2960-154">Java</span><span class="sxs-lookup"><span data-stu-id="c2960-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-bundle-and-children-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c2960-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="c2960-155">Response</span></span>

<span data-ttu-id="c2960-156">Essa chamada retornará os metadados do pacote e uma lista de filhos do pacote.</span><span class="sxs-lookup"><span data-stu-id="c2960-156">This call will return the bundle metadata and a list of children of the bundle.</span></span>
<span data-ttu-id="c2960-157">Se o pacote não tiver filhos, ele retornará uma coleção vazia.</span><span class="sxs-lookup"><span data-stu-id="c2960-157">If the bundle has no children, it will return an empty collection.</span></span>

<span data-ttu-id="c2960-158">Se o número de filhos no pacote for maior do que o tamanho padrão da página, a propriedade **children@odata.nextLink** será retornada com uma URL que pode ser usada para solicitar a próxima página de filhos no pacote.</span><span class="sxs-lookup"><span data-stu-id="c2960-158">If the number of children in the bundle is greater than the default page size, the **children@odata.nextLink** property will be returned with a URL that can be used to request the next page of children in the bundle.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```http
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

<span data-ttu-id="c2960-159">O objeto de resposta mostrado aqui pode ser reduzido para facilitar a leitura.</span><span class="sxs-lookup"><span data-stu-id="c2960-159">The response object shown here might be shortened for readability.</span></span>


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
  "tocPath&quot;: &quot;Bundles/Get Bundle Metadata"
} -->


