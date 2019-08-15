---
author: JeremyKelley
description: Recupere uma coleção de recursos ThumbnailSet para um recurso DriveItem.
ms.date: 09/10/2017
title: Recuperar miniaturas de um arquivo ou pasta
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 5c283a7b2e9ec1166c48af62b665a41ea1f05c1d
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36416692"
---
# <a name="list-thumbnails-for-a-driveitem"></a><span data-ttu-id="5941d-103">Listar miniaturas para um DriveItem</span><span class="sxs-lookup"><span data-stu-id="5941d-103">List thumbnails for a DriveItem</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5941d-104">Recupere uma coleção de recursos [ThumbnailSet](../resources/thumbnailset.md) para um recurso [DriveItem](../resources/driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="5941d-104">Retrieve a collection of [ThumbnailSet](../resources/thumbnailset.md) resources for a [DriveItem](../resources/driveitem.md) resource.</span></span>

<span data-ttu-id="5941d-p101">Um DriveItem pode ser representado por zero ou mais recursos [ThumbnailSet](../resources/thumbnailset.md). Cada **thumbnailSet** pode ter um ou mais objetos [**thumbnail**](../resources/thumbnail.md), que são imagens que representam o item. Por exemplo, um **thumbnailSet** podem incluir objetos **thumbnail**, como objetos comuns que incluem `small`, `medium` ou `large`.</span><span class="sxs-lookup"><span data-stu-id="5941d-p101">A DriveItem can be represented by zero or more [ThumbnailSet](../resources/thumbnailset.md) resources. Each **thumbnailSet** can have one or more [**thumbnail**](../resources/thumbnail.md) objects, which are images that represent the item. For example, a **thumbnailSet** may include **thumbnail** objects, such as common ones including `small`, `medium`, or `large`.</span></span>

<span data-ttu-id="5941d-p102">Há várias maneiras de trabalhar com miniaturas no OneDrive. Veja a seguir as mais comuns:</span><span class="sxs-lookup"><span data-stu-id="5941d-p102">There are many ways to work with thumbnails on OneDrive. Here are the most common ones:</span></span>

* <span data-ttu-id="5941d-110">Enumerar miniaturas disponíveis para um item</span><span class="sxs-lookup"><span data-stu-id="5941d-110">Enumerate available thumbnails for an item</span></span>
* <span data-ttu-id="5941d-111">Recuperar uma única miniatura para um item</span><span class="sxs-lookup"><span data-stu-id="5941d-111">Retrieve a single thumbnail for an item</span></span>
* <span data-ttu-id="5941d-112">Recuperar o conteúdo da miniatura</span><span class="sxs-lookup"><span data-stu-id="5941d-112">Retrieve thumbnail content</span></span>
* <span data-ttu-id="5941d-113">Recuperar miniaturas de vários itens em uma única solicitação</span><span class="sxs-lookup"><span data-stu-id="5941d-113">Retrieve thumbnails for multiple items in a single request</span></span>
* <span data-ttu-id="5941d-114">Recuperar tamanhos personalizados de miniaturas</span><span class="sxs-lookup"><span data-stu-id="5941d-114">Retrieve custom thumbnail sizes</span></span>
* <span data-ttu-id="5941d-115">Carregar uma miniatura personalizada para um item</span><span class="sxs-lookup"><span data-stu-id="5941d-115">Upload a custom thumbnail for an item</span></span>
* <span data-ttu-id="5941d-116">Determinar se uma miniatura personalizada carregada existe</span><span class="sxs-lookup"><span data-stu-id="5941d-116">Determine if a custom uploaded thumbnail exists</span></span>


## <a name="permissions"></a><span data-ttu-id="5941d-117">Permissões</span><span class="sxs-lookup"><span data-stu-id="5941d-117">Permissions</span></span>

<span data-ttu-id="5941d-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5941d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5941d-120">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5941d-120">Permission type</span></span>      | <span data-ttu-id="5941d-121">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5941d-121">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5941d-122">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5941d-122">Delegated (work or school account)</span></span> | <span data-ttu-id="5941d-123">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5941d-123">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="5941d-124">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5941d-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5941d-125">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5941d-125">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="5941d-126">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5941d-126">Application</span></span> | <span data-ttu-id="5941d-127">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5941d-127">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5941d-128">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5941d-128">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/thumbnails
GET /groups/{group-id}/drive/items/{item-id}/thumbnails
GET /me/drive/items/{item-id}/thumbnails
GET /sites/{site-id}/drive/items/{item-id}/thumbnails
GET /users/{user-id}/drive/items/{item-id}/thumbnails
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5941d-129">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5941d-129">Optional query parameters</span></span>

