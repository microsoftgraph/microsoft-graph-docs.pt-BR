---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Recuperar miniaturas de um arquivo ou pasta
localization_priority: Normal
ms.prod: sharepoint
description: Recupere uma coleção de recursos ThumbnailSet para um recurso DriveItem.
doc_type: apiPageType
ms.openlocfilehash: 51fc9302ab356ead935aabed24bbe76490fc75f1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42517710"
---
# <a name="list-thumbnails-for-a-driveitem"></a><span data-ttu-id="a05d2-103">Listar miniaturas para um DriveItem</span><span class="sxs-lookup"><span data-stu-id="a05d2-103">List thumbnails for a DriveItem</span></span>

<span data-ttu-id="a05d2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a05d2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a05d2-105">Recupere uma coleção de recursos [ThumbnailSet](../resources/thumbnailset.md) para um recurso [DriveItem](../resources/driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="a05d2-105">Retrieve a collection of [ThumbnailSet](../resources/thumbnailset.md) resources for a [DriveItem](../resources/driveitem.md) resource.</span></span>

<span data-ttu-id="a05d2-p101">Um DriveItem pode ser representado por zero ou mais recursos [ThumbnailSet](../resources/thumbnailset.md). Cada **thumbnailSet** pode ter um ou mais objetos [**thumbnail**](../resources/thumbnail.md), que são imagens que representam o item. Por exemplo, um **thumbnailSet** podem incluir objetos **thumbnail**, como objetos comuns que incluem `small`, `medium` ou `large`.</span><span class="sxs-lookup"><span data-stu-id="a05d2-p101">A DriveItem can be represented by zero or more [ThumbnailSet](../resources/thumbnailset.md) resources. Each **thumbnailSet** can have one or more [**thumbnail**](../resources/thumbnail.md) objects, which are images that represent the item. For example, a **thumbnailSet** may include **thumbnail** objects, such as common ones including `small`, `medium`, or `large`.</span></span>

<span data-ttu-id="a05d2-p102">Há várias maneiras de trabalhar com miniaturas no OneDrive. Veja a seguir as mais comuns:</span><span class="sxs-lookup"><span data-stu-id="a05d2-p102">There are many ways to work with thumbnails on OneDrive. Here are the most common ones:</span></span>

* <span data-ttu-id="a05d2-111">Enumerar miniaturas disponíveis para um item</span><span class="sxs-lookup"><span data-stu-id="a05d2-111">Enumerate available thumbnails for an item</span></span>
* <span data-ttu-id="a05d2-112">Recuperar uma única miniatura para um item</span><span class="sxs-lookup"><span data-stu-id="a05d2-112">Retrieve a single thumbnail for an item</span></span>
* <span data-ttu-id="a05d2-113">Recuperar o conteúdo da miniatura</span><span class="sxs-lookup"><span data-stu-id="a05d2-113">Retrieve thumbnail content</span></span>
* <span data-ttu-id="a05d2-114">Recuperar miniaturas de vários itens em uma única solicitação</span><span class="sxs-lookup"><span data-stu-id="a05d2-114">Retrieve thumbnails for multiple items in a single request</span></span>
* <span data-ttu-id="a05d2-115">Recuperar tamanhos personalizados de miniaturas</span><span class="sxs-lookup"><span data-stu-id="a05d2-115">Retrieve custom thumbnail sizes</span></span>
* <span data-ttu-id="a05d2-116">Carregar uma miniatura personalizada para um item</span><span class="sxs-lookup"><span data-stu-id="a05d2-116">Upload a custom thumbnail for an item</span></span>
* <span data-ttu-id="a05d2-117">Determinar se uma miniatura personalizada carregada existe</span><span class="sxs-lookup"><span data-stu-id="a05d2-117">Determine if a custom uploaded thumbnail exists</span></span>

## <a name="permissions"></a><span data-ttu-id="a05d2-118">Permissões</span><span class="sxs-lookup"><span data-stu-id="a05d2-118">Permissions</span></span>

<span data-ttu-id="a05d2-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a05d2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a05d2-121">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a05d2-121">Permission type</span></span>      | <span data-ttu-id="a05d2-122">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a05d2-122">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a05d2-123">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a05d2-123">Delegated (work or school account)</span></span> | <span data-ttu-id="a05d2-124">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a05d2-124">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="a05d2-125">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a05d2-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a05d2-126">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a05d2-126">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="a05d2-127">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a05d2-127">Application</span></span> | <span data-ttu-id="a05d2-128">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a05d2-128">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a05d2-129">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a05d2-129">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/thumbnails
GET /groups/{group-id}/drive/items/{item-id}/thumbnails
GET /me/drive/items/{item-id}/thumbnails
GET /sites/{site-id}/drive/items/{item-id}/thumbnails
GET /users/{user-id}/drive/items/{item-id}/thumbnails
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a05d2-130">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a05d2-130">Optional query parameters</span></span>

<span data-ttu-id="a05d2-131">Este método oferece suporte ao [Parâmetro de consulta OData](/graph/query-parameters) `$select` para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a05d2-131">This method supports the `$select` [OData puery parameter](/graph/query-parameters) to customize the response.</span></span>

## <a name="response"></a><span data-ttu-id="a05d2-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="a05d2-132">Response</span></span>

<span data-ttu-id="a05d2-133">Se for bem-sucedido, esse método retornará um código de resposta `200 OK` e uma coleção de objetos [ThumbnailSet](../resources/thumbnailset.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a05d2-133">If successful, this method returns a `200 OK` response code and collection of [ThumbnailSet](../resources/thumbnailset.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a05d2-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a05d2-134">Example</span></span>

<span data-ttu-id="a05d2-135">Veja um exemplo da solicitação que recupera as miniaturas disponíveis de um item no OneDrive atual do usuário.</span><span class="sxs-lookup"><span data-stu-id="a05d2-135">Here is an example of the request which retrieves available thumbnails for an item in the current user's OneDrive.</span></span>


# <a name="http"></a>[<span data-ttu-id="a05d2-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="a05d2-136">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "enum-item-thumbnails", "scopes": "files.read", "tags": "service.graph" } -->

```msgraph-interactive
GET /me/drive/items/{item-id}/thumbnails
```
# <a name="c"></a>[<span data-ttu-id="a05d2-137">C#</span><span class="sxs-lookup"><span data-stu-id="a05d2-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/enum-item-thumbnails-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a05d2-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a05d2-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/enum-item-thumbnails-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a05d2-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a05d2-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/enum-item-thumbnails-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a05d2-140">Java</span><span class="sxs-lookup"><span data-stu-id="a05d2-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/enum-item-thumbnails-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="a05d2-141">Isto retorna uma matriz de **thumbnailSets** disponíveis para o item.</span><span class="sxs-lookup"><span data-stu-id="a05d2-141">This returns an array of available **thumbnailSets** for the item.</span></span> <span data-ttu-id="a05d2-142">Qualquer item em uma unidade pode ter zero ou mais miniaturas.</span><span class="sxs-lookup"><span data-stu-id="a05d2-142">Any item in a drive can have zero or more thumbnails.</span></span>

<span data-ttu-id="a05d2-p105">**Observação:** Você pode usar o parâmetro da cadeia de caracteres de consulta _select_ para controlar quais tamanhos de miniatura são retornados no **ThumbnailSet**. Por exemplo, `/thumbnails?select=medium` recupera somente miniaturas de tamanho médio.</span><span class="sxs-lookup"><span data-stu-id="a05d2-p105">**Note:** You can use the _select_ query string parameter to control which thumbnail sizes are returned in the **ThumbnailSet**. For example, `/thumbnails?select=medium` retrieves only the medium sized thumbnails.</span></span>


### <a name="response"></a><span data-ttu-id="a05d2-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="a05d2-145">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.thumbnailSet)" } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "0",
      "small": { "height": 64, "width": 96, "url": "https://sn3302files..."},
      "medium": { "height": 117, "width": 176, "url": "https://sn3302files..."},
      "large": { "height": 533, "width": 800, "url": "https://sn3302files..."}
    }
  ]
}
```

## <a name="get-a-single-thumbnail"></a><span data-ttu-id="a05d2-146">Obter uma única miniatura</span><span class="sxs-lookup"><span data-stu-id="a05d2-146">Get a single thumbnail</span></span>

<span data-ttu-id="a05d2-147">Recupere os metadados de uma única miniatura e tamanho tratando-os diretamente em uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="a05d2-147">Retrieve the metadata for a single thumbnail and size by addressing it directly in a request.</span></span>

### <a name="http-request"></a><span data-ttu-id="a05d2-148">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a05d2-148">HTTP request</span></span>


# <a name="http"></a>[<span data-ttu-id="a05d2-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="a05d2-149">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-one-thumbnail", "scopes": "files.read", "tags": "service.graph" } -->

```msgraph-interactive
GET /me/drive/items/{item-id}/thumbnails/{thumb-id}/{size}
```
# <a name="c"></a>[<span data-ttu-id="a05d2-150">C#</span><span class="sxs-lookup"><span data-stu-id="a05d2-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-one-thumbnail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a05d2-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a05d2-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-one-thumbnail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a05d2-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a05d2-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-one-thumbnail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a05d2-153">Java</span><span class="sxs-lookup"><span data-stu-id="a05d2-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-one-thumbnail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="path-parameters"></a><span data-ttu-id="a05d2-154">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="a05d2-154">Path parameters</span></span>

| <span data-ttu-id="a05d2-155">Name</span><span class="sxs-lookup"><span data-stu-id="a05d2-155">Name</span></span>         | <span data-ttu-id="a05d2-156">Tipo</span><span class="sxs-lookup"><span data-stu-id="a05d2-156">Type</span></span>   | <span data-ttu-id="a05d2-157">Descrição</span><span class="sxs-lookup"><span data-stu-id="a05d2-157">Description</span></span>                                                                              |
|:-------------|:-------|:-----------------------------------------------------------------------------------------|
| <span data-ttu-id="a05d2-158">**item-id**</span><span class="sxs-lookup"><span data-stu-id="a05d2-158">**item-id**</span></span>  | <span data-ttu-id="a05d2-159">string</span><span class="sxs-lookup"><span data-stu-id="a05d2-159">string</span></span> | <span data-ttu-id="a05d2-160">O identificador exclusivo do item referenciado.</span><span class="sxs-lookup"><span data-stu-id="a05d2-160">The unique identifier for the item referenced.</span></span>                                           |
| <span data-ttu-id="a05d2-161">**thumb-id**</span><span class="sxs-lookup"><span data-stu-id="a05d2-161">**thumb-id**</span></span> | <span data-ttu-id="a05d2-162">number</span><span class="sxs-lookup"><span data-stu-id="a05d2-162">number</span></span> | <span data-ttu-id="a05d2-p106">O índice da miniatura, geralmente de 0 a 4. Se houver uma miniatura personalizada, seu índice será 0.</span><span class="sxs-lookup"><span data-stu-id="a05d2-p106">The index of the thumbnail, usually 0-4. If there is a custom thumbnail, its index is 0.</span></span> |
| <span data-ttu-id="a05d2-165">**size**</span><span class="sxs-lookup"><span data-stu-id="a05d2-165">**size**</span></span>     | <span data-ttu-id="a05d2-166">string</span><span class="sxs-lookup"><span data-stu-id="a05d2-166">string</span></span> | <span data-ttu-id="a05d2-167">O tamanho da miniatura solicitada.</span><span class="sxs-lookup"><span data-stu-id="a05d2-167">The size of the thumbnail requested.</span></span> <span data-ttu-id="a05d2-168">Pode ter um dos tamanhos padrão listados abaixo, ou um tamanho personalizado.</span><span class="sxs-lookup"><span data-stu-id="a05d2-168">This can be one of the standard sizes listed below or a custom size.</span></span> |

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.thumbnail" } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "width": 100,
  "height": 100,
  "url": "https://onedrive.com/asd123a/asdjlkasjdkasdjlk.jpg"
}
```

