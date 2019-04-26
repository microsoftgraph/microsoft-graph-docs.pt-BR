---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Recuperar miniaturas de um arquivo ou pasta
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 271bf311c121807bede6ba49ce2a585a7400c641
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33325309"
---
# <a name="list-thumbnails-for-a-driveitem"></a><span data-ttu-id="68a58-102">Listar miniaturas para um DriveItem</span><span class="sxs-lookup"><span data-stu-id="68a58-102">List thumbnails for a DriveItem</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="68a58-103">Recupere uma coleção de recursos [ThumbnailSet](../resources/thumbnailset.md) para um recurso [DriveItem](../resources/driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="68a58-103">Retrieve a collection of [ThumbnailSet](../resources/thumbnailset.md) resources for a [DriveItem](../resources/driveitem.md) resource.</span></span>

<span data-ttu-id="68a58-p101">Um DriveItem pode ser representado por zero ou mais recursos [ThumbnailSet](../resources/thumbnailset.md). Cada **thumbnailSet** pode ter um ou mais objetos [**thumbnail**](../resources/thumbnail.md), que são imagens que representam o item. Por exemplo, um **thumbnailSet** podem incluir objetos **thumbnail**, como objetos comuns que incluem `small`, `medium` ou `large`.</span><span class="sxs-lookup"><span data-stu-id="68a58-p101">A DriveItem can be represented by zero or more [ThumbnailSet](../resources/thumbnailset.md) resources. Each **thumbnailSet** can have one or more [**thumbnail**](../resources/thumbnail.md) objects, which are images that represent the item. For example, a **thumbnailSet** may include **thumbnail** objects, such as common ones including `small`, `medium`, or `large`.</span></span>

<span data-ttu-id="68a58-p102">Há várias maneiras de trabalhar com miniaturas no OneDrive. Veja a seguir as mais comuns:</span><span class="sxs-lookup"><span data-stu-id="68a58-p102">There are many ways to work with thumbnails on OneDrive. Here are the most common ones:</span></span>

* <span data-ttu-id="68a58-109">Enumerar miniaturas disponíveis para um item</span><span class="sxs-lookup"><span data-stu-id="68a58-109">Enumerate available thumbnails for an item</span></span>
* <span data-ttu-id="68a58-110">Recuperar uma única miniatura para um item</span><span class="sxs-lookup"><span data-stu-id="68a58-110">Retrieve a single thumbnail for an item</span></span>
* <span data-ttu-id="68a58-111">Recuperar o conteúdo da miniatura</span><span class="sxs-lookup"><span data-stu-id="68a58-111">Retrieve thumbnail content</span></span>
* <span data-ttu-id="68a58-112">Recuperar miniaturas de vários itens em uma única solicitação</span><span class="sxs-lookup"><span data-stu-id="68a58-112">Retrieve thumbnails for multiple items in a single request</span></span>
* <span data-ttu-id="68a58-113">Recuperar tamanhos personalizados de miniaturas</span><span class="sxs-lookup"><span data-stu-id="68a58-113">Retrieve custom thumbnail sizes</span></span>
* <span data-ttu-id="68a58-114">Carregar uma miniatura personalizada para um item</span><span class="sxs-lookup"><span data-stu-id="68a58-114">Upload a custom thumbnail for an item</span></span>
* <span data-ttu-id="68a58-115">Determinar se uma miniatura personalizada carregada existe</span><span class="sxs-lookup"><span data-stu-id="68a58-115">Determine if a custom uploaded thumbnail exists</span></span>


## <a name="permissions"></a><span data-ttu-id="68a58-116">Permissões</span><span class="sxs-lookup"><span data-stu-id="68a58-116">Permissions</span></span>