<span data-ttu-id="5941d-130">Este método oferece suporte ao [Parâmetro de consulta OData](/graph/query-parameters) `$select` para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5941d-130">This method supports the `$select` [OData puery parameter](/graph/query-parameters) to customize the response.</span></span>

## <a name="response"></a><span data-ttu-id="5941d-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="5941d-131">Response</span></span>

<span data-ttu-id="5941d-132">Se for bem-sucedido, esse método retornará um código de resposta `200 OK` e uma coleção de objetos [ThumbnailSet](../resources/thumbnailset.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5941d-132">If successful, this method returns a `200 OK` response code and collection of [ThumbnailSet](../resources/thumbnailset.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5941d-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5941d-133">Example</span></span>

<span data-ttu-id="5941d-134">Veja um exemplo da solicitação que recupera as miniaturas disponíveis de um item no OneDrive atual do usuário.</span><span class="sxs-lookup"><span data-stu-id="5941d-134">Here is an example of the request which retrieves available thumbnails for an item in the current user's OneDrive.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="5941d-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="5941d-135">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "enum-item-thumbnails", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/thumbnails
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="5941d-136">C#</span><span class="sxs-lookup"><span data-stu-id="5941d-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/enum-item-thumbnails-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5941d-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5941d-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/enum-item-thumbnails-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5941d-138">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="5941d-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/enum-item-thumbnails-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="5941d-139">Isto retorna uma matriz de **thumbnailSets** disponíveis para o item.</span><span class="sxs-lookup"><span data-stu-id="5941d-139">This returns an array of available **thumbnailSets** for the item.</span></span> <span data-ttu-id="5941d-140">Qualquer item em uma unidade pode ter zero ou mais miniaturas.</span><span class="sxs-lookup"><span data-stu-id="5941d-140">Any item in a drive can have zero or more thumbnails.</span></span>

<span data-ttu-id="5941d-p105">**Observação:** Você pode usar o parâmetro da cadeia de caracteres de consulta _select_ para controlar quais tamanhos de miniatura são retornados no **ThumbnailSet**. Por exemplo, `/thumbnails?select=medium` recupera somente miniaturas de tamanho médio.</span><span class="sxs-lookup"><span data-stu-id="5941d-p105">**Note:** You can use the _select_ query string parameter to control which thumbnail sizes are returned in the **ThumbnailSet**. For example, `/thumbnails?select=medium` retrieves only the medium sized thumbnails.</span></span>


### <a name="response"></a><span data-ttu-id="5941d-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="5941d-143">Response</span></span>

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

## <a name="get-a-single-thumbnail"></a><span data-ttu-id="5941d-144">Obter uma única miniatura</span><span class="sxs-lookup"><span data-stu-id="5941d-144">Get a single thumbnail</span></span>

<span data-ttu-id="5941d-145">Recupere os metadados de uma única miniatura e um único tamanho endereçando-os diretamente em uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="5941d-145">Retrieve the metadata for a single thumbnail and size by addressing it directly in a request.</span></span>

### <a name="http-request"></a><span data-ttu-id="5941d-146">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5941d-146">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="5941d-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="5941d-147">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-one-thumbnail", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/thumbnails/{thumb-id}/{size}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="5941d-148">C#</span><span class="sxs-lookup"><span data-stu-id="5941d-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-one-thumbnail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5941d-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5941d-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-one-thumbnail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5941d-150">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="5941d-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-one-thumbnail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="path-parameters"></a><span data-ttu-id="5941d-151">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="5941d-151">Path parameters</span></span>

| <span data-ttu-id="5941d-152">Nome</span><span class="sxs-lookup"><span data-stu-id="5941d-152">Name</span></span>         | <span data-ttu-id="5941d-153">Tipo</span><span class="sxs-lookup"><span data-stu-id="5941d-153">Type</span></span>   | <span data-ttu-id="5941d-154">Descrição</span><span class="sxs-lookup"><span data-stu-id="5941d-154">Description</span></span>                                                                              |
|:-------------|:-------|:-----------------------------------------------------------------------------------------|
| <span data-ttu-id="5941d-155">**item-id**</span><span class="sxs-lookup"><span data-stu-id="5941d-155">**item-id**</span></span>  | <span data-ttu-id="5941d-156">string</span><span class="sxs-lookup"><span data-stu-id="5941d-156">string</span></span> | <span data-ttu-id="5941d-157">O identificador exclusivo do item referenciado.</span><span class="sxs-lookup"><span data-stu-id="5941d-157">The unique identifier for the item referenced.</span></span>                                           |
| <span data-ttu-id="5941d-158">**thumb-id**</span><span class="sxs-lookup"><span data-stu-id="5941d-158">**thumb-id**</span></span> | <span data-ttu-id="5941d-159">number</span><span class="sxs-lookup"><span data-stu-id="5941d-159">number</span></span> | <span data-ttu-id="5941d-p106">O índice da miniatura, geralmente de 0 a 4. Se houver uma miniatura personalizada, seu índice será 0.</span><span class="sxs-lookup"><span data-stu-id="5941d-p106">The index of the thumbnail, usually 0-4. If there is a custom thumbnail, its index is 0.</span></span> |
| <span data-ttu-id="5941d-162">**size**</span><span class="sxs-lookup"><span data-stu-id="5941d-162">**size**</span></span>     | <span data-ttu-id="5941d-163">string</span><span class="sxs-lookup"><span data-stu-id="5941d-163">string</span></span> | <span data-ttu-id="5941d-164">O tamanho da miniatura solicitada.</span><span class="sxs-lookup"><span data-stu-id="5941d-164">The size of the thumbnail requested.</span></span> <span data-ttu-id="5941d-165">Pode ter um dos tamanhos padrão listados abaixo, ou um tamanho personalizado.</span><span class="sxs-lookup"><span data-stu-id="5941d-165">This can be one of the standard sizes listed below or a custom size.</span></span> |

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

## <a name="retrieve-thumbnail-binary-content"></a><span data-ttu-id="5941d-166">Recuperar o conteúdo binário da miniatura</span><span class="sxs-lookup"><span data-stu-id="5941d-166">Retrieve thumbnail binary content</span></span>

<span data-ttu-id="5941d-167">Você pode recuperar diretamente o conteúdo da miniatura solicitando a propriedade **content** dessa miniatura.</span><span class="sxs-lookup"><span data-stu-id="5941d-167">You can directly retrieve the content of the thumbnail by requesting the **content** property of the thumbnail.</span></span>

### <a name="http-request"></a><span data-ttu-id="5941d-168">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5941d-168">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="5941d-169">HTTP</span><span class="sxs-lookup"><span data-stu-id="5941d-169">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name":"get-thumbnail-content", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/thumbnails/{thumb-id}/{size}/content
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="5941d-170">C#</span><span class="sxs-lookup"><span data-stu-id="5941d-170">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-thumbnail-content-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5941d-171">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5941d-171">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-thumbnail-content-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5941d-172">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="5941d-172">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-thumbnail-content-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5941d-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="5941d-173">Response</span></span>

<span data-ttu-id="5941d-174">O serviço responde com um redirecionamento para a URL da miniatura.</span><span class="sxs-lookup"><span data-stu-id="5941d-174">The service responds with a redirect to the thumbnail URL.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```

<span data-ttu-id="5941d-175">URLs de miniaturas são seguras em cache.</span><span class="sxs-lookup"><span data-stu-id="5941d-175">Thumbnail URLs are cache-safe.</span></span> <span data-ttu-id="5941d-176">A URL mudará se o item for alterado de uma maneira que exigir que uma nova miniatura seja gerada.</span><span class="sxs-lookup"><span data-stu-id="5941d-176">The URL will change, if the item changes in a way that requires a new thumbnail to be generated.</span></span>


## <a name="getting-thumbnails-while-listing-driveitems"></a><span data-ttu-id="5941d-177">Obter miniaturas ao listar DriveItems</span><span class="sxs-lookup"><span data-stu-id="5941d-177">Getting thumbnails while listing DriveItems</span></span>

<span data-ttu-id="5941d-178">Se você estiver recuperando uma lista de recursos DriveItem para exibição, use o parâmetro de cadeia de consulta _$expand_ para incluir as miniaturas para esses recursos.</span><span class="sxs-lookup"><span data-stu-id="5941d-178">If you are retrieving a list of DriveItem resources to display, you can use the _$expand_ query string parameter to also include the thumbnails for those resources.</span></span>
<span data-ttu-id="5941d-179">Isso permite que seu aplicativo recupere miniaturas e itens em uma única solicitação, em vez de emitir muitas solicitações.</span><span class="sxs-lookup"><span data-stu-id="5941d-179">This enables your app to retrieve thumbnails and items in a single request, instead of issuing many requests.</span></span>

### <a name="http-request"></a><span data-ttu-id="5941d-180">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5941d-180">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="5941d-181">HTTP</span><span class="sxs-lookup"><span data-stu-id="5941d-181">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name":"get-thumbnail-while-listing", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/children?$expand=thumbnails
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="5941d-182">C#</span><span class="sxs-lookup"><span data-stu-id="5941d-182">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-thumbnail-while-listing-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5941d-183">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5941d-183">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-thumbnail-while-listing-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5941d-184">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="5941d-184">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-thumbnail-while-listing-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5941d-185">Resposta</span><span class="sxs-lookup"><span data-stu-id="5941d-185">Response</span></span>

<span data-ttu-id="5941d-186">As respostas do serviço com a lista de DriveItems e suas miniaturas.</span><span class="sxs-lookup"><span data-stu-id="5941d-186">The service responses with the list of DriveItems and their thumbnails.</span></span>

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

## <a name="size-values"></a><span data-ttu-id="5941d-187">Valores de tamanho</span><span class="sxs-lookup"><span data-stu-id="5941d-187">Size values</span></span>

<span data-ttu-id="5941d-p110">Essa tabela define os possíveis tamanhos de miniaturas. Embora você possa solicitar qualquer tamanho de miniatura arbitrário, os valores definidos provavelmente existem e retornam um valor rapidamente:</span><span class="sxs-lookup"><span data-stu-id="5941d-p110">This table defines the possible thumbnail sizes. While you can request any arbitrary thumbnail size, the defined values are likely to exist and return a value quickly:</span></span>

| <span data-ttu-id="5941d-190">Nome</span><span class="sxs-lookup"><span data-stu-id="5941d-190">Name</span></span>           | <span data-ttu-id="5941d-191">Resolução</span><span class="sxs-lookup"><span data-stu-id="5941d-191">Resolution</span></span>  | <span data-ttu-id="5941d-192">Taxa de proporção</span><span class="sxs-lookup"><span data-stu-id="5941d-192">Aspect Ratio</span></span> | <span data-ttu-id="5941d-193">Descrição</span><span class="sxs-lookup"><span data-stu-id="5941d-193">Description</span></span>                                                          |
|:---------------|:------------|:-------------|:---------------------------------------------------------------------|
| `small`        | <span data-ttu-id="5941d-194">96 mais longa</span><span class="sxs-lookup"><span data-stu-id="5941d-194">96 longest</span></span>  | <span data-ttu-id="5941d-195">Original</span><span class="sxs-lookup"><span data-stu-id="5941d-195">Original</span></span>     | <span data-ttu-id="5941d-196">Miniatura pequena e altamente compactada, recortada em uma taxa de proporção quadrada.</span><span class="sxs-lookup"><span data-stu-id="5941d-196">Small, highly compressed thumbnail cropped to a square aspect ratio.</span></span> |
| `medium`       | <span data-ttu-id="5941d-197">176 mais longa</span><span class="sxs-lookup"><span data-stu-id="5941d-197">176 longest</span></span> | <span data-ttu-id="5941d-198">Original</span><span class="sxs-lookup"><span data-stu-id="5941d-198">Original</span></span>     | <span data-ttu-id="5941d-199">Recortada no tamanho do item padrão para o modo de exibição de Web do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="5941d-199">Cropped to the standard item size for the OneDrive web view.</span></span>         |
| `large`        | <span data-ttu-id="5941d-200">800 mais longa</span><span class="sxs-lookup"><span data-stu-id="5941d-200">800 longest</span></span> | <span data-ttu-id="5941d-201">Original</span><span class="sxs-lookup"><span data-stu-id="5941d-201">Original</span></span>     | <span data-ttu-id="5941d-202">Miniatura com a borda mais longa redimensionada para 800 pixels.</span><span class="sxs-lookup"><span data-stu-id="5941d-202">Thumbnail with the longest edge resized to 800 pixels.</span></span>               |
| `smallSquare`  | <span data-ttu-id="5941d-203">96x96</span><span class="sxs-lookup"><span data-stu-id="5941d-203">96x96</span></span>       | <span data-ttu-id="5941d-204">Corte quadrado</span><span class="sxs-lookup"><span data-stu-id="5941d-204">Square Crop</span></span>  | <span data-ttu-id="5941d-205">Miniatura quadrada pequena</span><span class="sxs-lookup"><span data-stu-id="5941d-205">Small square thumbnail</span></span>                                               |
| `mediumSquare` | <span data-ttu-id="5941d-206">176x176</span><span class="sxs-lookup"><span data-stu-id="5941d-206">176x176</span></span>     | <span data-ttu-id="5941d-207">Corte quadrado</span><span class="sxs-lookup"><span data-stu-id="5941d-207">Square Crop</span></span>  | <span data-ttu-id="5941d-208">Miniatura quadrada pequena</span><span class="sxs-lookup"><span data-stu-id="5941d-208">Small square thumbnail</span></span>                                               |
| `largeSquare`  | <span data-ttu-id="5941d-209">800x800</span><span class="sxs-lookup"><span data-stu-id="5941d-209">800x800</span></span>     | <span data-ttu-id="5941d-210">Corte quadrado</span><span class="sxs-lookup"><span data-stu-id="5941d-210">Square Crop</span></span>  | <span data-ttu-id="5941d-211">Miniatura quadrada grande</span><span class="sxs-lookup"><span data-stu-id="5941d-211">Large square thumbnail</span></span>                                               |

## <a name="requesting-custom-thumbnail-sizes"></a><span data-ttu-id="5941d-212">Solicitar tamanhos personalizados de miniaturas</span><span class="sxs-lookup"><span data-stu-id="5941d-212">Requesting custom thumbnail sizes</span></span>

<span data-ttu-id="5941d-213">Além dos tamanhos definidos, seu aplicativo pode solicitar um tamanho personalizado de miniatura, especificando as dimensões da miniatura prefixadas com `c`.</span><span class="sxs-lookup"><span data-stu-id="5941d-213">In addition to the defined sizes, your app can request a custom thumbnail size by specifying the dimensions of the thumbnail prefixed with `c`.</span></span>
<span data-ttu-id="5941d-214">Por exemplo, se o seu aplicativo precisar de miniaturas de 300 x 400, é possível solicitar esse tamanho desta forma:</span><span class="sxs-lookup"><span data-stu-id="5941d-214">For example if your app needs thumbnails that are 300x400, it can request that size like this:</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="5941d-215">HTTP</span><span class="sxs-lookup"><span data-stu-id="5941d-215">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request","name": "get-thumbnail-custom-size", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/thumbnails?select=c300x400_Crop
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="5941d-216">C#</span><span class="sxs-lookup"><span data-stu-id="5941d-216">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-thumbnail-custom-size-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5941d-217">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5941d-217">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-thumbnail-custom-size-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5941d-218">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="5941d-218">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-thumbnail-custom-size-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="5941d-219">Que responde com o tamanho de miniatura personalizado selecionado:</span><span class="sxs-lookup"><span data-stu-id="5941d-219">Which responds with just the custom thumbnail size selected:</span></span>

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

<span data-ttu-id="5941d-220">Você pode especificar as seguintes opções após o tamanho de miniatura solicitado:</span><span class="sxs-lookup"><span data-stu-id="5941d-220">You can specify the following options after the size of the thumbnail requested:</span></span>

### <a name="examples-of-custom-identifiers"></a><span data-ttu-id="5941d-221">Exemplos de identificadores personalizados</span><span class="sxs-lookup"><span data-stu-id="5941d-221">Examples of custom identifiers</span></span>

| <span data-ttu-id="5941d-222">Identificador de miniatura</span><span class="sxs-lookup"><span data-stu-id="5941d-222">Thumbnail identifier</span></span> | <span data-ttu-id="5941d-223">Resolução</span><span class="sxs-lookup"><span data-stu-id="5941d-223">Resolution</span></span>             | <span data-ttu-id="5941d-224">Taxa de proporção</span><span class="sxs-lookup"><span data-stu-id="5941d-224">Aspect ratio</span></span> | <span data-ttu-id="5941d-225">Descrição</span><span class="sxs-lookup"><span data-stu-id="5941d-225">Description</span></span>                                                                                                                                         |
|:---------------------|:-----------------------|:-------------|:----------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="5941d-226">c300x400</span><span class="sxs-lookup"><span data-stu-id="5941d-226">c300x400</span></span>             | <span data-ttu-id="5941d-227">Limitado por uma caixa de 300 x 400</span><span class="sxs-lookup"><span data-stu-id="5941d-227">Bounded by 300x400 box</span></span> | <span data-ttu-id="5941d-228">Original</span><span class="sxs-lookup"><span data-stu-id="5941d-228">Original</span></span>     | <span data-ttu-id="5941d-229">Gere uma miniatura que se ajuste em uma caixa de 300 x 400 pixels, mantendo a taxa de proporção</span><span class="sxs-lookup"><span data-stu-id="5941d-229">Generate a thumbnail that fits inside a 300x400 pixel box, maintaining aspect ratio</span></span>                                                                 |
| <span data-ttu-id="5941d-230">c300x400_Crop</span><span class="sxs-lookup"><span data-stu-id="5941d-230">c300x400_Crop</span></span>        | <span data-ttu-id="5941d-231">300x400</span><span class="sxs-lookup"><span data-stu-id="5941d-231">300x400</span></span>                | <span data-ttu-id="5941d-232">Recortada</span><span class="sxs-lookup"><span data-stu-id="5941d-232">Cropped</span></span>      | <span data-ttu-id="5941d-p112">Gere uma miniatura de 300 x 400 pixels. Para isso, é preciso redimensionar a imagem para caber na caixa de 300 x 400 e recortar o que ficar fora da caixa.</span><span class="sxs-lookup"><span data-stu-id="5941d-p112">Generate a thumbnail that is 300x400 pixels. This works by resizing the image to fill the 300x400 box and cropping whatever spills outside the box.</span></span> |

<span data-ttu-id="5941d-235">**Observação:** talvez a miniatura retornada não corresponda exatamente às dimensões de pixel solicitadas, mas corresponderá com a taxa de proporção.</span><span class="sxs-lookup"><span data-stu-id="5941d-235">**Note:** The thumbnail returned may not exactly match the pixel dimensions that was requested, but will match the aspect ratio.</span></span>
<span data-ttu-id="5941d-236">Em alguns casos, uma miniatura maior do que a solicitada pode retornar, se a miniatura já existir, e pode ser facilmente dimensionada para coincidir com a resolução solicitada.</span><span class="sxs-lookup"><span data-stu-id="5941d-236">In some cases, a larger thumbnail may be returned than was requested, if the thumbnail already exists and can easily be scaled to match the requested resolution.</span></span>

## <a name="remarks"></a><span data-ttu-id="5941d-237">Comentários</span><span class="sxs-lookup"><span data-stu-id="5941d-237">Remarks</span></span>

<span data-ttu-id="5941d-238">**Observação** No OneDrive for Business e no SharePoint:</span><span class="sxs-lookup"><span data-stu-id="5941d-238">**Note** In OneDrive for Business and SharePoint:</span></span>

<span data-ttu-id="5941d-239">O uso dessas chamadas para expandir a coleção de miniaturas não funcionará:</span><span class="sxs-lookup"><span data-stu-id="5941d-239">Using these calls to expand the thumbnails collection will not work:</span></span>

* `GET /drive/root:/{item-path}?expand=children(expand=thumbnails)`
* `GET /drive/items/{item-id}/children?expand=thumbnails`

<span data-ttu-id="5941d-240">Não há suporte para miniaturas no SharePoint Server 2016.</span><span class="sxs-lookup"><span data-stu-id="5941d-240">Thumbnails are not supported on SharePoint Server 2016.</span></span>

### <a name="error-responses"></a><span data-ttu-id="5941d-241">Respostas de erro</span><span class="sxs-lookup"><span data-stu-id="5941d-241">Error responses</span></span>

<span data-ttu-id="5941d-242">Confira mais informações sobre como os erros são retornados em [Respostas de erro][error-response].</span><span class="sxs-lookup"><span data-stu-id="5941d-242">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

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