## <a name="retrieve-thumbnail-binary-content"></a><span data-ttu-id="a05d2-169">Recuperar o conteúdo binário da miniatura</span><span class="sxs-lookup"><span data-stu-id="a05d2-169">Retrieve thumbnail binary content</span></span>

<span data-ttu-id="a05d2-170">Você pode recuperar diretamente o conteúdo da miniatura solicitando a propriedade **content** dessa miniatura.</span><span class="sxs-lookup"><span data-stu-id="a05d2-170">You can directly retrieve the content of the thumbnail by requesting the **content** property of the thumbnail.</span></span>

### <a name="http-request"></a><span data-ttu-id="a05d2-171">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a05d2-171">HTTP request</span></span>


# <a name="http"></a>[<span data-ttu-id="a05d2-172">HTTP</span><span class="sxs-lookup"><span data-stu-id="a05d2-172">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name":"get-thumbnail-content", "scopes": "files.read", "tags": "service.graph" } -->

```msgraph-interactive
GET /me/drive/items/{item-id}/thumbnails/{thumb-id}/{size}/content
```
# <a name="c"></a>[<span data-ttu-id="a05d2-173">C#</span><span class="sxs-lookup"><span data-stu-id="a05d2-173">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-thumbnail-content-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a05d2-174">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a05d2-174">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-thumbnail-content-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a05d2-175">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a05d2-175">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-thumbnail-content-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a05d2-176">Java</span><span class="sxs-lookup"><span data-stu-id="a05d2-176">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-thumbnail-content-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a05d2-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="a05d2-177">Response</span></span>

