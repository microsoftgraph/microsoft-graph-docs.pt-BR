---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Recuperar miniaturas de um arquivo ou pasta
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: a8d53ba41fda9c915e8eec799e1cd96805e4dc0c
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35260095"
---
# <a name="list-thumbnails-for-a-driveitem"></a><span data-ttu-id="2c6f4-102">Listar miniaturas para um DriveItem</span><span class="sxs-lookup"><span data-stu-id="2c6f4-102">List thumbnails for a DriveItem</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2c6f4-103">Recupere uma coleção de recursos [ThumbnailSet](../resources/thumbnailset.md) para um recurso [DriveItem](../resources/driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="2c6f4-103">Retrieve a collection of [ThumbnailSet](../resources/thumbnailset.md) resources for a [DriveItem](../resources/driveitem.md) resource.</span></span>

<span data-ttu-id="2c6f4-p101">Um DriveItem pode ser representado por zero ou mais recursos [ThumbnailSet](../resources/thumbnailset.md). Cada **thumbnailSet** pode ter um ou mais objetos [**thumbnail**](../resources/thumbnail.md), que são imagens que representam o item. Por exemplo, um **thumbnailSet** podem incluir objetos **thumbnail**, como objetos comuns que incluem `small`, `medium` ou `large`.</span><span class="sxs-lookup"><span data-stu-id="2c6f4-p101">A DriveItem can be represented by zero or more [ThumbnailSet](../resources/thumbnailset.md) resources. Each **thumbnailSet** can have one or more [**thumbnail**](../resources/thumbnail.md) objects, which are images that represent the item. For example, a **thumbnailSet** may include **thumbnail** objects, such as common ones including `small`, `medium`, or `large`.</span></span>

<span data-ttu-id="2c6f4-p102">Há várias maneiras de trabalhar com miniaturas no OneDrive. Veja a seguir as mais comuns:</span><span class="sxs-lookup"><span data-stu-id="2c6f4-p102">There are many ways to work with thumbnails on OneDrive. Here are the most common ones:</span></span>

* <span data-ttu-id="2c6f4-109">Enumerar miniaturas disponíveis para um item</span><span class="sxs-lookup"><span data-stu-id="2c6f4-109">Enumerate available thumbnails for an item</span></span>
* <span data-ttu-id="2c6f4-110">Recuperar uma única miniatura para um item</span><span class="sxs-lookup"><span data-stu-id="2c6f4-110">Retrieve a single thumbnail for an item</span></span>
* <span data-ttu-id="2c6f4-111">Recuperar o conteúdo da miniatura</span><span class="sxs-lookup"><span data-stu-id="2c6f4-111">Retrieve thumbnail content</span></span>
* <span data-ttu-id="2c6f4-112">Recuperar miniaturas de vários itens em uma única solicitação</span><span class="sxs-lookup"><span data-stu-id="2c6f4-112">Retrieve thumbnails for multiple items in a single request</span></span>
* <span data-ttu-id="2c6f4-113">Recuperar tamanhos personalizados de miniaturas</span><span class="sxs-lookup"><span data-stu-id="2c6f4-113">Retrieve custom thumbnail sizes</span></span>
* <span data-ttu-id="2c6f4-114">Carregar uma miniatura personalizada para um item</span><span class="sxs-lookup"><span data-stu-id="2c6f4-114">Upload a custom thumbnail for an item</span></span>
* <span data-ttu-id="2c6f4-115">Determinar se uma miniatura personalizada carregada existe</span><span class="sxs-lookup"><span data-stu-id="2c6f4-115">Determine if a custom uploaded thumbnail exists</span></span>


## <a name="permissions"></a><span data-ttu-id="2c6f4-116">Permissões</span><span class="sxs-lookup"><span data-stu-id="2c6f4-116">Permissions</span></span>