<span data-ttu-id="68a58-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="68a58-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="68a58-119">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="68a58-119">Permission type</span></span>      | <span data-ttu-id="68a58-120">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="68a58-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="68a58-121">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="68a58-121">Delegated (work or school account)</span></span> | <span data-ttu-id="68a58-122">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68a58-122">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="68a58-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="68a58-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="68a58-124">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68a58-124">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="68a58-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="68a58-125">Application</span></span> | <span data-ttu-id="68a58-126">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68a58-126">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="68a58-127">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="68a58-127">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/thumbnails
GET /groups/{group-id}/drive/items/{item-id}/thumbnails
GET /me/drive/items/{item-id}/thumbnails
GET /sites/{site-id}/drive/items/{item-id}/thumbnails
GET /users/{user-id}/drive/items/{item-id}/thumbnails
```

## <a name="optional-query-parameters"></a><span data-ttu-id="68a58-128">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="68a58-128">Optional query parameters</span></span>

<span data-ttu-id="68a58-129">Este método oferece suporte ao [Parâmetro de consulta OData](/graph/query-parameters) `$select` para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="68a58-129">This method supports the `$select` [OData puery parameter](/graph/query-parameters) to customize the response.</span></span>

## <a name="response"></a><span data-ttu-id="68a58-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="68a58-130">Response</span></span>

<span data-ttu-id="68a58-131">Se for bem-sucedido, esse método retornará um código de resposta `200 OK` e uma coleção de objetos [ThumbnailSet](../resources/thumbnailset.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="68a58-131">If successful, this method returns a `200 OK` response code and collection of [ThumbnailSet](../resources/thumbnailset.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="68a58-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="68a58-132">Example</span></span>

<span data-ttu-id="68a58-133">Veja um exemplo da solicitação que recupera as miniaturas disponíveis de um item no OneDrive atual do usuário.</span><span class="sxs-lookup"><span data-stu-id="68a58-133">Here is an example of the request which retrieves available thumbnails for an item in the current user's OneDrive.</span></span>

<!-- { "blockType": "request", "name": "enum-item-thumbnails", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/thumbnails
```

<span data-ttu-id="68a58-134">Isto retorna uma matriz de **thumbnailSets** disponíveis para o item.</span><span class="sxs-lookup"><span data-stu-id="68a58-134">This returns an array of available **thumbnailSets** for the item.</span></span> <span data-ttu-id="68a58-135">Qualquer item em uma unidade pode ter zero ou mais miniaturas.</span><span class="sxs-lookup"><span data-stu-id="68a58-135">Any item in a drive can have zero or more thumbnails.</span></span>

<span data-ttu-id="68a58-p105">**Observação:** Você pode usar o parâmetro da cadeia de caracteres de consulta _select_ para controlar quais tamanhos de miniatura são retornados no **ThumbnailSet**. Por exemplo, `/thumbnails?select=medium` recupera somente miniaturas de tamanho médio.</span><span class="sxs-lookup"><span data-stu-id="68a58-p105">**Note:** You can use the _select_ query string parameter to control which thumbnail sizes are returned in the **ThumbnailSet**. For example, `/thumbnails?select=medium` retrieves only the medium sized thumbnails.</span></span>


### <a name="response"></a><span data-ttu-id="68a58-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="68a58-138">Response</span></span>

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

## <a name="get-a-single-thumbnail"></a><span data-ttu-id="68a58-139">Obter uma única miniatura</span><span class="sxs-lookup"><span data-stu-id="68a58-139">Get a single thumbnail</span></span>

<span data-ttu-id="68a58-140">Recupere os metadados de uma única miniatura e um único tamanho endereçando-os diretamente em uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="68a58-140">Retrieve the metadata for a single thumbnail and size by addressing it directly in a request.</span></span>

