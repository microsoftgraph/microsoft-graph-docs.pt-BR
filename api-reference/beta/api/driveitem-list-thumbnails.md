---
author: JeremyKelley
description: Recupere uma coleção de recursos ThumbnailSet para um recurso DriveItem.
ms.date: 09/10/2017
title: Recuperar miniaturas de um arquivo ou pasta
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: be3c85dd72410b84b7fac49fe1e8794d56beab05
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42432520"
---
# <a name="list-thumbnails-for-a-driveitem"></a><span data-ttu-id="a1783-103">Listar miniaturas para um DriveItem</span><span class="sxs-lookup"><span data-stu-id="a1783-103">List thumbnails for a DriveItem</span></span>

<span data-ttu-id="a1783-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="a1783-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a1783-105">Recupere uma coleção de recursos [ThumbnailSet](../resources/thumbnailset.md) para um recurso [DriveItem](../resources/driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="a1783-105">Retrieve a collection of [ThumbnailSet](../resources/thumbnailset.md) resources for a [DriveItem](../resources/driveitem.md) resource.</span></span>

<span data-ttu-id="a1783-p101">Um DriveItem pode ser representado por zero ou mais recursos [ThumbnailSet](../resources/thumbnailset.md). Cada **thumbnailSet** pode ter um ou mais objetos [**thumbnail**](../resources/thumbnail.md), que são imagens que representam o item. Por exemplo, um **thumbnailSet** podem incluir objetos **thumbnail**, como objetos comuns que incluem `small`, `medium` ou `large`.</span><span class="sxs-lookup"><span data-stu-id="a1783-p101">A DriveItem can be represented by zero or more [ThumbnailSet](../resources/thumbnailset.md) resources. Each **thumbnailSet** can have one or more [**thumbnail**](../resources/thumbnail.md) objects, which are images that represent the item. For example, a **thumbnailSet** may include **thumbnail** objects, such as common ones including `small`, `medium`, or `large`.</span></span>

<span data-ttu-id="a1783-p102">Há várias maneiras de trabalhar com miniaturas no OneDrive. Veja a seguir as mais comuns:</span><span class="sxs-lookup"><span data-stu-id="a1783-p102">There are many ways to work with thumbnails on OneDrive. Here are the most common ones:</span></span>

* <span data-ttu-id="a1783-111">Enumerar miniaturas disponíveis para um item</span><span class="sxs-lookup"><span data-stu-id="a1783-111">Enumerate available thumbnails for an item</span></span>
* <span data-ttu-id="a1783-112">Recuperar uma única miniatura para um item</span><span class="sxs-lookup"><span data-stu-id="a1783-112">Retrieve a single thumbnail for an item</span></span>
* <span data-ttu-id="a1783-113">Recuperar o conteúdo da miniatura</span><span class="sxs-lookup"><span data-stu-id="a1783-113">Retrieve thumbnail content</span></span>
* <span data-ttu-id="a1783-114">Recuperar miniaturas de vários itens em uma única solicitação</span><span class="sxs-lookup"><span data-stu-id="a1783-114">Retrieve thumbnails for multiple items in a single request</span></span>
* <span data-ttu-id="a1783-115">Recuperar tamanhos personalizados de miniaturas</span><span class="sxs-lookup"><span data-stu-id="a1783-115">Retrieve custom thumbnail sizes</span></span>
* <span data-ttu-id="a1783-116">Carregar uma miniatura personalizada para um item</span><span class="sxs-lookup"><span data-stu-id="a1783-116">Upload a custom thumbnail for an item</span></span>
* <span data-ttu-id="a1783-117">Determinar se uma miniatura personalizada carregada existe</span><span class="sxs-lookup"><span data-stu-id="a1783-117">Determine if a custom uploaded thumbnail exists</span></span>


## <a name="permissions"></a><span data-ttu-id="a1783-118">Permissões</span><span class="sxs-lookup"><span data-stu-id="a1783-118">Permissions</span></span>