<span data-ttu-id="a05d2-178">O serviço responde com um redirecionamento para a URL da miniatura.</span><span class="sxs-lookup"><span data-stu-id="a05d2-178">The service responds with a redirect to the thumbnail URL.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```

<span data-ttu-id="a05d2-179">URLs de miniaturas são seguras em cache.</span><span class="sxs-lookup"><span data-stu-id="a05d2-179">Thumbnail URLs are cache-safe.</span></span> <span data-ttu-id="a05d2-180">A URL mudará se o item for alterado de uma maneira que exigir que uma nova miniatura seja gerada.</span><span class="sxs-lookup"><span data-stu-id="a05d2-180">The URL will change, if the item changes in a way that requires a new thumbnail to be generated.</span></span>


## <a name="getting-thumbnails-while-listing-driveitems"></a><span data-ttu-id="a05d2-181">Obter miniaturas ao listar DriveItems</span><span class="sxs-lookup"><span data-stu-id="a05d2-181">Getting thumbnails while listing DriveItems</span></span>

<span data-ttu-id="a05d2-182">Se você estiver recuperando uma lista de recursos DriveItem para exibição, use o parâmetro de cadeia de consulta _$expand_ para incluir as miniaturas para esses recursos.</span><span class="sxs-lookup"><span data-stu-id="a05d2-182">If you are retrieving a list of DriveItem resources to display, you can use the _$expand_ query string parameter to also include the thumbnails for those resources.</span></span>
<span data-ttu-id="a05d2-183">Isso permite que seu aplicativo recupere miniaturas e itens em uma única solicitação, em vez de emitir muitas solicitações.</span><span class="sxs-lookup"><span data-stu-id="a05d2-183">This enables your app to retrieve thumbnails and items in a single request, instead of issuing many requests.</span></span>

### <a name="http-request"></a><span data-ttu-id="a05d2-184">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a05d2-184">HTTP request</span></span>


# <a name="http"></a>[<span data-ttu-id="a05d2-185">HTTP</span><span class="sxs-lookup"><span data-stu-id="a05d2-185">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name":"get-thumbnail-while-listing", "scopes": "files.read", "tags": "service.graph" } -->

```msgraph-interactive
GET /me/drive/items/{item-id}/children?$expand=thumbnails
```
# <a name="c"></a>[<span data-ttu-id="a05d2-186">C#</span><span class="sxs-lookup"><span data-stu-id="a05d2-186">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-thumbnail-while-listing-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a05d2-187">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a05d2-187">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-thumbnail-while-listing-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a05d2-188">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a05d2-188">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-thumbnail-while-listing-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a05d2-189">Java</span><span class="sxs-lookup"><span data-stu-id="a05d2-189">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-thumbnail-while-listing-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a05d2-190">Resposta</span><span class="sxs-lookup"><span data-stu-id="a05d2-190">Response</span></span>

<span data-ttu-id="a05d2-191">As respostas do serviço com a lista de DriveItems e suas miniaturas.</span><span class="sxs-lookup"><span data-stu-id="a05d2-191">The service responses with the list of DriveItems and their thumbnails.</span></span>

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.driveItem)", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "182331E8-2788-4932-B52A-A6550577043F",
      "name": "my photo.jpg",
      "thumbnails": [
        {
          "small": { "width": 96,
                     "height": 96,
                     "url": "https://sn3302files..."
                   }
        }
      ]
    },
    {
      "id": "2D223953-A56B-4D9B-ADF3-13E7820673A2",
      "name": "presentation.pptx",
      "thumbnails": [
        {
          "small": { "width": 96,
                     "height": 96,
                     "url": "https://sn3302files..."
                   }
        }
      ]
    }
  ]
}
```