<span data-ttu-id="2c6f4-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2c6f4-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2c6f4-119">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2c6f4-119">Permission type</span></span>      | <span data-ttu-id="2c6f4-120">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2c6f4-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2c6f4-121">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2c6f4-121">Delegated (work or school account)</span></span> | <span data-ttu-id="2c6f4-122">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c6f4-122">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="2c6f4-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2c6f4-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2c6f4-124">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c6f4-124">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="2c6f4-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2c6f4-125">Application</span></span> | <span data-ttu-id="2c6f4-126">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c6f4-126">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2c6f4-127">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2c6f4-127">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/thumbnails
GET /groups/{group-id}/drive/items/{item-id}/thumbnails
GET /me/drive/items/{item-id}/thumbnails
GET /sites/{site-id}/drive/items/{item-id}/thumbnails
GET /users/{user-id}/drive/items/{item-id}/thumbnails
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2c6f4-128">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2c6f4-128">Optional query parameters</span></span>

<span data-ttu-id="2c6f4-129">Este método oferece suporte ao [Parâmetro de consulta OData](/graph/query-parameters) `$select` para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2c6f4-129">This method supports the `$select` [OData puery parameter](/graph/query-parameters) to customize the response.</span></span>

## <a name="response"></a><span data-ttu-id="2c6f4-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="2c6f4-130">Response</span></span>