<span data-ttu-id="a1783-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a1783-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1783-121">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a1783-121">Permission type</span></span>      | <span data-ttu-id="a1783-122">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a1783-122">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a1783-123">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a1783-123">Delegated (work or school account)</span></span> | <span data-ttu-id="a1783-124">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1783-124">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="a1783-125">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a1783-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a1783-126">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1783-126">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="a1783-127">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a1783-127">Application</span></span> | <span data-ttu-id="a1783-128">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1783-128">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a1783-129">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a1783-129">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/thumbnails
GET /groups/{group-id}/drive/items/{item-id}/thumbnails
GET /me/drive/items/{item-id}/thumbnails
GET /sites/{site-id}/drive/items/{item-id}/thumbnails
GET /users/{user-id}/drive/items/{item-id}/thumbnails
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a1783-130">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a1783-130">Optional query parameters</span></span>

<span data-ttu-id="a1783-131">Este método oferece suporte ao [Parâmetro de consulta OData](/graph/query-parameters) `$select` para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a1783-131">This method supports the `$select` [OData puery parameter](/graph/query-parameters) to customize the response.</span></span>

<span data-ttu-id="a1783-132">Além disso, esse método dá suporte à recuperação da miniatura com o valor de EXIF da orientação original e sem a rotação aplicada `originalOrientation=true` acrescentando o parâmetro de consulta.</span><span class="sxs-lookup"><span data-stu-id="a1783-132">Additionally, this method supports retrieving the thumbnail with the original orientation EXIF value and without the applied rotation by appending the `originalOrientation=true` query parameter.</span></span>
<span data-ttu-id="a1783-133">No momento, isso só tem suporte no OneDrive Personal.</span><span class="sxs-lookup"><span data-stu-id="a1783-133">This is currently only supported on OneDrive Personal.</span></span>

## <a name="response"></a><span data-ttu-id="a1783-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1783-134">Response</span></span>