### <a name="http-request"></a><span data-ttu-id="68a58-141">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="68a58-141">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-one-thumbnail", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/thumbnails/{thumb-id}/{size}
```

### <a name="path-parameters"></a><span data-ttu-id="68a58-142">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="68a58-142">Path parameters</span></span>

| <span data-ttu-id="68a58-143">Nome</span><span class="sxs-lookup"><span data-stu-id="68a58-143">Name</span></span>         | <span data-ttu-id="68a58-144">Tipo</span><span class="sxs-lookup"><span data-stu-id="68a58-144">Type</span></span>   | <span data-ttu-id="68a58-145">Descrição</span><span class="sxs-lookup"><span data-stu-id="68a58-145">Description</span></span>                                                                              |
|:-------------|:-------|:-----------------------------------------------------------------------------------------|
| <span data-ttu-id="68a58-146">**item-id**</span><span class="sxs-lookup"><span data-stu-id="68a58-146">**item-id**</span></span>  | <span data-ttu-id="68a58-147">string</span><span class="sxs-lookup"><span data-stu-id="68a58-147">string</span></span> | <span data-ttu-id="68a58-148">O identificador exclusivo do item referenciado.</span><span class="sxs-lookup"><span data-stu-id="68a58-148">The unique identifier for the item referenced.</span></span>                                           |
| <span data-ttu-id="68a58-149">**thumb-id**</span><span class="sxs-lookup"><span data-stu-id="68a58-149">**thumb-id**</span></span> | <span data-ttu-id="68a58-150">number</span><span class="sxs-lookup"><span data-stu-id="68a58-150">number</span></span> | <span data-ttu-id="68a58-p106">O índice da miniatura, geralmente de 0 a 4. Se houver uma miniatura personalizada, seu índice será 0.</span><span class="sxs-lookup"><span data-stu-id="68a58-p106">The index of the thumbnail, usually 0-4. If there is a custom thumbnail, its index is 0.</span></span> |
| <span data-ttu-id="68a58-153">**size**</span><span class="sxs-lookup"><span data-stu-id="68a58-153">**size**</span></span>     | <span data-ttu-id="68a58-154">string</span><span class="sxs-lookup"><span data-stu-id="68a58-154">string</span></span> | <span data-ttu-id="68a58-155">O tamanho da miniatura solicitada.</span><span class="sxs-lookup"><span data-stu-id="68a58-155">The size of the thumbnail requested.</span></span> <span data-ttu-id="68a58-156">Pode ter um dos tamanhos padrão listados abaixo, ou um tamanho personalizado.</span><span class="sxs-lookup"><span data-stu-id="68a58-156">This can be one of the standard sizes listed below or a custom size.</span></span> |

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

## <a name="retrieve-thumbnail-binary-content"></a><span data-ttu-id="68a58-157">Recuperar o conteúdo binário da miniatura</span><span class="sxs-lookup"><span data-stu-id="68a58-157">Retrieve thumbnail binary content</span></span>

<span data-ttu-id="68a58-158">Você pode recuperar diretamente o conteúdo da miniatura solicitando a propriedade **content** dessa miniatura.</span><span class="sxs-lookup"><span data-stu-id="68a58-158">You can directly retrieve the content of the thumbnail by requesting the **content** property of the thumbnail.</span></span>

### <a name="http-request"></a><span data-ttu-id="68a58-159">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="68a58-159">HTTP request</span></span>

<!-- { "blockType": "request", "name":"get-thumbnail-content", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/thumbnails/{thumb-id}/{size}/content
```

### <a name="response"></a><span data-ttu-id="68a58-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="68a58-160">Response</span></span>

<span data-ttu-id="68a58-161">O serviço responde com um redirecionamento para a URL da miniatura.</span><span class="sxs-lookup"><span data-stu-id="68a58-161">The service responds with a redirect to the thumbnail URL.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```

<span data-ttu-id="68a58-162">URLs de miniaturas são seguras em cache.</span><span class="sxs-lookup"><span data-stu-id="68a58-162">Thumbnail URLs are cache-safe.</span></span> <span data-ttu-id="68a58-163">A URL mudará se o item for alterado de uma maneira que exigir que uma nova miniatura seja gerada.</span><span class="sxs-lookup"><span data-stu-id="68a58-163">The URL will change, if the item changes in a way that requires a new thumbnail to be generated.</span></span>


## <a name="getting-thumbnails-while-listing-driveitems"></a><span data-ttu-id="68a58-164">Obter miniaturas ao listar DriveItems</span><span class="sxs-lookup"><span data-stu-id="68a58-164">Getting thumbnails while listing DriveItems</span></span>

<span data-ttu-id="68a58-165">Se você estiver recuperando uma lista de recursos DriveItem para exibição, use o parâmetro de cadeia de consulta _$expand_ para incluir as miniaturas para esses recursos.</span><span class="sxs-lookup"><span data-stu-id="68a58-165">If you are retrieving a list of DriveItem resources to display, you can use the _$expand_ query string parameter to also include the thumbnails for those resources.</span></span>
<span data-ttu-id="68a58-166">Isso permite que seu aplicativo recupere miniaturas e itens em uma única solicitação, em vez de emitir muitas solicitações.</span><span class="sxs-lookup"><span data-stu-id="68a58-166">This enables your app to retrieve thumbnails and items in a single request, instead of issuing many requests.</span></span>

### <a name="http-request"></a><span data-ttu-id="68a58-167">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="68a58-167">HTTP request</span></span>

<!-- { "blockType": "request", "name":"get-thumbnail-while-listing", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/children?$expand=thumbnails
```

