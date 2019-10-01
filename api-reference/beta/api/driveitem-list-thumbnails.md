---
author: JeremyKelley
description: Recupere uma coleção de recursos ThumbnailSet para um recurso DriveItem.
ms.date: 09/10/2017
title: Recuperar miniaturas de um arquivo ou pasta
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 2bed97e65a57c4a7d46336e9dcd845780e9e8d30
ms.sourcegitcommit: 2fb178ae78b5ecc47207d2b19d0c5a46e07e0960
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/01/2019
ms.locfileid: "37333224"
---
# <a name="list-thumbnails-for-a-driveitem"></a><span data-ttu-id="5c56e-103">Listar miniaturas para um DriveItem</span><span class="sxs-lookup"><span data-stu-id="5c56e-103">List thumbnails for a DriveItem</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5c56e-104">Recupere uma coleção de recursos [ThumbnailSet](../resources/thumbnailset.md) para um recurso [DriveItem](../resources/driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="5c56e-104">Retrieve a collection of [ThumbnailSet](../resources/thumbnailset.md) resources for a [DriveItem](../resources/driveitem.md) resource.</span></span>

<span data-ttu-id="5c56e-p101">Um DriveItem pode ser representado por zero ou mais recursos [ThumbnailSet](../resources/thumbnailset.md). Cada **thumbnailSet** pode ter um ou mais objetos [**thumbnail**](../resources/thumbnail.md), que são imagens que representam o item. Por exemplo, um **thumbnailSet** podem incluir objetos **thumbnail**, como objetos comuns que incluem `small`, `medium` ou `large`.</span><span class="sxs-lookup"><span data-stu-id="5c56e-p101">A DriveItem can be represented by zero or more [ThumbnailSet](../resources/thumbnailset.md) resources. Each **thumbnailSet** can have one or more [**thumbnail**](../resources/thumbnail.md) objects, which are images that represent the item. For example, a **thumbnailSet** may include **thumbnail** objects, such as common ones including `small`, `medium`, or `large`.</span></span>

<span data-ttu-id="5c56e-p102">Há várias maneiras de trabalhar com miniaturas no OneDrive. Veja a seguir as mais comuns:</span><span class="sxs-lookup"><span data-stu-id="5c56e-p102">There are many ways to work with thumbnails on OneDrive. Here are the most common ones:</span></span>

* <span data-ttu-id="5c56e-110">Enumerar miniaturas disponíveis para um item</span><span class="sxs-lookup"><span data-stu-id="5c56e-110">Enumerate available thumbnails for an item</span></span>
* <span data-ttu-id="5c56e-111">Recuperar uma única miniatura para um item</span><span class="sxs-lookup"><span data-stu-id="5c56e-111">Retrieve a single thumbnail for an item</span></span>
* <span data-ttu-id="5c56e-112">Recuperar o conteúdo da miniatura</span><span class="sxs-lookup"><span data-stu-id="5c56e-112">Retrieve thumbnail content</span></span>
* <span data-ttu-id="5c56e-113">Recuperar miniaturas de vários itens em uma única solicitação</span><span class="sxs-lookup"><span data-stu-id="5c56e-113">Retrieve thumbnails for multiple items in a single request</span></span>
* <span data-ttu-id="5c56e-114">Recuperar tamanhos personalizados de miniaturas</span><span class="sxs-lookup"><span data-stu-id="5c56e-114">Retrieve custom thumbnail sizes</span></span>
* <span data-ttu-id="5c56e-115">Carregar uma miniatura personalizada para um item</span><span class="sxs-lookup"><span data-stu-id="5c56e-115">Upload a custom thumbnail for an item</span></span>
* <span data-ttu-id="5c56e-116">Determinar se uma miniatura personalizada carregada existe</span><span class="sxs-lookup"><span data-stu-id="5c56e-116">Determine if a custom uploaded thumbnail exists</span></span>


## <a name="permissions"></a><span data-ttu-id="5c56e-117">Permissões</span><span class="sxs-lookup"><span data-stu-id="5c56e-117">Permissions</span></span>