<span data-ttu-id="a1783-135">Se for bem-sucedido, esse método retornará um código de resposta `200 OK` e uma coleção de objetos [ThumbnailSet](../resources/thumbnailset.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a1783-135">If successful, this method returns a `200 OK` response code and collection of [ThumbnailSet](../resources/thumbnailset.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1783-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a1783-136">Example</span></span>

<span data-ttu-id="a1783-137">Veja um exemplo da solicitação que recupera as miniaturas disponíveis de um item no OneDrive atual do usuário.</span><span class="sxs-lookup"><span data-stu-id="a1783-137">Here is an example of the request which retrieves available thumbnails for an item in the current user's OneDrive.</span></span>


# <a name="http"></a>[<span data-ttu-id="a1783-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="a1783-138">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "enum-item-thumbnails", "scopes": "files.read" } -->

```msgraph-interactive
GET /me/drive/items/{item-id}/thumbnails
```
# <a name="c"></a>[<span data-ttu-id="a1783-139">C#</span><span class="sxs-lookup"><span data-stu-id="a1783-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/enum-item-thumbnails-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a1783-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a1783-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/enum-item-thumbnails-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a1783-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a1783-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/enum-item-thumbnails-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="a1783-142">Isto retorna uma matriz de **thumbnailSets** disponíveis para o item.</span><span class="sxs-lookup"><span data-stu-id="a1783-142">This returns an array of available **thumbnailSets** for the item.</span></span> <span data-ttu-id="a1783-143">Qualquer item em uma unidade pode ter zero ou mais miniaturas.</span><span class="sxs-lookup"><span data-stu-id="a1783-143">Any item in a drive can have zero or more thumbnails.</span></span>

<span data-ttu-id="a1783-p106">**Observação:** Você pode usar o parâmetro da cadeia de caracteres de consulta _select_ para controlar quais tamanhos de miniatura são retornados no **ThumbnailSet**. Por exemplo, `/thumbnails?select=medium` recupera somente miniaturas de tamanho médio.</span><span class="sxs-lookup"><span data-stu-id="a1783-p106">**Note:** You can use the _select_ query string parameter to control which thumbnail sizes are returned in the **ThumbnailSet**. For example, `/thumbnails?select=medium` retrieves only the medium sized thumbnails.</span></span>


### <a name="response"></a><span data-ttu-id="a1783-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1783-146">Response</span></span>

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

## <a name="get-a-single-thumbnail"></a><span data-ttu-id="a1783-147">Obter uma única miniatura</span><span class="sxs-lookup"><span data-stu-id="a1783-147">Get a single thumbnail</span></span>

<span data-ttu-id="a1783-148">Recupere os metadados de uma única miniatura e tamanho tratando-os diretamente em uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="a1783-148">Retrieve the metadata for a single thumbnail and size by addressing it directly in a request.</span></span>

### <a name="http-request"></a><span data-ttu-id="a1783-149">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a1783-149">HTTP request</span></span>


# <a name="http"></a>[<span data-ttu-id="a1783-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="a1783-150">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-one-thumbnail", "scopes": "files.read" } -->

```msgraph-interactive
GET /me/drive/items/{item-id}/thumbnails/{thumb-id}/{size}
```
# <a name="c"></a>[<span data-ttu-id="a1783-151">C#</span><span class="sxs-lookup"><span data-stu-id="a1783-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-one-thumbnail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a1783-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a1783-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-one-thumbnail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a1783-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a1783-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-one-thumbnail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="path-parameters"></a><span data-ttu-id="a1783-154">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="a1783-154">Path parameters</span></span>

| <span data-ttu-id="a1783-155">Name</span><span class="sxs-lookup"><span data-stu-id="a1783-155">Name</span></span>         | <span data-ttu-id="a1783-156">Tipo</span><span class="sxs-lookup"><span data-stu-id="a1783-156">Type</span></span>   | <span data-ttu-id="a1783-157">Descrição</span><span class="sxs-lookup"><span data-stu-id="a1783-157">Description</span></span>                                                                              |
|:-------------|:-------|:-----------------------------------------------------------------------------------------|
| <span data-ttu-id="a1783-158">**item-id**</span><span class="sxs-lookup"><span data-stu-id="a1783-158">**item-id**</span></span>  | <span data-ttu-id="a1783-159">string</span><span class="sxs-lookup"><span data-stu-id="a1783-159">string</span></span> | <span data-ttu-id="a1783-160">O identificador exclusivo do item referenciado.</span><span class="sxs-lookup"><span data-stu-id="a1783-160">The unique identifier for the item referenced.</span></span>                                           |
| <span data-ttu-id="a1783-161">**thumb-id**</span><span class="sxs-lookup"><span data-stu-id="a1783-161">**thumb-id**</span></span> | <span data-ttu-id="a1783-162">number</span><span class="sxs-lookup"><span data-stu-id="a1783-162">number</span></span> | <span data-ttu-id="a1783-p107">O índice da miniatura, geralmente de 0 a 4. Se houver uma miniatura personalizada, seu índice será 0.</span><span class="sxs-lookup"><span data-stu-id="a1783-p107">The index of the thumbnail, usually 0-4. If there is a custom thumbnail, its index is 0.</span></span> |
| <span data-ttu-id="a1783-165">**size**</span><span class="sxs-lookup"><span data-stu-id="a1783-165">**size**</span></span>     | <span data-ttu-id="a1783-166">string</span><span class="sxs-lookup"><span data-stu-id="a1783-166">string</span></span> | <span data-ttu-id="a1783-167">O tamanho da miniatura solicitada.</span><span class="sxs-lookup"><span data-stu-id="a1783-167">The size of the thumbnail requested.</span></span> <span data-ttu-id="a1783-168">Pode ter um dos tamanhos padrão listados abaixo, ou um tamanho personalizado.</span><span class="sxs-lookup"><span data-stu-id="a1783-168">This can be one of the standard sizes listed below or a custom size.</span></span> |

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

## <a name="retrieve-thumbnail-binary-content"></a><span data-ttu-id="a1783-169">Recuperar o conteúdo binário da miniatura</span><span class="sxs-lookup"><span data-stu-id="a1783-169">Retrieve thumbnail binary content</span></span>

<span data-ttu-id="a1783-170">Você pode recuperar diretamente o conteúdo da miniatura solicitando a propriedade **content** dessa miniatura.</span><span class="sxs-lookup"><span data-stu-id="a1783-170">You can directly retrieve the content of the thumbnail by requesting the **content** property of the thumbnail.</span></span>

### <a name="http-request"></a><span data-ttu-id="a1783-171">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a1783-171">HTTP request</span></span>


# <a name="http"></a>[<span data-ttu-id="a1783-172">HTTP</span><span class="sxs-lookup"><span data-stu-id="a1783-172">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name":"get-thumbnail-content", "scopes": "files.read" } -->

```msgraph-interactive
GET /me/drive/items/{item-id}/thumbnails/{thumb-id}/{size}/content
```
# <a name="c"></a>[<span data-ttu-id="a1783-173">C#</span><span class="sxs-lookup"><span data-stu-id="a1783-173">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-thumbnail-content-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a1783-174">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a1783-174">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-thumbnail-content-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a1783-175">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a1783-175">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-thumbnail-content-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a1783-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1783-176">Response</span></span>

<span data-ttu-id="a1783-177">O serviço responde com um redirecionamento para a URL da miniatura.</span><span class="sxs-lookup"><span data-stu-id="a1783-177">The service responds with a redirect to the thumbnail URL.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```

<span data-ttu-id="a1783-178">URLs de miniaturas são seguras em cache.</span><span class="sxs-lookup"><span data-stu-id="a1783-178">Thumbnail URLs are cache-safe.</span></span> <span data-ttu-id="a1783-179">A URL mudará se o item for alterado de uma maneira que exigir que uma nova miniatura seja gerada.</span><span class="sxs-lookup"><span data-stu-id="a1783-179">The URL will change, if the item changes in a way that requires a new thumbnail to be generated.</span></span>


## <a name="getting-thumbnails-while-listing-driveitems"></a><span data-ttu-id="a1783-180">Obter miniaturas ao listar DriveItems</span><span class="sxs-lookup"><span data-stu-id="a1783-180">Getting thumbnails while listing DriveItems</span></span>

<span data-ttu-id="a1783-181">Se você estiver recuperando uma lista de recursos DriveItem para exibição, use o parâmetro de cadeia de consulta _$expand_ para incluir as miniaturas para esses recursos.</span><span class="sxs-lookup"><span data-stu-id="a1783-181">If you are retrieving a list of DriveItem resources to display, you can use the _$expand_ query string parameter to also include the thumbnails for those resources.</span></span>
<span data-ttu-id="a1783-182">Isso permite que seu aplicativo recupere miniaturas e itens em uma única solicitação, em vez de emitir muitas solicitações.</span><span class="sxs-lookup"><span data-stu-id="a1783-182">This enables your app to retrieve thumbnails and items in a single request, instead of issuing many requests.</span></span>

### <a name="http-request"></a><span data-ttu-id="a1783-183">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a1783-183">HTTP request</span></span>


# <a name="http"></a>[<span data-ttu-id="a1783-184">HTTP</span><span class="sxs-lookup"><span data-stu-id="a1783-184">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name":"get-thumbnail-while-listing", "scopes": "files.read" } -->

```msgraph-interactive
GET /me/drive/items/{item-id}/children?$expand=thumbnails
```
# <a name="c"></a>[<span data-ttu-id="a1783-185">C#</span><span class="sxs-lookup"><span data-stu-id="a1783-185">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-thumbnail-while-listing-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a1783-186">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a1783-186">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-thumbnail-while-listing-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a1783-187">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a1783-187">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-thumbnail-while-listing-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a1783-188">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1783-188">Response</span></span>

<span data-ttu-id="a1783-189">As respostas do serviço com a lista de DriveItems e suas miniaturas.</span><span class="sxs-lookup"><span data-stu-id="a1783-189">The service responses with the list of DriveItems and their thumbnails.</span></span>

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

## <a name="size-values"></a><span data-ttu-id="a1783-190">Valores de tamanho</span><span class="sxs-lookup"><span data-stu-id="a1783-190">Size values</span></span>

<span data-ttu-id="a1783-p111">Essa tabela define os possíveis tamanhos de miniaturas. Embora você possa solicitar qualquer tamanho de miniatura arbitrário, os valores definidos provavelmente existem e retornam um valor rapidamente:</span><span class="sxs-lookup"><span data-stu-id="a1783-p111">This table defines the possible thumbnail sizes. While you can request any arbitrary thumbnail size, the defined values are likely to exist and return a value quickly:</span></span>

| <span data-ttu-id="a1783-193">Nome</span><span class="sxs-lookup"><span data-stu-id="a1783-193">Name</span></span>           | <span data-ttu-id="a1783-194">Resolução</span><span class="sxs-lookup"><span data-stu-id="a1783-194">Resolution</span></span>  | <span data-ttu-id="a1783-195">Taxa de proporção</span><span class="sxs-lookup"><span data-stu-id="a1783-195">Aspect Ratio</span></span> | <span data-ttu-id="a1783-196">Descrição</span><span class="sxs-lookup"><span data-stu-id="a1783-196">Description</span></span>                                                          |
|:---------------|:------------|:-------------|:---------------------------------------------------------------------|
| `small`        | <span data-ttu-id="a1783-197">96 mais longa</span><span class="sxs-lookup"><span data-stu-id="a1783-197">96 longest</span></span>  | <span data-ttu-id="a1783-198">Original</span><span class="sxs-lookup"><span data-stu-id="a1783-198">Original</span></span>     | <span data-ttu-id="a1783-199">Miniatura pequena e altamente compactada, recortada em uma taxa de proporção quadrada.</span><span class="sxs-lookup"><span data-stu-id="a1783-199">Small, highly compressed thumbnail cropped to a square aspect ratio.</span></span> |
| `medium`       | <span data-ttu-id="a1783-200">176 mais longa</span><span class="sxs-lookup"><span data-stu-id="a1783-200">176 longest</span></span> | <span data-ttu-id="a1783-201">Original</span><span class="sxs-lookup"><span data-stu-id="a1783-201">Original</span></span>     | <span data-ttu-id="a1783-202">Recortada no tamanho do item padrão para o modo de exibição de Web do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="a1783-202">Cropped to the standard item size for the OneDrive web view.</span></span>         |
| `large`        | <span data-ttu-id="a1783-203">800 mais longa</span><span class="sxs-lookup"><span data-stu-id="a1783-203">800 longest</span></span> | <span data-ttu-id="a1783-204">Original</span><span class="sxs-lookup"><span data-stu-id="a1783-204">Original</span></span>     | <span data-ttu-id="a1783-205">Miniatura com a borda mais longa redimensionada para 800 pixels.</span><span class="sxs-lookup"><span data-stu-id="a1783-205">Thumbnail with the longest edge resized to 800 pixels.</span></span>               |
| `smallSquare`  | <span data-ttu-id="a1783-206">96x96</span><span class="sxs-lookup"><span data-stu-id="a1783-206">96x96</span></span>       | <span data-ttu-id="a1783-207">Corte quadrado</span><span class="sxs-lookup"><span data-stu-id="a1783-207">Square Crop</span></span>  | <span data-ttu-id="a1783-208">Miniatura quadrada pequena</span><span class="sxs-lookup"><span data-stu-id="a1783-208">Small square thumbnail</span></span>                                               |
| `mediumSquare` | <span data-ttu-id="a1783-209">176x176</span><span class="sxs-lookup"><span data-stu-id="a1783-209">176x176</span></span>     | <span data-ttu-id="a1783-210">Corte quadrado</span><span class="sxs-lookup"><span data-stu-id="a1783-210">Square Crop</span></span>  | <span data-ttu-id="a1783-211">Miniatura quadrada pequena</span><span class="sxs-lookup"><span data-stu-id="a1783-211">Small square thumbnail</span></span>                                               |
| `largeSquare`  | <span data-ttu-id="a1783-212">800x800</span><span class="sxs-lookup"><span data-stu-id="a1783-212">800x800</span></span>     | <span data-ttu-id="a1783-213">Corte quadrado</span><span class="sxs-lookup"><span data-stu-id="a1783-213">Square Crop</span></span>  | <span data-ttu-id="a1783-214">Miniatura quadrada grande</span><span class="sxs-lookup"><span data-stu-id="a1783-214">Large square thumbnail</span></span>                                               |

## <a name="requesting-custom-thumbnail-sizes"></a><span data-ttu-id="a1783-215">Solicitar tamanhos personalizados de miniaturas</span><span class="sxs-lookup"><span data-stu-id="a1783-215">Requesting custom thumbnail sizes</span></span>

<span data-ttu-id="a1783-216">Além dos tamanhos definidos, seu aplicativo pode solicitar um tamanho personalizado de miniatura, especificando as dimensões da miniatura prefixadas com `c`.</span><span class="sxs-lookup"><span data-stu-id="a1783-216">In addition to the defined sizes, your app can request a custom thumbnail size by specifying the dimensions of the thumbnail prefixed with `c`.</span></span>
<span data-ttu-id="a1783-217">Por exemplo, se o seu aplicativo precisar de miniaturas de 300 x 400, é possível solicitar esse tamanho desta forma:</span><span class="sxs-lookup"><span data-stu-id="a1783-217">For example if your app needs thumbnails that are 300x400, it can request that size like this:</span></span>


# <a name="http"></a>[<span data-ttu-id="a1783-218">HTTP</span><span class="sxs-lookup"><span data-stu-id="a1783-218">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request","name": "get-thumbnail-custom-size", "scopes": "files.read" } -->

```msgraph-interactive
GET /me/drive/items/{item-id}/thumbnails?select=c300x400_Crop
```
# <a name="c"></a>[<span data-ttu-id="a1783-219">C#</span><span class="sxs-lookup"><span data-stu-id="a1783-219">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-thumbnail-custom-size-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a1783-220">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a1783-220">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-thumbnail-custom-size-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a1783-221">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a1783-221">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-thumbnail-custom-size-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="a1783-222">Que responde com o tamanho de miniatura personalizado selecionado:</span><span class="sxs-lookup"><span data-stu-id="a1783-222">Which responds with just the custom thumbnail size selected:</span></span>

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

<span data-ttu-id="a1783-223">Você pode especificar as seguintes opções após o tamanho de miniatura solicitado:</span><span class="sxs-lookup"><span data-stu-id="a1783-223">You can specify the following options after the size of the thumbnail requested:</span></span>

### <a name="examples-of-custom-identifiers"></a><span data-ttu-id="a1783-224">Exemplos de identificadores personalizados</span><span class="sxs-lookup"><span data-stu-id="a1783-224">Examples of custom identifiers</span></span>

| <span data-ttu-id="a1783-225">Identificador de miniatura</span><span class="sxs-lookup"><span data-stu-id="a1783-225">Thumbnail identifier</span></span> | <span data-ttu-id="a1783-226">Resolução</span><span class="sxs-lookup"><span data-stu-id="a1783-226">Resolution</span></span>             | <span data-ttu-id="a1783-227">Taxa de proporção</span><span class="sxs-lookup"><span data-stu-id="a1783-227">Aspect ratio</span></span> | <span data-ttu-id="a1783-228">Descrição</span><span class="sxs-lookup"><span data-stu-id="a1783-228">Description</span></span>                                                                                                                                         |
|:---------------------|:-----------------------|:-------------|:----------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="a1783-229">c300x400</span><span class="sxs-lookup"><span data-stu-id="a1783-229">c300x400</span></span>             | <span data-ttu-id="a1783-230">Limitado por uma caixa de 300 x 400</span><span class="sxs-lookup"><span data-stu-id="a1783-230">Bounded by 300x400 box</span></span> | <span data-ttu-id="a1783-231">Original</span><span class="sxs-lookup"><span data-stu-id="a1783-231">Original</span></span>     | <span data-ttu-id="a1783-232">Gere uma miniatura que se ajuste em uma caixa de 300 x 400 pixels, mantendo a taxa de proporção</span><span class="sxs-lookup"><span data-stu-id="a1783-232">Generate a thumbnail that fits inside a 300x400 pixel box, maintaining aspect ratio</span></span>                                                                 |
| <span data-ttu-id="a1783-233">c300x400_Crop</span><span class="sxs-lookup"><span data-stu-id="a1783-233">c300x400_Crop</span></span>        | <span data-ttu-id="a1783-234">300x400</span><span class="sxs-lookup"><span data-stu-id="a1783-234">300x400</span></span>                | <span data-ttu-id="a1783-235">Recortada</span><span class="sxs-lookup"><span data-stu-id="a1783-235">Cropped</span></span>      | <span data-ttu-id="a1783-p113">Gere uma miniatura de 300 x 400 pixels. Para isso, é preciso redimensionar a imagem para caber na caixa de 300 x 400 e recortar o que ficar fora da caixa.</span><span class="sxs-lookup"><span data-stu-id="a1783-p113">Generate a thumbnail that is 300x400 pixels. This works by resizing the image to fill the 300x400 box and cropping whatever spills outside the box.</span></span> |

<span data-ttu-id="a1783-238">**Observação:** talvez a miniatura retornada não corresponda exatamente às dimensões de pixel solicitadas, mas corresponderá com a taxa de proporção.</span><span class="sxs-lookup"><span data-stu-id="a1783-238">**Note:** The thumbnail returned may not exactly match the pixel dimensions that was requested, but will match the aspect ratio.</span></span>
<span data-ttu-id="a1783-239">Em alguns casos, uma miniatura maior do que a solicitada pode retornar, se a miniatura já existir, e pode ser facilmente dimensionada para coincidir com a resolução solicitada.</span><span class="sxs-lookup"><span data-stu-id="a1783-239">In some cases, a larger thumbnail may be returned than was requested, if the thumbnail already exists and can easily be scaled to match the requested resolution.</span></span>

## <a name="remarks"></a><span data-ttu-id="a1783-240">Comentários</span><span class="sxs-lookup"><span data-stu-id="a1783-240">Remarks</span></span>

<span data-ttu-id="a1783-241">**Observação** No OneDrive for Business e no SharePoint:</span><span class="sxs-lookup"><span data-stu-id="a1783-241">**Note** In OneDrive for Business and SharePoint:</span></span>

<span data-ttu-id="a1783-242">O uso dessas chamadas para expandir a coleção de miniaturas não funcionará:</span><span class="sxs-lookup"><span data-stu-id="a1783-242">Using these calls to expand the thumbnails collection will not work:</span></span>

* `GET /drive/root:/{item-path}?expand=children(expand=thumbnails)`
* `GET /drive/items/{item-id}/children?expand=thumbnails`

<span data-ttu-id="a1783-243">Não há suporte para miniaturas no SharePoint Server 2016.</span><span class="sxs-lookup"><span data-stu-id="a1783-243">Thumbnails are not supported on SharePoint Server 2016.</span></span>

### <a name="error-responses"></a><span data-ttu-id="a1783-244">Respostas de erros</span><span class="sxs-lookup"><span data-stu-id="a1783-244">Error responses</span></span>

<span data-ttu-id="a1783-245">Confira mais informações sobre como os erros são retornados em [Respostas de Erros][error-response].</span><span class="sxs-lookup"><span data-stu-id="a1783-245">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

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