### <a name="response"></a><span data-ttu-id="68a58-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="68a58-168">Response</span></span>

<span data-ttu-id="68a58-169">As respostas do serviço com a lista de DriveItems e suas miniaturas.</span><span class="sxs-lookup"><span data-stu-id="68a58-169">The service responses with the list of DriveItems and their thumbnails.</span></span>

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

## <a name="size-values"></a><span data-ttu-id="68a58-170">Valores de tamanho</span><span class="sxs-lookup"><span data-stu-id="68a58-170">Size values</span></span>

<span data-ttu-id="68a58-p110">Essa tabela define os possíveis tamanhos de miniaturas. Embora você possa solicitar qualquer tamanho de miniatura arbitrário, os valores definidos provavelmente existem e retornam um valor rapidamente:</span><span class="sxs-lookup"><span data-stu-id="68a58-p110">This table defines the possible thumbnail sizes. While you can request any arbitrary thumbnail size, the defined values are likely to exist and return a value quickly:</span></span>

| <span data-ttu-id="68a58-173">Nome</span><span class="sxs-lookup"><span data-stu-id="68a58-173">Name</span></span>           | <span data-ttu-id="68a58-174">Resolução</span><span class="sxs-lookup"><span data-stu-id="68a58-174">Resolution</span></span>  | <span data-ttu-id="68a58-175">Taxa de proporção</span><span class="sxs-lookup"><span data-stu-id="68a58-175">Aspect Ratio</span></span> | <span data-ttu-id="68a58-176">Descrição</span><span class="sxs-lookup"><span data-stu-id="68a58-176">Description</span></span>                                                          |
|:---------------|:------------|:-------------|:---------------------------------------------------------------------|
| `small`        | <span data-ttu-id="68a58-177">96 mais longa</span><span class="sxs-lookup"><span data-stu-id="68a58-177">96 longest</span></span>  | <span data-ttu-id="68a58-178">Original</span><span class="sxs-lookup"><span data-stu-id="68a58-178">Original</span></span>     | <span data-ttu-id="68a58-179">Miniatura pequena e altamente compactada, recortada em uma taxa de proporção quadrada.</span><span class="sxs-lookup"><span data-stu-id="68a58-179">Small, highly compressed thumbnail cropped to a square aspect ratio.</span></span> |
| `medium`       | <span data-ttu-id="68a58-180">176 mais longa</span><span class="sxs-lookup"><span data-stu-id="68a58-180">176 longest</span></span> | <span data-ttu-id="68a58-181">Original</span><span class="sxs-lookup"><span data-stu-id="68a58-181">Original</span></span>     | <span data-ttu-id="68a58-182">Recortada no tamanho do item padrão para o modo de exibição de Web do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="68a58-182">Cropped to the standard item size for the OneDrive web view.</span></span>         |
| `large`        | <span data-ttu-id="68a58-183">800 mais longa</span><span class="sxs-lookup"><span data-stu-id="68a58-183">800 longest</span></span> | <span data-ttu-id="68a58-184">Original</span><span class="sxs-lookup"><span data-stu-id="68a58-184">Original</span></span>     | <span data-ttu-id="68a58-185">Miniatura com a borda mais longa redimensionada para 800 pixels.</span><span class="sxs-lookup"><span data-stu-id="68a58-185">Thumbnail with the longest edge resized to 800 pixels.</span></span>               |
| `smallSquare`  | <span data-ttu-id="68a58-186">96x96</span><span class="sxs-lookup"><span data-stu-id="68a58-186">96x96</span></span>       | <span data-ttu-id="68a58-187">Corte quadrado</span><span class="sxs-lookup"><span data-stu-id="68a58-187">Square Crop</span></span>  | <span data-ttu-id="68a58-188">Miniatura quadrada pequena</span><span class="sxs-lookup"><span data-stu-id="68a58-188">Small square thumbnail</span></span>                                               |
| `mediumSquare` | <span data-ttu-id="68a58-189">176x176</span><span class="sxs-lookup"><span data-stu-id="68a58-189">176x176</span></span>     | <span data-ttu-id="68a58-190">Corte quadrado</span><span class="sxs-lookup"><span data-stu-id="68a58-190">Square Crop</span></span>  | <span data-ttu-id="68a58-191">Miniatura quadrada pequena</span><span class="sxs-lookup"><span data-stu-id="68a58-191">Small square thumbnail</span></span>                                               |
| `largeSquare`  | <span data-ttu-id="68a58-192">800x800</span><span class="sxs-lookup"><span data-stu-id="68a58-192">800x800</span></span>     | <span data-ttu-id="68a58-193">Corte quadrado</span><span class="sxs-lookup"><span data-stu-id="68a58-193">Square Crop</span></span>  | <span data-ttu-id="68a58-194">Miniatura quadrada grande</span><span class="sxs-lookup"><span data-stu-id="68a58-194">Large square thumbnail</span></span>                                               |

