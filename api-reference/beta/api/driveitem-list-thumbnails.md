---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Recuperar miniaturas de um arquivo ou uma pasta
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 2a64b8b7af4a1be82d4f14b4eedc17efd9839bab
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27975383"
---
# <a name="list-thumbnails-for-a-driveitem"></a><span data-ttu-id="1d062-102">Listar miniaturas para um DriveItem</span><span class="sxs-lookup"><span data-stu-id="1d062-102">List thumbnails for a DriveItem</span></span>

> <span data-ttu-id="1d062-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="1d062-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1d062-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="1d062-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1d062-105">Recupere uma coleção de recursos [ThumbnailSet](../resources/thumbnailset.md) para um recurso [DriveItem](../resources/driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="1d062-105">Retrieve a collection of [ThumbnailSet](../resources/thumbnailset.md) resources for a [DriveItem](../resources/driveitem.md) resource.</span></span>

<span data-ttu-id="1d062-p102">Um DriveItem pode ser representado por zero ou mais recursos [ThumbnailSet](../resources/thumbnailset.md). Cada **thumbnailSet** pode ter um ou mais objetos [**thumbnail**](../resources/thumbnail.md), que são imagens que representam o item. Por exemplo, um **thumbnailSet** podem incluir objetos **thumbnail**, como objetos comuns que incluem `small`, `medium` ou `large`.</span><span class="sxs-lookup"><span data-stu-id="1d062-p102">A DriveItem can be represented by zero or more [ThumbnailSet](../resources/thumbnailset.md) resources. Each **thumbnailSet** can have one or more [**thumbnail**](../resources/thumbnail.md) objects, which are images that represent the item. For example, a **thumbnailSet** may include **thumbnail** objects, such as common ones including `small`, `medium`, or `large`.</span></span>

<span data-ttu-id="1d062-p103">Há várias maneiras de trabalhar com miniaturas no OneDrive. Veja a seguir as mais comuns:</span><span class="sxs-lookup"><span data-stu-id="1d062-p103">There are many ways to work with thumbnails on OneDrive. Here are the most common ones:</span></span>

* <span data-ttu-id="1d062-111">Enumerar miniaturas disponíveis para um item</span><span class="sxs-lookup"><span data-stu-id="1d062-111">Enumerate available thumbnails for an item</span></span>
* <span data-ttu-id="1d062-112">Recuperar uma única miniatura para um item</span><span class="sxs-lookup"><span data-stu-id="1d062-112">Retrieve a single thumbnail for an item</span></span>
* <span data-ttu-id="1d062-113">Recuperar o conteúdo da miniatura</span><span class="sxs-lookup"><span data-stu-id="1d062-113">Retrieve thumbnail content</span></span>
* <span data-ttu-id="1d062-114">Recuperar miniaturas de vários itens em uma única solicitação</span><span class="sxs-lookup"><span data-stu-id="1d062-114">Retrieve thumbnails for multiple items in a single request</span></span>
* <span data-ttu-id="1d062-115">Recuperar tamanhos personalizados de miniaturas</span><span class="sxs-lookup"><span data-stu-id="1d062-115">Retrieve custom thumbnail sizes</span></span>
* <span data-ttu-id="1d062-116">Carregar uma miniatura personalizada para um item</span><span class="sxs-lookup"><span data-stu-id="1d062-116">Upload a custom thumbnail for an item</span></span>
* <span data-ttu-id="1d062-117">Determinar se uma miniatura personalizada carregada existe</span><span class="sxs-lookup"><span data-stu-id="1d062-117">Determine if a custom uploaded thumbnail exists</span></span>


## <a name="permissions"></a><span data-ttu-id="1d062-118">Permissões</span><span class="sxs-lookup"><span data-stu-id="1d062-118">Permissions</span></span>

<span data-ttu-id="1d062-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1d062-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1d062-121">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1d062-121">Permission type</span></span>      | <span data-ttu-id="1d062-122">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1d062-122">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1d062-123">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1d062-123">Delegated (work or school account)</span></span> | <span data-ttu-id="1d062-124">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d062-124">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="1d062-125">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1d062-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1d062-126">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d062-126">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="1d062-127">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1d062-127">Application</span></span> | <span data-ttu-id="1d062-128">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d062-128">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1d062-129">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1d062-129">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/thumbnails
GET /groups/{group-id}/drive/items/{item-id}/thumbnails
GET /me/drive/items/{item-id}/thumbnails
GET /sites/{site-id}/drive/items/{item-id}/thumbnails
GET /users/{user-id}/drive/items/{item-id}/thumbnails
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1d062-130">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1d062-130">Optional query parameters</span></span>

<span data-ttu-id="1d062-131">Este método oferece suporte ao [Parâmetro de consulta OData](/graph/query-parameters) `$select` para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1d062-131">This method supports the `$select` [OData puery parameter](/graph/query-parameters) to customize the response.</span></span>

## <a name="response"></a><span data-ttu-id="1d062-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="1d062-132">Response</span></span>

<span data-ttu-id="1d062-133">Se for bem-sucedido, esse método retornará um código de resposta `200 OK` e uma coleção de objetos [ThumbnailSet](../resources/thumbnailset.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1d062-133">If successful, this method returns a `200 OK` response code and collection of [ThumbnailSet](../resources/thumbnailset.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1d062-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1d062-134">Example</span></span>

<span data-ttu-id="1d062-135">Veja um exemplo da solicitação que recupera as miniaturas disponíveis de um item no OneDrive atual do usuário.</span><span class="sxs-lookup"><span data-stu-id="1d062-135">Here is an example of the request which retrieves available thumbnails for an item in the current user's OneDrive.</span></span>

<!-- { "blockType": "request", "name": "enum-item-thumbnails", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/thumbnails
```

<span data-ttu-id="1d062-136">Isto retorna uma matriz de **thumbnailSets** disponíveis para o item.</span><span class="sxs-lookup"><span data-stu-id="1d062-136">This returns an array of available **thumbnailSets** for the item.</span></span> <span data-ttu-id="1d062-137">Qualquer item em uma unidade pode ter zero ou mais miniaturas.</span><span class="sxs-lookup"><span data-stu-id="1d062-137">Any item in a drive can have zero or more thumbnails.</span></span>

<span data-ttu-id="1d062-138">**Observação:** Você pode usar o parâmetro da cadeia de caracteres de consulta _select_ para controlar quais tamanhos de miniatura são retornados no **ThumbnailSet**.</span><span class="sxs-lookup"><span data-stu-id="1d062-138">**Note:** You can use the _select_ query string parameter to control which thumbnail sizes are returned in the **ThumbnailSet**.</span></span>
<span data-ttu-id="1d062-139">Por exemplo, `/thumbnails?select=medium` recupera somente miniaturas de tamanho médio.</span><span class="sxs-lookup"><span data-stu-id="1d062-139">For example, `/thumbnails?select=medium` retrieves only the medium sized thumbnails.</span></span>


### <a name="response"></a><span data-ttu-id="1d062-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="1d062-140">Response</span></span>

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

## <a name="get-a-single-thumbnail"></a><span data-ttu-id="1d062-141">Obter uma única miniatura</span><span class="sxs-lookup"><span data-stu-id="1d062-141">Get a single thumbnail</span></span>

<span data-ttu-id="1d062-142">Recupere os metadados de uma única miniatura e um único tamanho endereçando-os diretamente em uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="1d062-142">Retrieve the metadata for a single thumbnail and size by addressing it directly in a request.</span></span>

### <a name="http-request"></a><span data-ttu-id="1d062-143">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1d062-143">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-one-thumbnail", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/thumbnails/{thumb-id}/{size}
```

### <a name="path-parameters"></a><span data-ttu-id="1d062-144">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="1d062-144">Path parameters</span></span>

| <span data-ttu-id="1d062-145">Nome</span><span class="sxs-lookup"><span data-stu-id="1d062-145">Name</span></span>         | <span data-ttu-id="1d062-146">Tipo</span><span class="sxs-lookup"><span data-stu-id="1d062-146">Type</span></span>   | <span data-ttu-id="1d062-147">Descrição</span><span class="sxs-lookup"><span data-stu-id="1d062-147">Description</span></span>                                                                              |
|:-------------|:-------|:-----------------------------------------------------------------------------------------|
| <span data-ttu-id="1d062-148">**item-id**</span><span class="sxs-lookup"><span data-stu-id="1d062-148">**item-id**</span></span>  | <span data-ttu-id="1d062-149">string</span><span class="sxs-lookup"><span data-stu-id="1d062-149">string</span></span> | <span data-ttu-id="1d062-150">O identificador exclusivo do item referenciado.</span><span class="sxs-lookup"><span data-stu-id="1d062-150">The unique identifier for the item referenced.</span></span>                                           |
| <span data-ttu-id="1d062-151">**thumb-id**</span><span class="sxs-lookup"><span data-stu-id="1d062-151">**thumb-id**</span></span> | <span data-ttu-id="1d062-152">number</span><span class="sxs-lookup"><span data-stu-id="1d062-152">number</span></span> | <span data-ttu-id="1d062-153">O índice da miniatura, geralmente de 0 a 4.</span><span class="sxs-lookup"><span data-stu-id="1d062-153">The index of the thumbnail, usually 0-4.</span></span> <span data-ttu-id="1d062-154">Se houver uma miniatura personalizada, seu índice será 0.</span><span class="sxs-lookup"><span data-stu-id="1d062-154">If there is a custom thumbnail, its index is 0.</span></span> |
| <span data-ttu-id="1d062-155">**size**</span><span class="sxs-lookup"><span data-stu-id="1d062-155">**size**</span></span>     | <span data-ttu-id="1d062-156">string</span><span class="sxs-lookup"><span data-stu-id="1d062-156">string</span></span> | <span data-ttu-id="1d062-157">O tamanho da miniatura solicitada.</span><span class="sxs-lookup"><span data-stu-id="1d062-157">The size of the thumbnail requested.</span></span> <span data-ttu-id="1d062-158">Pode ter um dos tamanhos padrão listados abaixo, ou um tamanho personalizado.</span><span class="sxs-lookup"><span data-stu-id="1d062-158">This can be one of the standard sizes listed below or a custom size.</span></span> |

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

## <a name="retrieve-thumbnail-binary-content"></a><span data-ttu-id="1d062-159">Recuperar o conteúdo binário da miniatura</span><span class="sxs-lookup"><span data-stu-id="1d062-159">Retrieve thumbnail binary content</span></span>

<span data-ttu-id="1d062-160">Você pode recuperar diretamente o conteúdo da miniatura solicitando a propriedade **content** dessa miniatura.</span><span class="sxs-lookup"><span data-stu-id="1d062-160">You can directly retrieve the content of the thumbnail by requesting the **content** property of the thumbnail.</span></span>

### <a name="http-request"></a><span data-ttu-id="1d062-161">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1d062-161">HTTP request</span></span>

<!-- { "blockType": "request", "name":"get-thumbnail-content", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/thumbnails/{thumb-id}/{size}/content
```

### <a name="response"></a><span data-ttu-id="1d062-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="1d062-162">Response</span></span>

<span data-ttu-id="1d062-163">O serviço responde com um redirecionamento para a URL da miniatura.</span><span class="sxs-lookup"><span data-stu-id="1d062-163">The service responds with a redirect to the thumbnail URL.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```

<span data-ttu-id="1d062-164">URLs de miniaturas são seguras em cache.</span><span class="sxs-lookup"><span data-stu-id="1d062-164">Thumbnail URLs are cache-safe.</span></span> <span data-ttu-id="1d062-165">A URL mudará se o item for alterado de uma maneira que exigir que uma nova miniatura seja gerada.</span><span class="sxs-lookup"><span data-stu-id="1d062-165">The URL will change, if the item changes in a way that requires a new thumbnail to be generated.</span></span>


## <a name="getting-thumbnails-while-listing-driveitems"></a><span data-ttu-id="1d062-166">Obter miniaturas ao listar DriveItems</span><span class="sxs-lookup"><span data-stu-id="1d062-166">Getting thumbnails while listing DriveItems</span></span>

<span data-ttu-id="1d062-167">Se você estiver recuperando uma lista de recursos DriveItem para exibição, use o parâmetro de cadeia de consulta _$expand_ para incluir as miniaturas para esses recursos.</span><span class="sxs-lookup"><span data-stu-id="1d062-167">If you are retrieving a list of DriveItem resources to display, you can use the _$expand_ query string parameter to also include the thumbnails for those resources.</span></span>
<span data-ttu-id="1d062-168">Isso permite que seu aplicativo recupere miniaturas e itens em uma única solicitação, em vez de emitir muitas solicitações.</span><span class="sxs-lookup"><span data-stu-id="1d062-168">This enables your app to retrieve thumbnails and items in a single request, instead of issuing many requests.</span></span>

### <a name="http-request"></a><span data-ttu-id="1d062-169">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1d062-169">HTTP request</span></span>

<!-- { "blockType": "request", "name":"get-thumbnail-while-listing", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/children?$expand=thumbnails
```

### <a name="response"></a><span data-ttu-id="1d062-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="1d062-170">Response</span></span>

<span data-ttu-id="1d062-171">As respostas do serviço com a lista de DriveItems e suas miniaturas.</span><span class="sxs-lookup"><span data-stu-id="1d062-171">The service responses with the list of DriveItems and their thumbnails.</span></span>

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

## <a name="size-values"></a><span data-ttu-id="1d062-172">Valores de tamanho</span><span class="sxs-lookup"><span data-stu-id="1d062-172">Size values</span></span>

<span data-ttu-id="1d062-p111">Essa tabela define os possíveis tamanhos de miniaturas. Embora você possa solicitar qualquer tamanho de miniatura arbitrário, os valores definidos provavelmente existem e retornam um valor rapidamente:</span><span class="sxs-lookup"><span data-stu-id="1d062-p111">This table defines the possible thumbnail sizes. While you can request any arbitrary thumbnail size, the defined values are likely to exist and return a value quickly:</span></span>

| <span data-ttu-id="1d062-175">Nome</span><span class="sxs-lookup"><span data-stu-id="1d062-175">Name</span></span>           | <span data-ttu-id="1d062-176">Resolução</span><span class="sxs-lookup"><span data-stu-id="1d062-176">Resolution</span></span>  | <span data-ttu-id="1d062-177">Taxa de proporção</span><span class="sxs-lookup"><span data-stu-id="1d062-177">Aspect Ratio</span></span> | <span data-ttu-id="1d062-178">Descrição</span><span class="sxs-lookup"><span data-stu-id="1d062-178">Description</span></span>                                                          |
|:---------------|:------------|:-------------|:---------------------------------------------------------------------|
| `small`        | <span data-ttu-id="1d062-179">96 mais longa</span><span class="sxs-lookup"><span data-stu-id="1d062-179">96 longest</span></span>  | <span data-ttu-id="1d062-180">Original</span><span class="sxs-lookup"><span data-stu-id="1d062-180">Original</span></span>     | <span data-ttu-id="1d062-181">Miniatura pequena e altamente compactada, recortada em uma taxa de proporção quadrada.</span><span class="sxs-lookup"><span data-stu-id="1d062-181">Small, highly compressed thumbnail cropped to a square aspect ratio.</span></span> |
| `medium`       | <span data-ttu-id="1d062-182">176 mais longa</span><span class="sxs-lookup"><span data-stu-id="1d062-182">176 longest</span></span> | <span data-ttu-id="1d062-183">Original</span><span class="sxs-lookup"><span data-stu-id="1d062-183">Original</span></span>     | <span data-ttu-id="1d062-184">Recortada no tamanho do item padrão para o modo de exibição de Web do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="1d062-184">Cropped to the standard item size for the OneDrive web view.</span></span>         |
| `large`        | <span data-ttu-id="1d062-185">800 mais longa</span><span class="sxs-lookup"><span data-stu-id="1d062-185">800 longest</span></span> | <span data-ttu-id="1d062-186">Original</span><span class="sxs-lookup"><span data-stu-id="1d062-186">Original</span></span>     | <span data-ttu-id="1d062-187">Miniatura com a borda mais longa redimensionada para 800 pixels.</span><span class="sxs-lookup"><span data-stu-id="1d062-187">Thumbnail with the longest edge resized to 800 pixels.</span></span>               |
| `smallSquare`  | <span data-ttu-id="1d062-188">96x96</span><span class="sxs-lookup"><span data-stu-id="1d062-188">96x96</span></span>       | <span data-ttu-id="1d062-189">Corte quadrado</span><span class="sxs-lookup"><span data-stu-id="1d062-189">Square Crop</span></span>  | <span data-ttu-id="1d062-190">Miniatura quadrada pequena</span><span class="sxs-lookup"><span data-stu-id="1d062-190">Small square thumbnail</span></span>                                               |
| `mediumSquare` | <span data-ttu-id="1d062-191">176x176</span><span class="sxs-lookup"><span data-stu-id="1d062-191">176x176</span></span>     | <span data-ttu-id="1d062-192">Corte quadrado</span><span class="sxs-lookup"><span data-stu-id="1d062-192">Square Crop</span></span>  | <span data-ttu-id="1d062-193">Miniatura quadrada pequena</span><span class="sxs-lookup"><span data-stu-id="1d062-193">Small square thumbnail</span></span>                                               |
| `largeSquare`  | <span data-ttu-id="1d062-194">800x800</span><span class="sxs-lookup"><span data-stu-id="1d062-194">800x800</span></span>     | <span data-ttu-id="1d062-195">Corte quadrado</span><span class="sxs-lookup"><span data-stu-id="1d062-195">Square Crop</span></span>  | <span data-ttu-id="1d062-196">Miniatura quadrada grande</span><span class="sxs-lookup"><span data-stu-id="1d062-196">Large square thumbnail</span></span>                                               |

## <a name="requesting-custom-thumbnail-sizes"></a><span data-ttu-id="1d062-197">Solicitar tamanhos personalizados de miniaturas</span><span class="sxs-lookup"><span data-stu-id="1d062-197">Requesting custom thumbnail sizes</span></span>

<span data-ttu-id="1d062-198">Além dos tamanhos definidos, seu aplicativo pode solicitar um tamanho personalizado de miniatura, especificando as dimensões da miniatura prefixadas com `c`.</span><span class="sxs-lookup"><span data-stu-id="1d062-198">In addition to the defined sizes, your app can request a custom thumbnail size by specifying the dimensions of the thumbnail prefixed with `c`.</span></span>
<span data-ttu-id="1d062-199">Por exemplo, se o seu aplicativo precisar de miniaturas de 300 x 400, é possível solicitar esse tamanho desta forma:</span><span class="sxs-lookup"><span data-stu-id="1d062-199">For example if your app needs thumbnails that are 300x400, it can request that size like this:</span></span>

<!-- { "name": "get-thumbnail-custom-size", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/thumbnails?select=c300x400_Crop
```

<span data-ttu-id="1d062-200">Que responde com o tamanho de miniatura personalizado selecionado:</span><span class="sxs-lookup"><span data-stu-id="1d062-200">Which responds with just the custom thumbnail size selected:</span></span>

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

<span data-ttu-id="1d062-201">Você pode especificar as seguintes opções após o tamanho de miniatura solicitado:</span><span class="sxs-lookup"><span data-stu-id="1d062-201">You can specify the following options after the size of the thumbnail requested:</span></span>

### <a name="examples-of-custom-identifiers"></a><span data-ttu-id="1d062-202">Exemplos de identificadores personalizados</span><span class="sxs-lookup"><span data-stu-id="1d062-202">Examples of custom identifiers</span></span>

| <span data-ttu-id="1d062-203">Identificador de miniatura</span><span class="sxs-lookup"><span data-stu-id="1d062-203">Thumbnail identifier</span></span> | <span data-ttu-id="1d062-204">Resolução</span><span class="sxs-lookup"><span data-stu-id="1d062-204">Resolution</span></span>             | <span data-ttu-id="1d062-205">Taxa de proporção</span><span class="sxs-lookup"><span data-stu-id="1d062-205">Aspect ratio</span></span> | <span data-ttu-id="1d062-206">Descrição</span><span class="sxs-lookup"><span data-stu-id="1d062-206">Description</span></span>                                                                                                                                         |
|:---------------------|:-----------------------|:-------------|:----------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="1d062-207">c300x400</span><span class="sxs-lookup"><span data-stu-id="1d062-207">c300x400</span></span>             | <span data-ttu-id="1d062-208">Limitado por uma caixa de 300 x 400</span><span class="sxs-lookup"><span data-stu-id="1d062-208">Bounded by 300x400 box</span></span> | <span data-ttu-id="1d062-209">Original</span><span class="sxs-lookup"><span data-stu-id="1d062-209">Original</span></span>     | <span data-ttu-id="1d062-210">Gere uma miniatura que se ajuste em uma caixa de 300 x 400 pixels, mantendo a taxa de proporção</span><span class="sxs-lookup"><span data-stu-id="1d062-210">Generate a thumbnail that fits inside a 300x400 pixel box, maintaining aspect ratio</span></span>                                                                 |
| <span data-ttu-id="1d062-211">c300x400_Crop</span><span class="sxs-lookup"><span data-stu-id="1d062-211">c300x400_Crop</span></span>        | <span data-ttu-id="1d062-212">300x400</span><span class="sxs-lookup"><span data-stu-id="1d062-212">300x400</span></span>                | <span data-ttu-id="1d062-213">Recortada</span><span class="sxs-lookup"><span data-stu-id="1d062-213">Cropped</span></span>      | <span data-ttu-id="1d062-214">Gere uma miniatura de 300 x 400 pixels.</span><span class="sxs-lookup"><span data-stu-id="1d062-214">Generate a thumbnail that is 300x400 pixels.</span></span> <span data-ttu-id="1d062-215">Para isso, é preciso redimensionar a imagem para caber na caixa de 300 x 400 e recortar o que ficar fora da caixa.</span><span class="sxs-lookup"><span data-stu-id="1d062-215">This works by resizing the image to fill the 300x400 box and cropping whatever spills outside the box.</span></span> |

<span data-ttu-id="1d062-216">**Observação:** talvez a miniatura retornada não corresponda exatamente às dimensões de pixel solicitadas, mas corresponderá com a taxa de proporção.</span><span class="sxs-lookup"><span data-stu-id="1d062-216">**Note:** The thumbnail returned may not exactly match the pixel dimensions that was requested, but will match the aspect ratio.</span></span>
<span data-ttu-id="1d062-217">Em alguns casos, uma miniatura maior do que a solicitada pode retornar, se a miniatura já existir, e pode ser facilmente dimensionada para coincidir com a resolução solicitada.</span><span class="sxs-lookup"><span data-stu-id="1d062-217">In some cases, a larger thumbnail may be returned than was requested, if the thumbnail already exists and can easily be scaled to match the requested resolution.</span></span>

## <a name="remarks"></a><span data-ttu-id="1d062-218">Comentários</span><span class="sxs-lookup"><span data-stu-id="1d062-218">Remarks</span></span>

<span data-ttu-id="1d062-219">**Observação** No OneDrive for Business e no SharePoint:</span><span class="sxs-lookup"><span data-stu-id="1d062-219">**Note** In OneDrive for Business and SharePoint:</span></span>

<span data-ttu-id="1d062-220">O uso dessas chamadas para expandir a coleção de miniaturas não funcionará:</span><span class="sxs-lookup"><span data-stu-id="1d062-220">Using these calls to expand the thumbnails collection will not work:</span></span>

* `GET /drive/root:/{item-path}?expand=children(expand=thumbnails)`
* `GET /drive/items/{item-id}/children?expand=thumbnails`

<span data-ttu-id="1d062-221">Não há suporte para miniaturas no SharePoint Server 2016.</span><span class="sxs-lookup"><span data-stu-id="1d062-221">Thumbnails are not supported on SharePoint Server 2016.</span></span>

### <a name="error-responses"></a><span data-ttu-id="1d062-222">Respostas de erro</span><span class="sxs-lookup"><span data-stu-id="1d062-222">Error responses</span></span>

<span data-ttu-id="1d062-223">Confira mais informações sobre como os erros são retornados em [Respostas de erro][error-response].</span><span class="sxs-lookup"><span data-stu-id="1d062-223">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Get metadata and content for thumbnails of multiple sizes for OneDrive items.",
  "keywords": "thumbnail,content,download,sizes",
  "section": "documentation",
  "tocPath": "Items/Thumbnails"
} -->