<span data-ttu-id="2c6f4-131">Se for bem-sucedido, esse método retornará um código de resposta `200 OK` e uma coleção de objetos [ThumbnailSet](../resources/thumbnailset.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2c6f4-131">If successful, this method returns a `200 OK` response code and collection of [ThumbnailSet](../resources/thumbnailset.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2c6f4-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2c6f4-132">Example</span></span>

<span data-ttu-id="2c6f4-133">Veja um exemplo da solicitação que recupera as miniaturas disponíveis de um item no OneDrive atual do usuário.</span><span class="sxs-lookup"><span data-stu-id="2c6f4-133">Here is an example of the request which retrieves available thumbnails for an item in the current user's OneDrive.</span></span>

<!-- { "blockType": "request", "name": "enum-item-thumbnails", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/thumbnails
```

<span data-ttu-id="2c6f4-134">Isto retorna uma matriz de **thumbnailSets** disponíveis para o item.</span><span class="sxs-lookup"><span data-stu-id="2c6f4-134">This returns an array of available **thumbnailSets** for the item.</span></span> <span data-ttu-id="2c6f4-135">Qualquer item em uma unidade pode ter zero ou mais miniaturas.</span><span class="sxs-lookup"><span data-stu-id="2c6f4-135">Any item in a drive can have zero or more thumbnails.</span></span>

<span data-ttu-id="2c6f4-p105">**Observação:** Você pode usar o parâmetro da cadeia de caracteres de consulta _select_ para controlar quais tamanhos de miniatura são retornados no **ThumbnailSet**. Por exemplo, `/thumbnails?select=medium` recupera somente miniaturas de tamanho médio.</span><span class="sxs-lookup"><span data-stu-id="2c6f4-p105">**Note:** You can use the _select_ query string parameter to control which thumbnail sizes are returned in the **ThumbnailSet**. For example, `/thumbnails?select=medium` retrieves only the medium sized thumbnails.</span></span>


### <a name="response"></a><span data-ttu-id="2c6f4-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="2c6f4-138">Response</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="2c6f4-139">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="2c6f4-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="2c6f4-140">C#</span><span class="sxs-lookup"><span data-stu-id="2c6f4-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/enum-item-thumbnails-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2c6f4-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="2c6f4-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/enum-item-thumbnails-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="2c6f4-142">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="2c6f4-142">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/enum-item-thumbnails-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="get-a-single-thumbnail"></a><span data-ttu-id="2c6f4-143">Obter uma única miniatura</span><span class="sxs-lookup"><span data-stu-id="2c6f4-143">Get a single thumbnail</span></span>

<span data-ttu-id="2c6f4-144">Recupere os metadados de uma única miniatura e um único tamanho endereçando-os diretamente em uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="2c6f4-144">Retrieve the metadata for a single thumbnail and size by addressing it directly in a request.</span></span>

### <a name="http-request"></a><span data-ttu-id="2c6f4-145">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2c6f4-145">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-one-thumbnail", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/thumbnails/{thumb-id}/{size}
```

### <a name="path-parameters"></a><span data-ttu-id="2c6f4-146">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="2c6f4-146">Path parameters</span></span>

| <span data-ttu-id="2c6f4-147">Nome</span><span class="sxs-lookup"><span data-stu-id="2c6f4-147">Name</span></span>         | <span data-ttu-id="2c6f4-148">Tipo</span><span class="sxs-lookup"><span data-stu-id="2c6f4-148">Type</span></span>   | <span data-ttu-id="2c6f4-149">Descrição</span><span class="sxs-lookup"><span data-stu-id="2c6f4-149">Description</span></span>                                                                              |
|:-------------|:-------|:-----------------------------------------------------------------------------------------|
| <span data-ttu-id="2c6f4-150">**item-id**</span><span class="sxs-lookup"><span data-stu-id="2c6f4-150">**item-id**</span></span>  | <span data-ttu-id="2c6f4-151">string</span><span class="sxs-lookup"><span data-stu-id="2c6f4-151">string</span></span> | <span data-ttu-id="2c6f4-152">O identificador exclusivo do item referenciado.</span><span class="sxs-lookup"><span data-stu-id="2c6f4-152">The unique identifier for the item referenced.</span></span>                                           |
| <span data-ttu-id="2c6f4-153">**thumb-id**</span><span class="sxs-lookup"><span data-stu-id="2c6f4-153">**thumb-id**</span></span> | <span data-ttu-id="2c6f4-154">number</span><span class="sxs-lookup"><span data-stu-id="2c6f4-154">number</span></span> | <span data-ttu-id="2c6f4-p106">O índice da miniatura, geralmente de 0 a 4. Se houver uma miniatura personalizada, seu índice será 0.</span><span class="sxs-lookup"><span data-stu-id="2c6f4-p106">The index of the thumbnail, usually 0-4. If there is a custom thumbnail, its index is 0.</span></span> |
| <span data-ttu-id="2c6f4-157">**size**</span><span class="sxs-lookup"><span data-stu-id="2c6f4-157">**size**</span></span>     | <span data-ttu-id="2c6f4-158">string</span><span class="sxs-lookup"><span data-stu-id="2c6f4-158">string</span></span> | <span data-ttu-id="2c6f4-159">O tamanho da miniatura solicitada.</span><span class="sxs-lookup"><span data-stu-id="2c6f4-159">The size of the thumbnail requested.</span></span> <span data-ttu-id="2c6f4-160">Pode ter um dos tamanhos padrão listados abaixo, ou um tamanho personalizado.</span><span class="sxs-lookup"><span data-stu-id="2c6f4-160">This can be one of the standard sizes listed below or a custom size.</span></span> |

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="2c6f4-161">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="2c6f4-161">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="2c6f4-162">C#</span><span class="sxs-lookup"><span data-stu-id="2c6f4-162">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-one-thumbnail-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2c6f4-163">Javascript</span><span class="sxs-lookup"><span data-stu-id="2c6f4-163">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-one-thumbnail-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="2c6f4-164">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="2c6f4-164">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get-one-thumbnail-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="retrieve-thumbnail-binary-content"></a><span data-ttu-id="2c6f4-165">Recuperar o conteúdo binário da miniatura</span><span class="sxs-lookup"><span data-stu-id="2c6f4-165">Retrieve thumbnail binary content</span></span>

<span data-ttu-id="2c6f4-166">Você pode recuperar diretamente o conteúdo da miniatura solicitando a propriedade **content** dessa miniatura.</span><span class="sxs-lookup"><span data-stu-id="2c6f4-166">You can directly retrieve the content of the thumbnail by requesting the **content** property of the thumbnail.</span></span>

### <a name="http-request"></a><span data-ttu-id="2c6f4-167">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2c6f4-167">HTTP request</span></span>

<!-- { "blockType": "request", "name":"get-thumbnail-content", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/thumbnails/{thumb-id}/{size}/content
```

### <a name="response"></a><span data-ttu-id="2c6f4-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="2c6f4-168">Response</span></span>

<span data-ttu-id="2c6f4-169">O serviço responde com um redirecionamento para a URL da miniatura.</span><span class="sxs-lookup"><span data-stu-id="2c6f4-169">The service responds with a redirect to the thumbnail URL.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="2c6f4-170">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="2c6f4-170">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="2c6f4-171">C#</span><span class="sxs-lookup"><span data-stu-id="2c6f4-171">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-thumbnail-content-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2c6f4-172">Javascript</span><span class="sxs-lookup"><span data-stu-id="2c6f4-172">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-thumbnail-content-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="2c6f4-173">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="2c6f4-173">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get-thumbnail-content-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="2c6f4-174">URLs de miniaturas são seguras em cache.</span><span class="sxs-lookup"><span data-stu-id="2c6f4-174">Thumbnail URLs are cache-safe.</span></span> <span data-ttu-id="2c6f4-175">A URL mudará se o item for alterado de uma maneira que exigir que uma nova miniatura seja gerada.</span><span class="sxs-lookup"><span data-stu-id="2c6f4-175">The URL will change, if the item changes in a way that requires a new thumbnail to be generated.</span></span>


## <a name="getting-thumbnails-while-listing-driveitems"></a><span data-ttu-id="2c6f4-176">Obter miniaturas ao listar DriveItems</span><span class="sxs-lookup"><span data-stu-id="2c6f4-176">Getting thumbnails while listing DriveItems</span></span>

<span data-ttu-id="2c6f4-177">Se você estiver recuperando uma lista de recursos DriveItem para exibição, use o parâmetro de cadeia de consulta _$expand_ para incluir as miniaturas para esses recursos.</span><span class="sxs-lookup"><span data-stu-id="2c6f4-177">If you are retrieving a list of DriveItem resources to display, you can use the _$expand_ query string parameter to also include the thumbnails for those resources.</span></span>
<span data-ttu-id="2c6f4-178">Isso permite que seu aplicativo recupere miniaturas e itens em uma única solicitação, em vez de emitir muitas solicitações.</span><span class="sxs-lookup"><span data-stu-id="2c6f4-178">This enables your app to retrieve thumbnails and items in a single request, instead of issuing many requests.</span></span>

### <a name="http-request"></a><span data-ttu-id="2c6f4-179">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2c6f4-179">HTTP request</span></span>

<!-- { "blockType": "request", "name":"get-thumbnail-while-listing", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/children?$expand=thumbnails
```

### <a name="response"></a><span data-ttu-id="2c6f4-180">Resposta</span><span class="sxs-lookup"><span data-stu-id="2c6f4-180">Response</span></span>

<span data-ttu-id="2c6f4-181">As respostas do serviço com a lista de DriveItems e suas miniaturas.</span><span class="sxs-lookup"><span data-stu-id="2c6f4-181">The service responses with the list of DriveItems and their thumbnails.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="2c6f4-182">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="2c6f4-182">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="2c6f4-183">C#</span><span class="sxs-lookup"><span data-stu-id="2c6f4-183">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-thumbnail-while-listing-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2c6f4-184">Javascript</span><span class="sxs-lookup"><span data-stu-id="2c6f4-184">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-thumbnail-while-listing-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="2c6f4-185">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="2c6f4-185">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get-thumbnail-while-listing-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="size-values"></a><span data-ttu-id="2c6f4-186">Valores de tamanho</span><span class="sxs-lookup"><span data-stu-id="2c6f4-186">Size values</span></span>

<span data-ttu-id="2c6f4-p110">Essa tabela define os possíveis tamanhos de miniaturas. Embora você possa solicitar qualquer tamanho de miniatura arbitrário, os valores definidos provavelmente existem e retornam um valor rapidamente:</span><span class="sxs-lookup"><span data-stu-id="2c6f4-p110">This table defines the possible thumbnail sizes. While you can request any arbitrary thumbnail size, the defined values are likely to exist and return a value quickly:</span></span>

| <span data-ttu-id="2c6f4-189">Nome</span><span class="sxs-lookup"><span data-stu-id="2c6f4-189">Name</span></span>           | <span data-ttu-id="2c6f4-190">Resolução</span><span class="sxs-lookup"><span data-stu-id="2c6f4-190">Resolution</span></span>  | <span data-ttu-id="2c6f4-191">Taxa de proporção</span><span class="sxs-lookup"><span data-stu-id="2c6f4-191">Aspect Ratio</span></span> | <span data-ttu-id="2c6f4-192">Descrição</span><span class="sxs-lookup"><span data-stu-id="2c6f4-192">Description</span></span>                                                          |
|:---------------|:------------|:-------------|:---------------------------------------------------------------------|
| `small`        | <span data-ttu-id="2c6f4-193">96 mais longa</span><span class="sxs-lookup"><span data-stu-id="2c6f4-193">96 longest</span></span>  | <span data-ttu-id="2c6f4-194">Original</span><span class="sxs-lookup"><span data-stu-id="2c6f4-194">Original</span></span>     | <span data-ttu-id="2c6f4-195">Miniatura pequena e altamente compactada, recortada em uma taxa de proporção quadrada.</span><span class="sxs-lookup"><span data-stu-id="2c6f4-195">Small, highly compressed thumbnail cropped to a square aspect ratio.</span></span> |
| `medium`       | <span data-ttu-id="2c6f4-196">176 mais longa</span><span class="sxs-lookup"><span data-stu-id="2c6f4-196">176 longest</span></span> | <span data-ttu-id="2c6f4-197">Original</span><span class="sxs-lookup"><span data-stu-id="2c6f4-197">Original</span></span>     | <span data-ttu-id="2c6f4-198">Recortada no tamanho do item padrão para o modo de exibição de Web do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="2c6f4-198">Cropped to the standard item size for the OneDrive web view.</span></span>         |
| `large`        | <span data-ttu-id="2c6f4-199">800 mais longa</span><span class="sxs-lookup"><span data-stu-id="2c6f4-199">800 longest</span></span> | <span data-ttu-id="2c6f4-200">Original</span><span class="sxs-lookup"><span data-stu-id="2c6f4-200">Original</span></span>     | <span data-ttu-id="2c6f4-201">Miniatura com a borda mais longa redimensionada para 800 pixels.</span><span class="sxs-lookup"><span data-stu-id="2c6f4-201">Thumbnail with the longest edge resized to 800 pixels.</span></span>               |
| `smallSquare`  | <span data-ttu-id="2c6f4-202">96x96</span><span class="sxs-lookup"><span data-stu-id="2c6f4-202">96x96</span></span>       | <span data-ttu-id="2c6f4-203">Corte quadrado</span><span class="sxs-lookup"><span data-stu-id="2c6f4-203">Square Crop</span></span>  | <span data-ttu-id="2c6f4-204">Miniatura quadrada pequena</span><span class="sxs-lookup"><span data-stu-id="2c6f4-204">Small square thumbnail</span></span>                                               |
| `mediumSquare` | <span data-ttu-id="2c6f4-205">176x176</span><span class="sxs-lookup"><span data-stu-id="2c6f4-205">176x176</span></span>     | <span data-ttu-id="2c6f4-206">Corte quadrado</span><span class="sxs-lookup"><span data-stu-id="2c6f4-206">Square Crop</span></span>  | <span data-ttu-id="2c6f4-207">Miniatura quadrada pequena</span><span class="sxs-lookup"><span data-stu-id="2c6f4-207">Small square thumbnail</span></span>                                               |
| `largeSquare`  | <span data-ttu-id="2c6f4-208">800x800</span><span class="sxs-lookup"><span data-stu-id="2c6f4-208">800x800</span></span>     | <span data-ttu-id="2c6f4-209">Corte quadrado</span><span class="sxs-lookup"><span data-stu-id="2c6f4-209">Square Crop</span></span>  | <span data-ttu-id="2c6f4-210">Miniatura quadrada grande</span><span class="sxs-lookup"><span data-stu-id="2c6f4-210">Large square thumbnail</span></span>                                               |

## <a name="requesting-custom-thumbnail-sizes"></a><span data-ttu-id="2c6f4-211">Solicitar tamanhos personalizados de miniaturas</span><span class="sxs-lookup"><span data-stu-id="2c6f4-211">Requesting custom thumbnail sizes</span></span>

<span data-ttu-id="2c6f4-212">Além dos tamanhos definidos, seu aplicativo pode solicitar um tamanho personalizado de miniatura, especificando as dimensões da miniatura prefixadas com `c`.</span><span class="sxs-lookup"><span data-stu-id="2c6f4-212">In addition to the defined sizes, your app can request a custom thumbnail size by specifying the dimensions of the thumbnail prefixed with `c`.</span></span>
<span data-ttu-id="2c6f4-213">Por exemplo, se o seu aplicativo precisar de miniaturas de 300 x 400, é possível solicitar esse tamanho desta forma:</span><span class="sxs-lookup"><span data-stu-id="2c6f4-213">For example if your app needs thumbnails that are 300x400, it can request that size like this:</span></span>

<!-- { "name": "get-thumbnail-custom-size", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/thumbnails?select=c300x400_Crop
```

<span data-ttu-id="2c6f4-214">Que responde com o tamanho de miniatura personalizado selecionado:</span><span class="sxs-lookup"><span data-stu-id="2c6f4-214">Which responds with just the custom thumbnail size selected:</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="2c6f4-215">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="2c6f4-215">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="2c6f4-216">C#</span><span class="sxs-lookup"><span data-stu-id="2c6f4-216">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-thumbnail-custom-size-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2c6f4-217">Javascript</span><span class="sxs-lookup"><span data-stu-id="2c6f4-217">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-thumbnail-custom-size-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="2c6f4-218">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="2c6f4-218">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get-thumbnail-custom-size-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="2c6f4-219">Você pode especificar as seguintes opções após o tamanho de miniatura solicitado:</span><span class="sxs-lookup"><span data-stu-id="2c6f4-219">You can specify the following options after the size of the thumbnail requested:</span></span>

### <a name="examples-of-custom-identifiers"></a><span data-ttu-id="2c6f4-220">Exemplos de identificadores personalizados</span><span class="sxs-lookup"><span data-stu-id="2c6f4-220">Examples of custom identifiers</span></span>

| <span data-ttu-id="2c6f4-221">Identificador de miniatura</span><span class="sxs-lookup"><span data-stu-id="2c6f4-221">Thumbnail identifier</span></span> | <span data-ttu-id="2c6f4-222">Resolução</span><span class="sxs-lookup"><span data-stu-id="2c6f4-222">Resolution</span></span>             | <span data-ttu-id="2c6f4-223">Taxa de proporção</span><span class="sxs-lookup"><span data-stu-id="2c6f4-223">Aspect ratio</span></span> | <span data-ttu-id="2c6f4-224">Descrição</span><span class="sxs-lookup"><span data-stu-id="2c6f4-224">Description</span></span>                                                                                                                                         |
|:---------------------|:-----------------------|:-------------|:----------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="2c6f4-225">c300x400</span><span class="sxs-lookup"><span data-stu-id="2c6f4-225">c300x400</span></span>             | <span data-ttu-id="2c6f4-226">Limitado por uma caixa de 300 x 400</span><span class="sxs-lookup"><span data-stu-id="2c6f4-226">Bounded by 300x400 box</span></span> | <span data-ttu-id="2c6f4-227">Original</span><span class="sxs-lookup"><span data-stu-id="2c6f4-227">Original</span></span>     | <span data-ttu-id="2c6f4-228">Gere uma miniatura que se ajuste em uma caixa de 300 x 400 pixels, mantendo a taxa de proporção</span><span class="sxs-lookup"><span data-stu-id="2c6f4-228">Generate a thumbnail that fits inside a 300x400 pixel box, maintaining aspect ratio</span></span>                                                                 |
| <span data-ttu-id="2c6f4-229">c300x400_Crop</span><span class="sxs-lookup"><span data-stu-id="2c6f4-229">c300x400_Crop</span></span>        | <span data-ttu-id="2c6f4-230">300x400</span><span class="sxs-lookup"><span data-stu-id="2c6f4-230">300x400</span></span>                | <span data-ttu-id="2c6f4-231">Recortada</span><span class="sxs-lookup"><span data-stu-id="2c6f4-231">Cropped</span></span>      | <span data-ttu-id="2c6f4-p112">Gere uma miniatura de 300 x 400 pixels. Para isso, é preciso redimensionar a imagem para caber na caixa de 300 x 400 e recortar o que ficar fora da caixa.</span><span class="sxs-lookup"><span data-stu-id="2c6f4-p112">Generate a thumbnail that is 300x400 pixels. This works by resizing the image to fill the 300x400 box and cropping whatever spills outside the box.</span></span> |

<span data-ttu-id="2c6f4-234">**Observação:** talvez a miniatura retornada não corresponda exatamente às dimensões de pixel solicitadas, mas corresponderá com a taxa de proporção.</span><span class="sxs-lookup"><span data-stu-id="2c6f4-234">**Note:** The thumbnail returned may not exactly match the pixel dimensions that was requested, but will match the aspect ratio.</span></span>
<span data-ttu-id="2c6f4-235">Em alguns casos, uma miniatura maior do que a solicitada pode retornar, se a miniatura já existir, e pode ser facilmente dimensionada para coincidir com a resolução solicitada.</span><span class="sxs-lookup"><span data-stu-id="2c6f4-235">In some cases, a larger thumbnail may be returned than was requested, if the thumbnail already exists and can easily be scaled to match the requested resolution.</span></span>

## <a name="remarks"></a><span data-ttu-id="2c6f4-236">Comentários</span><span class="sxs-lookup"><span data-stu-id="2c6f4-236">Remarks</span></span>

<span data-ttu-id="2c6f4-237">**Observação** No OneDrive for Business e no SharePoint:</span><span class="sxs-lookup"><span data-stu-id="2c6f4-237">**Note** In OneDrive for Business and SharePoint:</span></span>

<span data-ttu-id="2c6f4-238">O uso dessas chamadas para expandir a coleção de miniaturas não funcionará:</span><span class="sxs-lookup"><span data-stu-id="2c6f4-238">Using these calls to expand the thumbnails collection will not work:</span></span>

* `GET /drive/root:/{item-path}?expand=children(expand=thumbnails)`
* `GET /drive/items/{item-id}/children?expand=thumbnails`

<span data-ttu-id="2c6f4-239">Não há suporte para miniaturas no SharePoint Server 2016.</span><span class="sxs-lookup"><span data-stu-id="2c6f4-239">Thumbnails are not supported on SharePoint Server 2016.</span></span>

### <a name="error-responses"></a><span data-ttu-id="2c6f4-240">Respostas de erro</span><span class="sxs-lookup"><span data-stu-id="2c6f4-240">Error responses</span></span>

<span data-ttu-id="2c6f4-241">Confira mais informações sobre como os erros são retornados em [Respostas de erro][error-response].</span><span class="sxs-lookup"><span data-stu-id="2c6f4-241">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

[error-response]: /graph/errors

<!--
{
  "type": "#page.annotation",
  "description": "Get metadata and content for thumbnails of multiple sizes for OneDrive items.",
  "keywords": "thumbnail,content,download,sizes",
  "section": "documentation",
  "tocPath": "Items/Thumbnails",
  "suppressions": [
    "Error: /api-reference/beta/api/driveitem-list-thumbnails.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/driveitem-list-thumbnails.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/driveitem-list-thumbnails.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/driveitem-list-thumbnails.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/driveitem-list-thumbnails.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/driveitem-list-thumbnails.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/driveitem-list-thumbnails.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/driveitem-list-thumbnails.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/driveitem-list-thumbnails.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/driveitem-list-thumbnails.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/driveitem-list-thumbnails.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