## <a name="requesting-custom-thumbnail-sizes"></a><span data-ttu-id="68a58-195">Solicitar tamanhos personalizados de miniaturas</span><span class="sxs-lookup"><span data-stu-id="68a58-195">Requesting custom thumbnail sizes</span></span>

<span data-ttu-id="68a58-196">Além dos tamanhos definidos, seu aplicativo pode solicitar um tamanho personalizado de miniatura, especificando as dimensões da miniatura prefixadas com `c`.</span><span class="sxs-lookup"><span data-stu-id="68a58-196">In addition to the defined sizes, your app can request a custom thumbnail size by specifying the dimensions of the thumbnail prefixed with `c`.</span></span>
<span data-ttu-id="68a58-197">Por exemplo, se o seu aplicativo precisar de miniaturas de 300 x 400, é possível solicitar esse tamanho desta forma:</span><span class="sxs-lookup"><span data-stu-id="68a58-197">For example if your app needs thumbnails that are 300x400, it can request that size like this:</span></span>

<!-- { "name": "get-thumbnail-custom-size", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/thumbnails?select=c300x400_Crop
```

<span data-ttu-id="68a58-198">Que responde com o tamanho de miniatura personalizado selecionado:</span><span class="sxs-lookup"><span data-stu-id="68a58-198">Which responds with just the custom thumbnail size selected:</span></span>

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

<span data-ttu-id="68a58-199">Você pode especificar as seguintes opções após o tamanho de miniatura solicitado:</span><span class="sxs-lookup"><span data-stu-id="68a58-199">You can specify the following options after the size of the thumbnail requested:</span></span>

### <a name="examples-of-custom-identifiers"></a><span data-ttu-id="68a58-200">Exemplos de identificadores personalizados</span><span class="sxs-lookup"><span data-stu-id="68a58-200">Examples of custom identifiers</span></span>

| <span data-ttu-id="68a58-201">Identificador de miniatura</span><span class="sxs-lookup"><span data-stu-id="68a58-201">Thumbnail identifier</span></span> | <span data-ttu-id="68a58-202">Resolução</span><span class="sxs-lookup"><span data-stu-id="68a58-202">Resolution</span></span>             | <span data-ttu-id="68a58-203">Taxa de proporção</span><span class="sxs-lookup"><span data-stu-id="68a58-203">Aspect ratio</span></span> | <span data-ttu-id="68a58-204">Descrição</span><span class="sxs-lookup"><span data-stu-id="68a58-204">Description</span></span>                                                                                                                                         |
|:---------------------|:-----------------------|:-------------|:----------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="68a58-205">c300x400</span><span class="sxs-lookup"><span data-stu-id="68a58-205">c300x400</span></span>             | <span data-ttu-id="68a58-206">Limitado por uma caixa de 300 x 400</span><span class="sxs-lookup"><span data-stu-id="68a58-206">Bounded by 300x400 box</span></span> | <span data-ttu-id="68a58-207">Original</span><span class="sxs-lookup"><span data-stu-id="68a58-207">Original</span></span>     | <span data-ttu-id="68a58-208">Gere uma miniatura que se ajuste em uma caixa de 300 x 400 pixels, mantendo a taxa de proporção</span><span class="sxs-lookup"><span data-stu-id="68a58-208">Generate a thumbnail that fits inside a 300x400 pixel box, maintaining aspect ratio</span></span>                                                                 |
| <span data-ttu-id="68a58-209">c300x400_Crop</span><span class="sxs-lookup"><span data-stu-id="68a58-209">c300x400_Crop</span></span>        | <span data-ttu-id="68a58-210">300x400</span><span class="sxs-lookup"><span data-stu-id="68a58-210">300x400</span></span>                | <span data-ttu-id="68a58-211">Recortada</span><span class="sxs-lookup"><span data-stu-id="68a58-211">Cropped</span></span>      | <span data-ttu-id="68a58-p112">Gere uma miniatura de 300 x 400 pixels. Para isso, é preciso redimensionar a imagem para caber na caixa de 300 x 400 e recortar o que ficar fora da caixa.</span><span class="sxs-lookup"><span data-stu-id="68a58-p112">Generate a thumbnail that is 300x400 pixels. This works by resizing the image to fill the 300x400 box and cropping whatever spills outside the box.</span></span> |

<span data-ttu-id="68a58-214">**Observação:** talvez a miniatura retornada não corresponda exatamente às dimensões de pixel solicitadas, mas corresponderá com a taxa de proporção.</span><span class="sxs-lookup"><span data-stu-id="68a58-214">**Note:** The thumbnail returned may not exactly match the pixel dimensions that was requested, but will match the aspect ratio.</span></span>
<span data-ttu-id="68a58-215">Em alguns casos, uma miniatura maior do que a solicitada pode retornar, se a miniatura já existir, e pode ser facilmente dimensionada para coincidir com a resolução solicitada.</span><span class="sxs-lookup"><span data-stu-id="68a58-215">In some cases, a larger thumbnail may be returned than was requested, if the thumbnail already exists and can easily be scaled to match the requested resolution.</span></span>

## <a name="remarks"></a><span data-ttu-id="68a58-216">Comentários</span><span class="sxs-lookup"><span data-stu-id="68a58-216">Remarks</span></span>

<span data-ttu-id="68a58-217">**Observação** No OneDrive for Business e no SharePoint:</span><span class="sxs-lookup"><span data-stu-id="68a58-217">**Note** In OneDrive for Business and SharePoint:</span></span>

<span data-ttu-id="68a58-218">O uso dessas chamadas para expandir a coleção de miniaturas não funcionará:</span><span class="sxs-lookup"><span data-stu-id="68a58-218">Using these calls to expand the thumbnails collection will not work:</span></span>

* `GET /drive/root:/{item-path}?expand=children(expand=thumbnails)`
* `GET /drive/items/{item-id}/children?expand=thumbnails`

<span data-ttu-id="68a58-219">Não há suporte para miniaturas no SharePoint Server 2016.</span><span class="sxs-lookup"><span data-stu-id="68a58-219">Thumbnails are not supported on SharePoint Server 2016.</span></span>

### <a name="error-responses"></a><span data-ttu-id="68a58-220">Respostas de erro</span><span class="sxs-lookup"><span data-stu-id="68a58-220">Error responses</span></span>

<span data-ttu-id="68a58-221">Confira mais informações sobre como os erros são retornados em [Respostas de erro][error-response].</span><span class="sxs-lookup"><span data-stu-id="68a58-221">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

[error-response]: /graph/errors

<!--
{
  "type": "#page.annotation",
  "description": "Get metadata and content for thumbnails of multiple sizes for OneDrive items.",
  "keywords": "thumbnail,content,download,sizes",
  "section": "documentation",
  "tocPath": "Items/Thumbnails",
  "suppressions": []
}
-->