<span data-ttu-id="5c56e-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5c56e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c56e-120">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5c56e-120">Permission type</span></span>      | <span data-ttu-id="5c56e-121">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5c56e-121">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5c56e-122">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5c56e-122">Delegated (work or school account)</span></span> | <span data-ttu-id="5c56e-123">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c56e-123">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="5c56e-124">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5c56e-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5c56e-125">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c56e-125">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="5c56e-126">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5c56e-126">Application</span></span> | <span data-ttu-id="5c56e-127">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c56e-127">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5c56e-128">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5c56e-128">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/thumbnails
GET /groups/{group-id}/drive/items/{item-id}/thumbnails
GET /me/drive/items/{item-id}/thumbnails
GET /sites/{site-id}/drive/items/{item-id}/thumbnails
GET /users/{user-id}/drive/items/{item-id}/thumbnails
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5c56e-129">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5c56e-129">Optional query parameters</span></span>

<span data-ttu-id="5c56e-130">Este método oferece suporte ao [Parâmetro de consulta OData](/graph/query-parameters) `$select` para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5c56e-130">This method supports the `$select` [OData puery parameter](/graph/query-parameters) to customize the response.</span></span>

<span data-ttu-id="5c56e-131">Além disso, esse método dá suporte à recuperação da miniatura com o valor de EXIF da orientação original e sem a rotação aplicada `originalOrientation=true` acrescentando o parâmetro de consulta.</span><span class="sxs-lookup"><span data-stu-id="5c56e-131">Additionally, this method supports retrieving the thumbnail with the original orientation EXIF value and without the applied rotation by appending the `originalOrientation=true` query parameter.</span></span>
<span data-ttu-id="5c56e-132">No momento, isso só tem suporte no OneDrive Personal.</span><span class="sxs-lookup"><span data-stu-id="5c56e-132">This is currently only supported on OneDrive Personal.</span></span>

## <a name="response"></a><span data-ttu-id="5c56e-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c56e-133">Response</span></span>

