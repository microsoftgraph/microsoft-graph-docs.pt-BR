---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Recuperar miniaturas de um arquivo ou pasta
localization_priority: Normal
ms.prod: sharepoint
description: Recupere uma coleção de recursos ThumbnailSet para um recurso DriveItem.
doc_type: apiPageType
ms.openlocfilehash: e210f42c7695d7c9f36c142c73621b09b71802e3
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36726386"
---
# <a name="list-thumbnails-for-a-driveitem"></a><span data-ttu-id="a3df7-103">Listar miniaturas para um DriveItem</span><span class="sxs-lookup"><span data-stu-id="a3df7-103">List thumbnails for a DriveItem</span></span>

<span data-ttu-id="a3df7-104">Recupere uma coleção de recursos [ThumbnailSet](../resources/thumbnailset.md) para um recurso [DriveItem](../resources/driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="a3df7-104">Retrieve a collection of [ThumbnailSet](../resources/thumbnailset.md) resources for a [DriveItem](../resources/driveitem.md) resource.</span></span>

<span data-ttu-id="a3df7-p101">Um DriveItem pode ser representado por zero ou mais recursos [ThumbnailSet](../resources/thumbnailset.md). Cada **thumbnailSet** pode ter um ou mais objetos [**thumbnail**](../resources/thumbnail.md), que são imagens que representam o item. Por exemplo, um **thumbnailSet** podem incluir objetos **thumbnail**, como objetos comuns que incluem `small`, `medium` ou `large`.</span><span class="sxs-lookup"><span data-stu-id="a3df7-p101">A DriveItem can be represented by zero or more [ThumbnailSet](../resources/thumbnailset.md) resources. Each **thumbnailSet** can have one or more [**thumbnail**](../resources/thumbnail.md) objects, which are images that represent the item. For example, a **thumbnailSet** may include **thumbnail** objects, such as common ones including `small`, `medium`, or `large`.</span></span>

<span data-ttu-id="a3df7-p102">Há várias maneiras de trabalhar com miniaturas no OneDrive. Veja a seguir as mais comuns:</span><span class="sxs-lookup"><span data-stu-id="a3df7-p102">There are many ways to work with thumbnails on OneDrive. Here are the most common ones:</span></span>

* <span data-ttu-id="a3df7-110">Enumerar miniaturas disponíveis para um item</span><span class="sxs-lookup"><span data-stu-id="a3df7-110">Enumerate available thumbnails for an item</span></span>
* <span data-ttu-id="a3df7-111">Recuperar uma única miniatura para um item</span><span class="sxs-lookup"><span data-stu-id="a3df7-111">Retrieve a single thumbnail for an item</span></span>
* <span data-ttu-id="a3df7-112">Recuperar o conteúdo da miniatura</span><span class="sxs-lookup"><span data-stu-id="a3df7-112">Retrieve thumbnail content</span></span>
* <span data-ttu-id="a3df7-113">Recuperar miniaturas de vários itens em uma única solicitação</span><span class="sxs-lookup"><span data-stu-id="a3df7-113">Retrieve thumbnails for multiple items in a single request</span></span>
* <span data-ttu-id="a3df7-114">Recuperar tamanhos personalizados de miniaturas</span><span class="sxs-lookup"><span data-stu-id="a3df7-114">Retrieve custom thumbnail sizes</span></span>
* <span data-ttu-id="a3df7-115">Carregar uma miniatura personalizada para um item</span><span class="sxs-lookup"><span data-stu-id="a3df7-115">Upload a custom thumbnail for an item</span></span>
* <span data-ttu-id="a3df7-116">Determinar se uma miniatura personalizada carregada existe</span><span class="sxs-lookup"><span data-stu-id="a3df7-116">Determine if a custom uploaded thumbnail exists</span></span>

## <a name="permissions"></a><span data-ttu-id="a3df7-117">Permissões</span><span class="sxs-lookup"><span data-stu-id="a3df7-117">Permissions</span></span>

<span data-ttu-id="a3df7-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a3df7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a3df7-120">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a3df7-120">Permission type</span></span>      | <span data-ttu-id="a3df7-121">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a3df7-121">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a3df7-122">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a3df7-122">Delegated (work or school account)</span></span> | <span data-ttu-id="a3df7-123">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3df7-123">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="a3df7-124">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a3df7-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a3df7-125">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3df7-125">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="a3df7-126">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a3df7-126">Application</span></span> | <span data-ttu-id="a3df7-127">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3df7-127">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a3df7-128">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a3df7-128">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/thumbnails
GET /groups/{group-id}/drive/items/{item-id}/thumbnails
GET /me/drive/items/{item-id}/thumbnails
GET /sites/{site-id}/drive/items/{item-id}/thumbnails
GET /users/{user-id}/drive/items/{item-id}/thumbnails
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a3df7-129">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a3df7-129">Optional query parameters</span></span>

<span data-ttu-id="a3df7-130">Este método oferece suporte ao [Parâmetro de consulta OData](/graph/query-parameters) `$select` para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a3df7-130">This method supports the `$select` [OData puery parameter](/graph/query-parameters) to customize the response.</span></span>

## <a name="response"></a><span data-ttu-id="a3df7-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="a3df7-131">Response</span></span>

<span data-ttu-id="a3df7-132">Se for bem-sucedido, esse método retornará um código de resposta `200 OK` e uma coleção de objetos [ThumbnailSet](../resources/thumbnailset.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a3df7-132">If successful, this method returns a `200 OK` response code and collection of [ThumbnailSet](../resources/thumbnailset.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a3df7-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a3df7-133">Example</span></span>

<span data-ttu-id="a3df7-134">Veja um exemplo da solicitação que recupera as miniaturas disponíveis de um item no OneDrive atual do usuário.</span><span class="sxs-lookup"><span data-stu-id="a3df7-134">Here is an example of the request which retrieves available thumbnails for an item in the current user's OneDrive.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="a3df7-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="a3df7-135">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "enum-item-thumbnails", "scopes": "files.read", "tags": "service.graph" } -->

```msgraph-interactive
GET /me/drive/items/{item-id}/thumbnails
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a3df7-136">C#</span><span class="sxs-lookup"><span data-stu-id="a3df7-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/enum-item-thumbnails-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a3df7-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a3df7-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/enum-item-thumbnails-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a3df7-138">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="a3df7-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/enum-item-thumbnails-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="a3df7-139">Java</span><span class="sxs-lookup"><span data-stu-id="a3df7-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/enum-item-thumbnails-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="a3df7-140">Isto retorna uma matriz de **thumbnailSets** disponíveis para o item.</span><span class="sxs-lookup"><span data-stu-id="a3df7-140">This returns an array of available **thumbnailSets** for the item.</span></span> <span data-ttu-id="a3df7-141">Qualquer item em uma unidade pode ter zero ou mais miniaturas.</span><span class="sxs-lookup"><span data-stu-id="a3df7-141">Any item in a drive can have zero or more thumbnails.</span></span>

<span data-ttu-id="a3df7-p105">**Observação:** Você pode usar o parâmetro da cadeia de caracteres de consulta _select_ para controlar quais tamanhos de miniatura são retornados no **ThumbnailSet**. Por exemplo, `/thumbnails?select=medium` recupera somente miniaturas de tamanho médio.</span><span class="sxs-lookup"><span data-stu-id="a3df7-p105">**Note:** You can use the _select_ query string parameter to control which thumbnail sizes are returned in the **ThumbnailSet**. For example, `/thumbnails?select=medium` retrieves only the medium sized thumbnails.</span></span>


### <a name="response"></a><span data-ttu-id="a3df7-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="a3df7-144">Response</span></span>

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

## <a name="get-a-single-thumbnail"></a><span data-ttu-id="a3df7-145">Obter uma única miniatura</span><span class="sxs-lookup"><span data-stu-id="a3df7-145">Get a single thumbnail</span></span>

<span data-ttu-id="a3df7-146">Recupere os metadados de uma única miniatura e um único tamanho endereçando-os diretamente em uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="a3df7-146">Retrieve the metadata for a single thumbnail and size by addressing it directly in a request.</span></span>

### <a name="http-request"></a><span data-ttu-id="a3df7-147">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a3df7-147">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="a3df7-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="a3df7-148">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-one-thumbnail", "scopes": "files.read", "tags": "service.graph" } -->

```msgraph-interactive
GET /me/drive/items/{item-id}/thumbnails/{thumb-id}/{size}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a3df7-149">C#</span><span class="sxs-lookup"><span data-stu-id="a3df7-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-one-thumbnail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a3df7-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a3df7-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-one-thumbnail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a3df7-151">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="a3df7-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-one-thumbnail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="a3df7-152">Java</span><span class="sxs-lookup"><span data-stu-id="a3df7-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-one-thumbnail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="path-parameters"></a><span data-ttu-id="a3df7-153">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="a3df7-153">Path parameters</span></span>

| <span data-ttu-id="a3df7-154">Nome</span><span class="sxs-lookup"><span data-stu-id="a3df7-154">Name</span></span>         | <span data-ttu-id="a3df7-155">Tipo</span><span class="sxs-lookup"><span data-stu-id="a3df7-155">Type</span></span>   | <span data-ttu-id="a3df7-156">Descrição</span><span class="sxs-lookup"><span data-stu-id="a3df7-156">Description</span></span>                                                                              |
|:-------------|:-------|:-----------------------------------------------------------------------------------------|
| <span data-ttu-id="a3df7-157">**item-id**</span><span class="sxs-lookup"><span data-stu-id="a3df7-157">**item-id**</span></span>  | <span data-ttu-id="a3df7-158">string</span><span class="sxs-lookup"><span data-stu-id="a3df7-158">string</span></span> | <span data-ttu-id="a3df7-159">O identificador exclusivo do item referenciado.</span><span class="sxs-lookup"><span data-stu-id="a3df7-159">The unique identifier for the item referenced.</span></span>                                           |
| <span data-ttu-id="a3df7-160">**thumb-id**</span><span class="sxs-lookup"><span data-stu-id="a3df7-160">**thumb-id**</span></span> | <span data-ttu-id="a3df7-161">number</span><span class="sxs-lookup"><span data-stu-id="a3df7-161">number</span></span> | <span data-ttu-id="a3df7-p106">O índice da miniatura, geralmente de 0 a 4. Se houver uma miniatura personalizada, seu índice será 0.</span><span class="sxs-lookup"><span data-stu-id="a3df7-p106">The index of the thumbnail, usually 0-4. If there is a custom thumbnail, its index is 0.</span></span> |
| <span data-ttu-id="a3df7-164">**size**</span><span class="sxs-lookup"><span data-stu-id="a3df7-164">**size**</span></span>     | <span data-ttu-id="a3df7-165">string</span><span class="sxs-lookup"><span data-stu-id="a3df7-165">string</span></span> | <span data-ttu-id="a3df7-166">O tamanho da miniatura solicitada.</span><span class="sxs-lookup"><span data-stu-id="a3df7-166">The size of the thumbnail requested.</span></span> <span data-ttu-id="a3df7-167">Pode ter um dos tamanhos padrão listados abaixo, ou um tamanho personalizado.</span><span class="sxs-lookup"><span data-stu-id="a3df7-167">This can be one of the standard sizes listed below or a custom size.</span></span> |

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

## <a name="retrieve-thumbnail-binary-content"></a><span data-ttu-id="a3df7-168">Recuperar o conteúdo binário da miniatura</span><span class="sxs-lookup"><span data-stu-id="a3df7-168">Retrieve thumbnail binary content</span></span>

<span data-ttu-id="a3df7-169">Você pode recuperar diretamente o conteúdo da miniatura solicitando a propriedade **content** dessa miniatura.</span><span class="sxs-lookup"><span data-stu-id="a3df7-169">You can directly retrieve the content of the thumbnail by requesting the **content** property of the thumbnail.</span></span>

### <a name="http-request"></a><span data-ttu-id="a3df7-170">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a3df7-170">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="a3df7-171">HTTP</span><span class="sxs-lookup"><span data-stu-id="a3df7-171">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name":"get-thumbnail-content", "scopes": "files.read", "tags": "service.graph" } -->

```msgraph-interactive
GET /me/drive/items/{item-id}/thumbnails/{thumb-id}/{size}/content
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a3df7-172">C#</span><span class="sxs-lookup"><span data-stu-id="a3df7-172">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-thumbnail-content-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a3df7-173">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a3df7-173">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-thumbnail-content-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a3df7-174">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="a3df7-174">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-thumbnail-content-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="a3df7-175">Java</span><span class="sxs-lookup"><span data-stu-id="a3df7-175">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-thumbnail-content-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a3df7-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="a3df7-176">Response</span></span>

<span data-ttu-id="a3df7-177">O serviço responde com um redirecionamento para a URL da miniatura.</span><span class="sxs-lookup"><span data-stu-id="a3df7-177">The service responds with a redirect to the thumbnail URL.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```

<span data-ttu-id="a3df7-178">URLs de miniaturas são seguras em cache.</span><span class="sxs-lookup"><span data-stu-id="a3df7-178">Thumbnail URLs are cache-safe.</span></span> <span data-ttu-id="a3df7-179">A URL mudará se o item for alterado de uma maneira que exigir que uma nova miniatura seja gerada.</span><span class="sxs-lookup"><span data-stu-id="a3df7-179">The URL will change, if the item changes in a way that requires a new thumbnail to be generated.</span></span>


## <a name="getting-thumbnails-while-listing-driveitems"></a><span data-ttu-id="a3df7-180">Obter miniaturas ao listar DriveItems</span><span class="sxs-lookup"><span data-stu-id="a3df7-180">Getting thumbnails while listing DriveItems</span></span>

<span data-ttu-id="a3df7-181">Se você estiver recuperando uma lista de recursos DriveItem para exibição, use o parâmetro de cadeia de consulta _$expand_ para incluir as miniaturas para esses recursos.</span><span class="sxs-lookup"><span data-stu-id="a3df7-181">If you are retrieving a list of DriveItem resources to display, you can use the _$expand_ query string parameter to also include the thumbnails for those resources.</span></span>
<span data-ttu-id="a3df7-182">Isso permite que seu aplicativo recupere miniaturas e itens em uma única solicitação, em vez de emitir muitas solicitações.</span><span class="sxs-lookup"><span data-stu-id="a3df7-182">This enables your app to retrieve thumbnails and items in a single request, instead of issuing many requests.</span></span>

### <a name="http-request"></a><span data-ttu-id="a3df7-183">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a3df7-183">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="a3df7-184">HTTP</span><span class="sxs-lookup"><span data-stu-id="a3df7-184">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name":"get-thumbnail-while-listing", "scopes": "files.read", "tags": "service.graph" } -->

```msgraph-interactive
GET /me/drive/items/{item-id}/children?$expand=thumbnails
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a3df7-185">C#</span><span class="sxs-lookup"><span data-stu-id="a3df7-185">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-thumbnail-while-listing-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a3df7-186">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a3df7-186">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-thumbnail-while-listing-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a3df7-187">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="a3df7-187">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-thumbnail-while-listing-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="a3df7-188">Java</span><span class="sxs-lookup"><span data-stu-id="a3df7-188">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-thumbnail-while-listing-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a3df7-189">Resposta</span><span class="sxs-lookup"><span data-stu-id="a3df7-189">Response</span></span>

<span data-ttu-id="a3df7-190">As respostas do serviço com a lista de DriveItems e suas miniaturas.</span><span class="sxs-lookup"><span data-stu-id="a3df7-190">The service responses with the list of DriveItems and their thumbnails.</span></span>

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

## <a name="size-options"></a><span data-ttu-id="a3df7-191">Opções de tamanho</span><span class="sxs-lookup"><span data-stu-id="a3df7-191">Size options</span></span>

<span data-ttu-id="a3df7-p110">Essa tabela define os possíveis tamanhos de miniaturas. Embora você possa solicitar qualquer tamanho de miniatura arbitrário, os valores definidos provavelmente existem e retornam um valor rapidamente:</span><span class="sxs-lookup"><span data-stu-id="a3df7-p110">This table defines the possible thumbnail sizes. While you can request any arbitrary thumbnail size, the defined values are likely to exist and return a value quickly:</span></span>

| <span data-ttu-id="a3df7-194">Nome</span><span class="sxs-lookup"><span data-stu-id="a3df7-194">Name</span></span>           | <span data-ttu-id="a3df7-195">Resolução</span><span class="sxs-lookup"><span data-stu-id="a3df7-195">Resolution</span></span>  | <span data-ttu-id="a3df7-196">Taxa de proporção</span><span class="sxs-lookup"><span data-stu-id="a3df7-196">Aspect Ratio</span></span> | <span data-ttu-id="a3df7-197">Descrição</span><span class="sxs-lookup"><span data-stu-id="a3df7-197">Description</span></span>                                                          |
|:---------------|:------------|:-------------|:---------------------------------------------------------------------|
| `small`        | <span data-ttu-id="a3df7-198">96 mais longa</span><span class="sxs-lookup"><span data-stu-id="a3df7-198">96 longest</span></span>  | <span data-ttu-id="a3df7-199">Original</span><span class="sxs-lookup"><span data-stu-id="a3df7-199">Original</span></span>     | <span data-ttu-id="a3df7-200">Miniatura pequena e altamente compactada, recortada em uma taxa de proporção quadrada.</span><span class="sxs-lookup"><span data-stu-id="a3df7-200">Small, highly compressed thumbnail cropped to a square aspect ratio.</span></span> |
| `medium`       | <span data-ttu-id="a3df7-201">176 mais longa</span><span class="sxs-lookup"><span data-stu-id="a3df7-201">176 longest</span></span> | <span data-ttu-id="a3df7-202">Original</span><span class="sxs-lookup"><span data-stu-id="a3df7-202">Original</span></span>     | <span data-ttu-id="a3df7-203">Recortada no tamanho do item padrão para o modo de exibição de Web do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="a3df7-203">Cropped to the standard item size for the OneDrive web view.</span></span>         |
| `large`        | <span data-ttu-id="a3df7-204">800 mais longa</span><span class="sxs-lookup"><span data-stu-id="a3df7-204">800 longest</span></span> | <span data-ttu-id="a3df7-205">Original</span><span class="sxs-lookup"><span data-stu-id="a3df7-205">Original</span></span>     | <span data-ttu-id="a3df7-206">Miniatura com a borda mais longa redimensionada para 800 pixels.</span><span class="sxs-lookup"><span data-stu-id="a3df7-206">Thumbnail with the longest edge resized to 800 pixels.</span></span>               |
| `smallSquare`  | <span data-ttu-id="a3df7-207">96x96</span><span class="sxs-lookup"><span data-stu-id="a3df7-207">96x96</span></span>       | <span data-ttu-id="a3df7-208">Corte quadrado</span><span class="sxs-lookup"><span data-stu-id="a3df7-208">Square Crop</span></span>  | <span data-ttu-id="a3df7-209">Miniatura quadrada pequena</span><span class="sxs-lookup"><span data-stu-id="a3df7-209">Small square thumbnail</span></span>                                               |
| `mediumSquare` | <span data-ttu-id="a3df7-210">176x176</span><span class="sxs-lookup"><span data-stu-id="a3df7-210">176x176</span></span>     | <span data-ttu-id="a3df7-211">Corte quadrado</span><span class="sxs-lookup"><span data-stu-id="a3df7-211">Square Crop</span></span>  | <span data-ttu-id="a3df7-212">Miniatura quadrada pequena</span><span class="sxs-lookup"><span data-stu-id="a3df7-212">Small square thumbnail</span></span>                                               |
| `largeSquare`  | <span data-ttu-id="a3df7-213">800x800</span><span class="sxs-lookup"><span data-stu-id="a3df7-213">800x800</span></span>     | <span data-ttu-id="a3df7-214">Corte quadrado</span><span class="sxs-lookup"><span data-stu-id="a3df7-214">Square Crop</span></span>  | <span data-ttu-id="a3df7-215">Miniatura quadrada grande</span><span class="sxs-lookup"><span data-stu-id="a3df7-215">Large square thumbnail</span></span>                                               |

## <a name="requesting-custom-thumbnail-sizes"></a><span data-ttu-id="a3df7-216">Solicitar tamanhos personalizados de miniaturas</span><span class="sxs-lookup"><span data-stu-id="a3df7-216">Requesting custom thumbnail sizes</span></span>

<span data-ttu-id="a3df7-217">Além dos tamanhos definidos, seu aplicativo pode solicitar um tamanho personalizado de miniatura, especificando as dimensões da miniatura prefixadas com `c`.</span><span class="sxs-lookup"><span data-stu-id="a3df7-217">In addition to the defined sizes, your app can request a custom thumbnail size by specifying the dimensions of the thumbnail prefixed with `c`.</span></span>
<span data-ttu-id="a3df7-218">Por exemplo, se o seu aplicativo precisar de miniaturas de 300 x 400, é possível solicitar esse tamanho desta forma:</span><span class="sxs-lookup"><span data-stu-id="a3df7-218">For example if your app needs thumbnails that are 300x400, it can request that size like this:</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="a3df7-219">HTTP</span><span class="sxs-lookup"><span data-stu-id="a3df7-219">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-thumbnail-custom-size", "scopes": "files.read", "tags": "service.graph" } -->

```msgraph-interactive
GET /me/drive/items/{item-id}/thumbnails?select=c300x400_Crop
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a3df7-220">C#</span><span class="sxs-lookup"><span data-stu-id="a3df7-220">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-thumbnail-custom-size-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a3df7-221">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a3df7-221">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-thumbnail-custom-size-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a3df7-222">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="a3df7-222">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-thumbnail-custom-size-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="a3df7-223">Java</span><span class="sxs-lookup"><span data-stu-id="a3df7-223">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-thumbnail-custom-size-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="a3df7-224">Que responde com o tamanho de miniatura personalizado selecionado:</span><span class="sxs-lookup"><span data-stu-id="a3df7-224">Which responds with just the custom thumbnail size selected:</span></span>

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

<span data-ttu-id="a3df7-225">Você pode especificar as seguintes opções após o tamanho de miniatura solicitado:</span><span class="sxs-lookup"><span data-stu-id="a3df7-225">You can specify the following options after the size of the thumbnail requested:</span></span>

### <a name="examples-of-custom-identifiers"></a><span data-ttu-id="a3df7-226">Exemplos de identificadores personalizados</span><span class="sxs-lookup"><span data-stu-id="a3df7-226">Examples of custom identifiers</span></span>

| <span data-ttu-id="a3df7-227">Identificador de miniatura</span><span class="sxs-lookup"><span data-stu-id="a3df7-227">Thumbnail identifier</span></span> | <span data-ttu-id="a3df7-228">Resolução</span><span class="sxs-lookup"><span data-stu-id="a3df7-228">Resolution</span></span>             | <span data-ttu-id="a3df7-229">Taxa de proporção</span><span class="sxs-lookup"><span data-stu-id="a3df7-229">Aspect ratio</span></span> | <span data-ttu-id="a3df7-230">Descrição</span><span class="sxs-lookup"><span data-stu-id="a3df7-230">Description</span></span>                                                                                                                                         |
|:---------------------|:-----------------------|:-------------|:----------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="a3df7-231">c300x400</span><span class="sxs-lookup"><span data-stu-id="a3df7-231">c300x400</span></span>             | <span data-ttu-id="a3df7-232">Limitado por uma caixa de 300 x 400</span><span class="sxs-lookup"><span data-stu-id="a3df7-232">Bounded by 300x400 box</span></span> | <span data-ttu-id="a3df7-233">Original</span><span class="sxs-lookup"><span data-stu-id="a3df7-233">Original</span></span>     | <span data-ttu-id="a3df7-234">Gere uma miniatura que se ajuste em uma caixa de 300 x 400 pixels, mantendo a taxa de proporção</span><span class="sxs-lookup"><span data-stu-id="a3df7-234">Generate a thumbnail that fits inside a 300x400 pixel box, maintaining aspect ratio</span></span>                                                                 |
| <span data-ttu-id="a3df7-235">c300x400_Crop</span><span class="sxs-lookup"><span data-stu-id="a3df7-235">c300x400_Crop</span></span>        | <span data-ttu-id="a3df7-236">300x400</span><span class="sxs-lookup"><span data-stu-id="a3df7-236">300x400</span></span>                | <span data-ttu-id="a3df7-237">Recortada</span><span class="sxs-lookup"><span data-stu-id="a3df7-237">Cropped</span></span>      | <span data-ttu-id="a3df7-p112">Gere uma miniatura de 300 x 400 pixels. Para isso, é preciso redimensionar a imagem para caber na caixa de 300 x 400 e recortar o que ficar fora da caixa.</span><span class="sxs-lookup"><span data-stu-id="a3df7-p112">Generate a thumbnail that is 300x400 pixels. This works by resizing the image to fill the 300x400 box and cropping whatever spills outside the box.</span></span> |

<span data-ttu-id="a3df7-240">**Observação:** talvez a miniatura retornada não corresponda exatamente às dimensões de pixel solicitadas, mas corresponderá com a taxa de proporção.</span><span class="sxs-lookup"><span data-stu-id="a3df7-240">**Note:** The thumbnail returned may not exactly match the pixel dimensions that was requested, but will match the aspect ratio.</span></span>
<span data-ttu-id="a3df7-241">Em alguns casos, uma miniatura maior do que a solicitada pode retornar, se a miniatura já existir, e pode ser facilmente dimensionada para coincidir com a resolução solicitada.</span><span class="sxs-lookup"><span data-stu-id="a3df7-241">In some cases, a larger thumbnail may be returned than was requested, if the thumbnail already exists and can easily be scaled to match the requested resolution.</span></span>

## <a name="remarks"></a><span data-ttu-id="a3df7-242">Comentários</span><span class="sxs-lookup"><span data-stu-id="a3df7-242">Remarks</span></span>

<span data-ttu-id="a3df7-243">**Observação** No OneDrive for Business e no SharePoint:</span><span class="sxs-lookup"><span data-stu-id="a3df7-243">**Note** In OneDrive for Business and SharePoint:</span></span>

<span data-ttu-id="a3df7-244">O uso dessas chamadas para expandir a coleção de miniaturas não funcionará:</span><span class="sxs-lookup"><span data-stu-id="a3df7-244">Using these calls to expand the thumbnails collection will not work:</span></span>

* `GET /drive/root:/{item-path}?expand=children(expand=thumbnails)`
* `GET /drive/items/{item-id}/children?expand=thumbnails`

<span data-ttu-id="a3df7-245">Não há suporte para miniaturas no SharePoint Server 2016.</span><span class="sxs-lookup"><span data-stu-id="a3df7-245">Thumbnails are not supported on SharePoint Server 2016.</span></span>

### <a name="error-responses"></a><span data-ttu-id="a3df7-246">Respostas de erro</span><span class="sxs-lookup"><span data-stu-id="a3df7-246">Error responses</span></span>

<span data-ttu-id="a3df7-247">Confira mais informações sobre como os erros são retornados em [Respostas de erro][error-response].</span><span class="sxs-lookup"><span data-stu-id="a3df7-247">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

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