## <a name="size-options"></a><span data-ttu-id="a05d2-192">Opções de tamanho</span><span class="sxs-lookup"><span data-stu-id="a05d2-192">Size options</span></span>

<span data-ttu-id="a05d2-p110">Essa tabela define os possíveis tamanhos de miniaturas. Embora você possa solicitar qualquer tamanho de miniatura arbitrário, os valores definidos provavelmente existem e retornam um valor rapidamente:</span><span class="sxs-lookup"><span data-stu-id="a05d2-p110">This table defines the possible thumbnail sizes. While you can request any arbitrary thumbnail size, the defined values are likely to exist and return a value quickly:</span></span>

| <span data-ttu-id="a05d2-195">Nome</span><span class="sxs-lookup"><span data-stu-id="a05d2-195">Name</span></span>           | <span data-ttu-id="a05d2-196">Resolução</span><span class="sxs-lookup"><span data-stu-id="a05d2-196">Resolution</span></span>  | <span data-ttu-id="a05d2-197">Taxa de proporção</span><span class="sxs-lookup"><span data-stu-id="a05d2-197">Aspect Ratio</span></span> | <span data-ttu-id="a05d2-198">Descrição</span><span class="sxs-lookup"><span data-stu-id="a05d2-198">Description</span></span>                                                          |
|:---------------|:------------|:-------------|:---------------------------------------------------------------------|
| `small`        | <span data-ttu-id="a05d2-199">96 mais longa</span><span class="sxs-lookup"><span data-stu-id="a05d2-199">96 longest</span></span>  | <span data-ttu-id="a05d2-200">Original</span><span class="sxs-lookup"><span data-stu-id="a05d2-200">Original</span></span>     | <span data-ttu-id="a05d2-201">Miniatura pequena e altamente compactada, recortada em uma taxa de proporção quadrada.</span><span class="sxs-lookup"><span data-stu-id="a05d2-201">Small, highly compressed thumbnail cropped to a square aspect ratio.</span></span> |
| `medium`       | <span data-ttu-id="a05d2-202">176 mais longa</span><span class="sxs-lookup"><span data-stu-id="a05d2-202">176 longest</span></span> | <span data-ttu-id="a05d2-203">Original</span><span class="sxs-lookup"><span data-stu-id="a05d2-203">Original</span></span>     | <span data-ttu-id="a05d2-204">Recortada no tamanho do item padrão para o modo de exibição de Web do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="a05d2-204">Cropped to the standard item size for the OneDrive web view.</span></span>         |
| `large`        | <span data-ttu-id="a05d2-205">800 mais longa</span><span class="sxs-lookup"><span data-stu-id="a05d2-205">800 longest</span></span> | <span data-ttu-id="a05d2-206">Original</span><span class="sxs-lookup"><span data-stu-id="a05d2-206">Original</span></span>     | <span data-ttu-id="a05d2-207">Miniatura com a borda mais longa redimensionada para 800 pixels.</span><span class="sxs-lookup"><span data-stu-id="a05d2-207">Thumbnail with the longest edge resized to 800 pixels.</span></span>               |
| `smallSquare`  | <span data-ttu-id="a05d2-208">96x96</span><span class="sxs-lookup"><span data-stu-id="a05d2-208">96x96</span></span>       | <span data-ttu-id="a05d2-209">Corte quadrado</span><span class="sxs-lookup"><span data-stu-id="a05d2-209">Square Crop</span></span>  | <span data-ttu-id="a05d2-210">Miniatura quadrada pequena</span><span class="sxs-lookup"><span data-stu-id="a05d2-210">Small square thumbnail</span></span>                                               |
| `mediumSquare` | <span data-ttu-id="a05d2-211">176x176</span><span class="sxs-lookup"><span data-stu-id="a05d2-211">176x176</span></span>     | <span data-ttu-id="a05d2-212">Corte quadrado</span><span class="sxs-lookup"><span data-stu-id="a05d2-212">Square Crop</span></span>  | <span data-ttu-id="a05d2-213">Miniatura quadrada pequena</span><span class="sxs-lookup"><span data-stu-id="a05d2-213">Small square thumbnail</span></span>                                               |
| `largeSquare`  | <span data-ttu-id="a05d2-214">800x800</span><span class="sxs-lookup"><span data-stu-id="a05d2-214">800x800</span></span>     | <span data-ttu-id="a05d2-215">Corte quadrado</span><span class="sxs-lookup"><span data-stu-id="a05d2-215">Square Crop</span></span>  | <span data-ttu-id="a05d2-216">Miniatura quadrada grande</span><span class="sxs-lookup"><span data-stu-id="a05d2-216">Large square thumbnail</span></span>                                               |