<span data-ttu-id="5c56e-134">Se for bem-sucedido, esse método retornará um código de resposta `200 OK` e uma coleção de objetos [ThumbnailSet](../resources/thumbnailset.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5c56e-134">If successful, this method returns a `200 OK` response code and collection of [ThumbnailSet](../resources/thumbnailset.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5c56e-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5c56e-135">Example</span></span>

<span data-ttu-id="5c56e-136">Veja um exemplo da solicitação que recupera as miniaturas disponíveis de um item no OneDrive atual do usuário.</span><span class="sxs-lookup"><span data-stu-id="5c56e-136">Here is an example of the request which retrieves available thumbnails for an item in the current user's OneDrive.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="5c56e-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="5c56e-137">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "enum-item-thumbnails", "scopes": "files.read" } -->

```msgraph-interactive
GET /me/drive/items/{item-id}/thumbnails
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="5c56e-138">C#</span><span class="sxs-lookup"><span data-stu-id="5c56e-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/enum-item-thumbnails-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5c56e-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5c56e-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/enum-item-thumbnails-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5c56e-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5c56e-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/enum-item-thumbnails-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="5c56e-141">Isto retorna uma matriz de **thumbnailSets** disponíveis para o item.</span><span class="sxs-lookup"><span data-stu-id="5c56e-141">This returns an array of available **thumbnailSets** for the item.</span></span> <span data-ttu-id="5c56e-142">Qualquer item em uma unidade pode ter zero ou mais miniaturas.</span><span class="sxs-lookup"><span data-stu-id="5c56e-142">Any item in a drive can have zero or more thumbnails.</span></span>

<span data-ttu-id="5c56e-p106">**Observação:** Você pode usar o parâmetro da cadeia de caracteres de consulta _select_ para controlar quais tamanhos de miniatura são retornados no **ThumbnailSet**. Por exemplo, `/thumbnails?select=medium` recupera somente miniaturas de tamanho médio.</span><span class="sxs-lookup"><span data-stu-id="5c56e-p106">**Note:** You can use the _select_ query string parameter to control which thumbnail sizes are returned in the **ThumbnailSet**. For example, `/thumbnails?select=medium` retrieves only the medium sized thumbnails.</span></span>


### <a name="response"></a><span data-ttu-id="5c56e-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c56e-145">Response</span></span>

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

## <a name="get-a-single-thumbnail"></a><span data-ttu-id="5c56e-146">Obter uma única miniatura</span><span class="sxs-lookup"><span data-stu-id="5c56e-146">Get a single thumbnail</span></span>

<span data-ttu-id="5c56e-147">Recupere os metadados de uma única miniatura e um único tamanho endereçando-os diretamente em uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="5c56e-147">Retrieve the metadata for a single thumbnail and size by addressing it directly in a request.</span></span>

### <a name="http-request"></a><span data-ttu-id="5c56e-148">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5c56e-148">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="5c56e-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="5c56e-149">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-one-thumbnail", "scopes": "files.read" } -->

```msgraph-interactive
GET /me/drive/items/{item-id}/thumbnails/{thumb-id}/{size}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="5c56e-150">C#</span><span class="sxs-lookup"><span data-stu-id="5c56e-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-one-thumbnail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5c56e-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5c56e-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-one-thumbnail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5c56e-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5c56e-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-one-thumbnail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="path-parameters"></a><span data-ttu-id="5c56e-153">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="5c56e-153">Path parameters</span></span>

| <span data-ttu-id="5c56e-154">Nome</span><span class="sxs-lookup"><span data-stu-id="5c56e-154">Name</span></span>         | <span data-ttu-id="5c56e-155">Tipo</span><span class="sxs-lookup"><span data-stu-id="5c56e-155">Type</span></span>   | <span data-ttu-id="5c56e-156">Descrição</span><span class="sxs-lookup"><span data-stu-id="5c56e-156">Description</span></span>                                                                              |
|:-------------|:-------|:-----------------------------------------------------------------------------------------|
| <span data-ttu-id="5c56e-157">**item-id**</span><span class="sxs-lookup"><span data-stu-id="5c56e-157">**item-id**</span></span>  | <span data-ttu-id="5c56e-158">string</span><span class="sxs-lookup"><span data-stu-id="5c56e-158">string</span></span> | <span data-ttu-id="5c56e-159">O identificador exclusivo do item referenciado.</span><span class="sxs-lookup"><span data-stu-id="5c56e-159">The unique identifier for the item referenced.</span></span>                                           |
| <span data-ttu-id="5c56e-160">**thumb-id**</span><span class="sxs-lookup"><span data-stu-id="5c56e-160">**thumb-id**</span></span> | <span data-ttu-id="5c56e-161">number</span><span class="sxs-lookup"><span data-stu-id="5c56e-161">number</span></span> | <span data-ttu-id="5c56e-p107">O índice da miniatura, geralmente de 0 a 4. Se houver uma miniatura personalizada, seu índice será 0.</span><span class="sxs-lookup"><span data-stu-id="5c56e-p107">The index of the thumbnail, usually 0-4. If there is a custom thumbnail, its index is 0.</span></span> |
| <span data-ttu-id="5c56e-164">**size**</span><span class="sxs-lookup"><span data-stu-id="5c56e-164">**size**</span></span>     | <span data-ttu-id="5c56e-165">string</span><span class="sxs-lookup"><span data-stu-id="5c56e-165">string</span></span> | <span data-ttu-id="5c56e-166">O tamanho da miniatura solicitada.</span><span class="sxs-lookup"><span data-stu-id="5c56e-166">The size of the thumbnail requested.</span></span> <span data-ttu-id="5c56e-167">Pode ter um dos tamanhos padrão listados abaixo, ou um tamanho personalizado.</span><span class="sxs-lookup"><span data-stu-id="5c56e-167">This can be one of the standard sizes listed below or a custom size.</span></span> |

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

## <a name="retrieve-thumbnail-binary-content"></a><span data-ttu-id="5c56e-168">Recuperar o conteúdo binário da miniatura</span><span class="sxs-lookup"><span data-stu-id="5c56e-168">Retrieve thumbnail binary content</span></span>

<span data-ttu-id="5c56e-169">Você pode recuperar diretamente o conteúdo da miniatura solicitando a propriedade **content** dessa miniatura.</span><span class="sxs-lookup"><span data-stu-id="5c56e-169">You can directly retrieve the content of the thumbnail by requesting the **content** property of the thumbnail.</span></span>

### <a name="http-request"></a><span data-ttu-id="5c56e-170">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5c56e-170">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="5c56e-171">HTTP</span><span class="sxs-lookup"><span data-stu-id="5c56e-171">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name":"get-thumbnail-content", "scopes": "files.read" } -->

```msgraph-interactive
GET /me/drive/items/{item-id}/thumbnails/{thumb-id}/{size}/content
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="5c56e-172">C#</span><span class="sxs-lookup"><span data-stu-id="5c56e-172">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-thumbnail-content-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5c56e-173">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5c56e-173">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-thumbnail-content-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5c56e-174">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5c56e-174">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-thumbnail-content-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5c56e-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c56e-175">Response</span></span>

<span data-ttu-id="5c56e-176">O serviço responde com um redirecionamento para a URL da miniatura.</span><span class="sxs-lookup"><span data-stu-id="5c56e-176">The service responds with a redirect to the thumbnail URL.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```

<span data-ttu-id="5c56e-177">URLs de miniaturas são seguras em cache.</span><span class="sxs-lookup"><span data-stu-id="5c56e-177">Thumbnail URLs are cache-safe.</span></span> <span data-ttu-id="5c56e-178">A URL mudará se o item for alterado de uma maneira que exigir que uma nova miniatura seja gerada.</span><span class="sxs-lookup"><span data-stu-id="5c56e-178">The URL will change, if the item changes in a way that requires a new thumbnail to be generated.</span></span>


## <a name="getting-thumbnails-while-listing-driveitems"></a><span data-ttu-id="5c56e-179">Obter miniaturas ao listar DriveItems</span><span class="sxs-lookup"><span data-stu-id="5c56e-179">Getting thumbnails while listing DriveItems</span></span>

<span data-ttu-id="5c56e-180">Se você estiver recuperando uma lista de recursos DriveItem para exibição, use o parâmetro de cadeia de consulta _$expand_ para incluir as miniaturas para esses recursos.</span><span class="sxs-lookup"><span data-stu-id="5c56e-180">If you are retrieving a list of DriveItem resources to display, you can use the _$expand_ query string parameter to also include the thumbnails for those resources.</span></span>
<span data-ttu-id="5c56e-181">Isso permite que seu aplicativo recupere miniaturas e itens em uma única solicitação, em vez de emitir muitas solicitações.</span><span class="sxs-lookup"><span data-stu-id="5c56e-181">This enables your app to retrieve thumbnails and items in a single request, instead of issuing many requests.</span></span>

### <a name="http-request"></a><span data-ttu-id="5c56e-182">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5c56e-182">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="5c56e-183">HTTP</span><span class="sxs-lookup"><span data-stu-id="5c56e-183">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name":"get-thumbnail-while-listing", "scopes": "files.read" } -->

```msgraph-interactive
GET /me/drive/items/{item-id}/children?$expand=thumbnails
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="5c56e-184">C#</span><span class="sxs-lookup"><span data-stu-id="5c56e-184">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-thumbnail-while-listing-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5c56e-185">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5c56e-185">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-thumbnail-while-listing-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5c56e-186">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5c56e-186">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-thumbnail-while-listing-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5c56e-187">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c56e-187">Response</span></span>

<span data-ttu-id="5c56e-188">As respostas do serviço com a lista de DriveItems e suas miniaturas.</span><span class="sxs-lookup"><span data-stu-id="5c56e-188">The service responses with the list of DriveItems and their thumbnails.</span></span>

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

## <a name="size-values"></a><span data-ttu-id="5c56e-189">Valores de tamanho</span><span class="sxs-lookup"><span data-stu-id="5c56e-189">Size values</span></span>

<span data-ttu-id="5c56e-p111">Essa tabela define os possíveis tamanhos de miniaturas. Embora você possa solicitar qualquer tamanho de miniatura arbitrário, os valores definidos provavelmente existem e retornam um valor rapidamente:</span><span class="sxs-lookup"><span data-stu-id="5c56e-p111">This table defines the possible thumbnail sizes. While you can request any arbitrary thumbnail size, the defined values are likely to exist and return a value quickly:</span></span>

| <span data-ttu-id="5c56e-192">Nome</span><span class="sxs-lookup"><span data-stu-id="5c56e-192">Name</span></span>           | <span data-ttu-id="5c56e-193">Resolução</span><span class="sxs-lookup"><span data-stu-id="5c56e-193">Resolution</span></span>  | <span data-ttu-id="5c56e-194">Taxa de proporção</span><span class="sxs-lookup"><span data-stu-id="5c56e-194">Aspect Ratio</span></span> | <span data-ttu-id="5c56e-195">Descrição</span><span class="sxs-lookup"><span data-stu-id="5c56e-195">Description</span></span>                                                          |
|:---------------|:------------|:-------------|:---------------------------------------------------------------------|
| `small`        | <span data-ttu-id="5c56e-196">96 mais longa</span><span class="sxs-lookup"><span data-stu-id="5c56e-196">96 longest</span></span>  | <span data-ttu-id="5c56e-197">Original</span><span class="sxs-lookup"><span data-stu-id="5c56e-197">Original</span></span>     | <span data-ttu-id="5c56e-198">Miniatura pequena e altamente compactada, recortada em uma taxa de proporção quadrada.</span><span class="sxs-lookup"><span data-stu-id="5c56e-198">Small, highly compressed thumbnail cropped to a square aspect ratio.</span></span> |
| `medium`       | <span data-ttu-id="5c56e-199">176 mais longa</span><span class="sxs-lookup"><span data-stu-id="5c56e-199">176 longest</span></span> | <span data-ttu-id="5c56e-200">Original</span><span class="sxs-lookup"><span data-stu-id="5c56e-200">Original</span></span>     | <span data-ttu-id="5c56e-201">Recortada no tamanho do item padrão para o modo de exibição de Web do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="5c56e-201">Cropped to the standard item size for the OneDrive web view.</span></span>         |
| `large`        | <span data-ttu-id="5c56e-202">800 mais longa</span><span class="sxs-lookup"><span data-stu-id="5c56e-202">800 longest</span></span> | <span data-ttu-id="5c56e-203">Original</span><span class="sxs-lookup"><span data-stu-id="5c56e-203">Original</span></span>     | <span data-ttu-id="5c56e-204">Miniatura com a borda mais longa redimensionada para 800 pixels.</span><span class="sxs-lookup"><span data-stu-id="5c56e-204">Thumbnail with the longest edge resized to 800 pixels.</span></span>               |
| `smallSquare`  | <span data-ttu-id="5c56e-205">96x96</span><span class="sxs-lookup"><span data-stu-id="5c56e-205">96x96</span></span>       | <span data-ttu-id="5c56e-206">Corte quadrado</span><span class="sxs-lookup"><span data-stu-id="5c56e-206">Square Crop</span></span>  | <span data-ttu-id="5c56e-207">Miniatura quadrada pequena</span><span class="sxs-lookup"><span data-stu-id="5c56e-207">Small square thumbnail</span></span>                                               |
| `mediumSquare` | <span data-ttu-id="5c56e-208">176x176</span><span class="sxs-lookup"><span data-stu-id="5c56e-208">176x176</span></span>     | <span data-ttu-id="5c56e-209">Corte quadrado</span><span class="sxs-lookup"><span data-stu-id="5c56e-209">Square Crop</span></span>  | <span data-ttu-id="5c56e-210">Miniatura quadrada pequena</span><span class="sxs-lookup"><span data-stu-id="5c56e-210">Small square thumbnail</span></span>                                               |
| `largeSquare`  | <span data-ttu-id="5c56e-211">800x800</span><span class="sxs-lookup"><span data-stu-id="5c56e-211">800x800</span></span>     | <span data-ttu-id="5c56e-212">Corte quadrado</span><span class="sxs-lookup"><span data-stu-id="5c56e-212">Square Crop</span></span>  | <span data-ttu-id="5c56e-213">Miniatura quadrada grande</span><span class="sxs-lookup"><span data-stu-id="5c56e-213">Large square thumbnail</span></span>                                               |

## <a name="requesting-custom-thumbnail-sizes"></a><span data-ttu-id="5c56e-214">Solicitar tamanhos personalizados de miniaturas</span><span class="sxs-lookup"><span data-stu-id="5c56e-214">Requesting custom thumbnail sizes</span></span>

<span data-ttu-id="5c56e-215">Além dos tamanhos definidos, seu aplicativo pode solicitar um tamanho personalizado de miniatura, especificando as dimensões da miniatura prefixadas com `c`.</span><span class="sxs-lookup"><span data-stu-id="5c56e-215">In addition to the defined sizes, your app can request a custom thumbnail size by specifying the dimensions of the thumbnail prefixed with `c`.</span></span>
<span data-ttu-id="5c56e-216">Por exemplo, se o seu aplicativo precisar de miniaturas de 300 x 400, é possível solicitar esse tamanho desta forma:</span><span class="sxs-lookup"><span data-stu-id="5c56e-216">For example if your app needs thumbnails that are 300x400, it can request that size like this:</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="5c56e-217">HTTP</span><span class="sxs-lookup"><span data-stu-id="5c56e-217">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request","name": "get-thumbnail-custom-size", "scopes": "files.read" } -->

```msgraph-interactive
GET /me/drive/items/{item-id}/thumbnails?select=c300x400_Crop
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="5c56e-218">C#</span><span class="sxs-lookup"><span data-stu-id="5c56e-218">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-thumbnail-custom-size-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5c56e-219">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5c56e-219">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-thumbnail-custom-size-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5c56e-220">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5c56e-220">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-thumbnail-custom-size-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="5c56e-221">Que responde com o tamanho de miniatura personalizado selecionado:</span><span class="sxs-lookup"><span data-stu-id="5c56e-221">Which responds with just the custom thumbnail size selected:</span></span>

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

<span data-ttu-id="5c56e-222">Você pode especificar as seguintes opções após o tamanho de miniatura solicitado:</span><span class="sxs-lookup"><span data-stu-id="5c56e-222">You can specify the following options after the size of the thumbnail requested:</span></span>

### <a name="examples-of-custom-identifiers"></a><span data-ttu-id="5c56e-223">Exemplos de identificadores personalizados</span><span class="sxs-lookup"><span data-stu-id="5c56e-223">Examples of custom identifiers</span></span>

| <span data-ttu-id="5c56e-224">Identificador de miniatura</span><span class="sxs-lookup"><span data-stu-id="5c56e-224">Thumbnail identifier</span></span> | <span data-ttu-id="5c56e-225">Resolução</span><span class="sxs-lookup"><span data-stu-id="5c56e-225">Resolution</span></span>             | <span data-ttu-id="5c56e-226">Taxa de proporção</span><span class="sxs-lookup"><span data-stu-id="5c56e-226">Aspect ratio</span></span> | <span data-ttu-id="5c56e-227">Descrição</span><span class="sxs-lookup"><span data-stu-id="5c56e-227">Description</span></span>                                                                                                                                         |
|:---------------------|:-----------------------|:-------------|:----------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="5c56e-228">c300x400</span><span class="sxs-lookup"><span data-stu-id="5c56e-228">c300x400</span></span>             | <span data-ttu-id="5c56e-229">Limitado por uma caixa de 300 x 400</span><span class="sxs-lookup"><span data-stu-id="5c56e-229">Bounded by 300x400 box</span></span> | <span data-ttu-id="5c56e-230">Original</span><span class="sxs-lookup"><span data-stu-id="5c56e-230">Original</span></span>     | <span data-ttu-id="5c56e-231">Gere uma miniatura que se ajuste em uma caixa de 300 x 400 pixels, mantendo a taxa de proporção</span><span class="sxs-lookup"><span data-stu-id="5c56e-231">Generate a thumbnail that fits inside a 300x400 pixel box, maintaining aspect ratio</span></span>                                                                 |
| <span data-ttu-id="5c56e-232">c300x400_Crop</span><span class="sxs-lookup"><span data-stu-id="5c56e-232">c300x400_Crop</span></span>        | <span data-ttu-id="5c56e-233">300x400</span><span class="sxs-lookup"><span data-stu-id="5c56e-233">300x400</span></span>                | <span data-ttu-id="5c56e-234">Recortada</span><span class="sxs-lookup"><span data-stu-id="5c56e-234">Cropped</span></span>      | <span data-ttu-id="5c56e-p113">Gere uma miniatura de 300 x 400 pixels. Para isso, é preciso redimensionar a imagem para caber na caixa de 300 x 400 e recortar o que ficar fora da caixa.</span><span class="sxs-lookup"><span data-stu-id="5c56e-p113">Generate a thumbnail that is 300x400 pixels. This works by resizing the image to fill the 300x400 box and cropping whatever spills outside the box.</span></span> |

<span data-ttu-id="5c56e-237">**Observação:** talvez a miniatura retornada não corresponda exatamente às dimensões de pixel solicitadas, mas corresponderá com a taxa de proporção.</span><span class="sxs-lookup"><span data-stu-id="5c56e-237">**Note:** The thumbnail returned may not exactly match the pixel dimensions that was requested, but will match the aspect ratio.</span></span>
<span data-ttu-id="5c56e-238">Em alguns casos, uma miniatura maior do que a solicitada pode retornar, se a miniatura já existir, e pode ser facilmente dimensionada para coincidir com a resolução solicitada.</span><span class="sxs-lookup"><span data-stu-id="5c56e-238">In some cases, a larger thumbnail may be returned than was requested, if the thumbnail already exists and can easily be scaled to match the requested resolution.</span></span>

## <a name="remarks"></a><span data-ttu-id="5c56e-239">Comentários</span><span class="sxs-lookup"><span data-stu-id="5c56e-239">Remarks</span></span>

<span data-ttu-id="5c56e-240">**Observação** No OneDrive for Business e no SharePoint:</span><span class="sxs-lookup"><span data-stu-id="5c56e-240">**Note** In OneDrive for Business and SharePoint:</span></span>

<span data-ttu-id="5c56e-241">O uso dessas chamadas para expandir a coleção de miniaturas não funcionará:</span><span class="sxs-lookup"><span data-stu-id="5c56e-241">Using these calls to expand the thumbnails collection will not work:</span></span>

* `GET /drive/root:/{item-path}?expand=children(expand=thumbnails)`
* `GET /drive/items/{item-id}/children?expand=thumbnails`

<span data-ttu-id="5c56e-242">Não há suporte para miniaturas no SharePoint Server 2016.</span><span class="sxs-lookup"><span data-stu-id="5c56e-242">Thumbnails are not supported on SharePoint Server 2016.</span></span>

### <a name="error-responses"></a><span data-ttu-id="5c56e-243">Respostas de erro</span><span class="sxs-lookup"><span data-stu-id="5c56e-243">Error responses</span></span>

<span data-ttu-id="5c56e-244">Confira mais informações sobre como os erros são retornados em [Respostas de erro][error-response].</span><span class="sxs-lookup"><span data-stu-id="5c56e-244">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

[error-response]: /graph/errors

<!--
{
  "type": "#page.annotation",
  "description": "Get metadata and content for thumbnails of multiple sizes for OneDrive items.",
  "keywords": "thumbnail,content,download,sizes",
  "section": "documentation",
  "tocPath": "Items/Thumbnails",
  "suppressions": [
  ]
}
-->