## <a name="requesting-custom-thumbnail-sizes"></a><span data-ttu-id="a05d2-217">Solicitar tamanhos personalizados de miniaturas</span><span class="sxs-lookup"><span data-stu-id="a05d2-217">Requesting custom thumbnail sizes</span></span>

<span data-ttu-id="a05d2-218">Além dos tamanhos definidos, seu aplicativo pode solicitar um tamanho personalizado de miniatura, especificando as dimensões da miniatura prefixadas com `c`.</span><span class="sxs-lookup"><span data-stu-id="a05d2-218">In addition to the defined sizes, your app can request a custom thumbnail size by specifying the dimensions of the thumbnail prefixed with `c`.</span></span>
<span data-ttu-id="a05d2-219">Por exemplo, se o seu aplicativo precisar de miniaturas de 300 x 400, é possível solicitar esse tamanho desta forma:</span><span class="sxs-lookup"><span data-stu-id="a05d2-219">For example if your app needs thumbnails that are 300x400, it can request that size like this:</span></span>


# <a name="http"></a>[<span data-ttu-id="a05d2-220">HTTP</span><span class="sxs-lookup"><span data-stu-id="a05d2-220">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-thumbnail-custom-size", "scopes": "files.read", "tags": "service.graph" } -->

```msgraph-interactive
GET /me/drive/items/{item-id}/thumbnails?select=c300x400_Crop
```
# <a name="c"></a>[<span data-ttu-id="a05d2-221">C#</span><span class="sxs-lookup"><span data-stu-id="a05d2-221">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-thumbnail-custom-size-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a05d2-222">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a05d2-222">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-thumbnail-custom-size-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a05d2-223">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a05d2-223">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-thumbnail-custom-size-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a05d2-224">Java</span><span class="sxs-lookup"><span data-stu-id="a05d2-224">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-thumbnail-custom-size-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="a05d2-225">Que responde com o tamanho de miniatura personalizado selecionado:</span><span class="sxs-lookup"><span data-stu-id="a05d2-225">Which responds with just the custom thumbnail size selected:</span></span>

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.thumbnailSet)" } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "0",
      "c300x400_Crop": { "height": 300, "width": 400, "url": "https://sn3302files.onedrive.com/123"},
    }
  ]
}
```

<span data-ttu-id="a05d2-226">Você pode especificar as seguintes opções após o tamanho de miniatura solicitado:</span><span class="sxs-lookup"><span data-stu-id="a05d2-226">You can specify the following options after the size of the thumbnail requested:</span></span>

### <a name="examples-of-custom-identifiers"></a><span data-ttu-id="a05d2-227">Exemplos de identificadores personalizados</span><span class="sxs-lookup"><span data-stu-id="a05d2-227">Examples of custom identifiers</span></span>

| <span data-ttu-id="a05d2-228">Identificador de miniatura</span><span class="sxs-lookup"><span data-stu-id="a05d2-228">Thumbnail identifier</span></span> | <span data-ttu-id="a05d2-229">Resolução</span><span class="sxs-lookup"><span data-stu-id="a05d2-229">Resolution</span></span>             | <span data-ttu-id="a05d2-230">Taxa de proporção</span><span class="sxs-lookup"><span data-stu-id="a05d2-230">Aspect ratio</span></span> | <span data-ttu-id="a05d2-231">Descrição</span><span class="sxs-lookup"><span data-stu-id="a05d2-231">Description</span></span>                                                                                                                                         |
|:---------------------|:-----------------------|:-------------|:----------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="a05d2-232">c300x400</span><span class="sxs-lookup"><span data-stu-id="a05d2-232">c300x400</span></span>             | <span data-ttu-id="a05d2-233">Limitado por uma caixa de 300 x 400</span><span class="sxs-lookup"><span data-stu-id="a05d2-233">Bounded by 300x400 box</span></span> | <span data-ttu-id="a05d2-234">Original</span><span class="sxs-lookup"><span data-stu-id="a05d2-234">Original</span></span>     | <span data-ttu-id="a05d2-235">Gere uma miniatura que se ajuste em uma caixa de 300 x 400 pixels, mantendo a taxa de proporção</span><span class="sxs-lookup"><span data-stu-id="a05d2-235">Generate a thumbnail that fits inside a 300x400 pixel box, maintaining aspect ratio</span></span>                                                                 |
| <span data-ttu-id="a05d2-236">c300x400_Crop</span><span class="sxs-lookup"><span data-stu-id="a05d2-236">c300x400_Crop</span></span>        | <span data-ttu-id="a05d2-237">300x400</span><span class="sxs-lookup"><span data-stu-id="a05d2-237">300x400</span></span>                | <span data-ttu-id="a05d2-238">Recortada</span><span class="sxs-lookup"><span data-stu-id="a05d2-238">Cropped</span></span>      | <span data-ttu-id="a05d2-p112">Gere uma miniatura de 300 x 400 pixels. Para isso, é preciso redimensionar a imagem para caber na caixa de 300 x 400 e recortar o que ficar fora da caixa.</span><span class="sxs-lookup"><span data-stu-id="a05d2-p112">Generate a thumbnail that is 300x400 pixels. This works by resizing the image to fill the 300x400 box and cropping whatever spills outside the box.</span></span> |

<span data-ttu-id="a05d2-241">**Observação:** talvez a miniatura retornada não corresponda exatamente às dimensões de pixel solicitadas, mas corresponderá com a taxa de proporção.</span><span class="sxs-lookup"><span data-stu-id="a05d2-241">**Note:** The thumbnail returned may not exactly match the pixel dimensions that was requested, but will match the aspect ratio.</span></span>
<span data-ttu-id="a05d2-242">Em alguns casos, uma miniatura maior do que a solicitada pode retornar, se a miniatura já existir, e pode ser facilmente dimensionada para coincidir com a resolução solicitada.</span><span class="sxs-lookup"><span data-stu-id="a05d2-242">In some cases, a larger thumbnail may be returned than was requested, if the thumbnail already exists and can easily be scaled to match the requested resolution.</span></span>

## <a name="remarks"></a><span data-ttu-id="a05d2-243">Comentários</span><span class="sxs-lookup"><span data-stu-id="a05d2-243">Remarks</span></span>

<span data-ttu-id="a05d2-244">**Observação** No OneDrive for Business e no SharePoint:</span><span class="sxs-lookup"><span data-stu-id="a05d2-244">**Note** In OneDrive for Business and SharePoint:</span></span>

<span data-ttu-id="a05d2-245">O uso dessas chamadas para expandir a coleção de miniaturas não funcionará:</span><span class="sxs-lookup"><span data-stu-id="a05d2-245">Using these calls to expand the thumbnails collection will not work:</span></span>

* `GET /drive/root:/{item-path}?expand=children(expand=thumbnails)`
* `GET /drive/items/{item-id}/children?expand=thumbnails`

<span data-ttu-id="a05d2-246">Não há suporte para miniaturas no SharePoint Server 2016.</span><span class="sxs-lookup"><span data-stu-id="a05d2-246">Thumbnails are not supported on SharePoint Server 2016.</span></span>

### <a name="error-responses"></a><span data-ttu-id="a05d2-247">Respostas de erros</span><span class="sxs-lookup"><span data-stu-id="a05d2-247">Error responses</span></span>

<span data-ttu-id="a05d2-248">Confira mais informações sobre como os erros são retornados em [Respostas de Erros][error-response].</span><span class="sxs-lookup"><span data-stu-id="a05d2-248">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Get metadata and content for thumbnails of multiple sizes for OneDrive items.",
  "keywords": "thumbnail,content,download,sizes",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/api/driveitem-list-thumbnails.md:
      Unable to map some markdown elements into schema.
         Unmapped methods:
      enum-item-thumbnails, get-one-thumbnail, get-thumbnail-content, get-thumbnail-while-listing, get-thumbnail-custom-size
         Unmapped tables:
      Permissions - AuthScopes, Path parameters - PathParameters, Size options - Unknown, Examples of custom identifiers - Unknown",
    "Warning: Couldn't serialize request for path /me/drive/items/{var}/thumbnails/{var}/{var}/content into EDMX: System.InvalidOperationException: Uri path requires navigating into unknown object hierarchy: missing property '{var}' on 'thumbnailSet'. Possible issues:
         1) Doc bug where '{var}' isn't defined on the resource.         2) Doc bug where '{var}' is an example key and should instead be replaced with a placeholder like {item-id} or declared in the sampleKeys annotation.       3) Doc bug where 'thumbnailSet' is supposed to be an entity type, but is being treated as a complex because it (and its ancestors) are missing the keyProperty annotation
     at ApiDocs.Publishing.CSDL.CsdlWriter.ParseRequestTargetType(String requestPath, MethodCollection requestMethodCollection, EntityFramework edmx, IssueLogger issues) in D:/src/mds2/ApiDocs.Publishing/CSDL/CsdlWriter.cs:line 1145
     at ApiDocs.Publishing.CSDL.CsdlWriter.ProcessRestRequestPaths(EntityFramework edmx, String[] baseUrlsToRemove, IssueLogger issues) in D:/src/mds2/ApiDocs.Publishing/CSDL/CsdlWriter.cs:line 821"
  ],
  "tocPath": "Items/Thumbnails"
} -->
