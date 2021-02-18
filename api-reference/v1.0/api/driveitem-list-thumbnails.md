---
author: JeremyKelley
ms.date: 09/10/2017
title: Recuperar miniaturas de um arquivo ou pasta
localization_priority: Normal
ms.prod: sharepoint
description: Recupere uma coleção de recursos ThumbnailSet para um recurso DriveItem.
doc_type: apiPageType
ms.openlocfilehash: 9746221fe0aed4b606019250bd63f65d3972ebc3
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/18/2021
ms.locfileid: "50293040"
---
# <a name="list-thumbnails-for-a-driveitem"></a><span data-ttu-id="0cf92-103">Listar miniaturas para um DriveItem</span><span class="sxs-lookup"><span data-stu-id="0cf92-103">List thumbnails for a DriveItem</span></span>

<span data-ttu-id="0cf92-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0cf92-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0cf92-105">Recupere uma coleção de recursos [ThumbnailSet](../resources/thumbnailset.md) para um recurso [DriveItem](../resources/driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="0cf92-105">Retrieve a collection of [ThumbnailSet](../resources/thumbnailset.md) resources for a [DriveItem](../resources/driveitem.md) resource.</span></span>

<span data-ttu-id="0cf92-p101">Um DriveItem pode ser representado por zero ou mais recursos [ThumbnailSet](../resources/thumbnailset.md). Cada **thumbnailSet** pode ter um ou mais objetos [**thumbnail**](../resources/thumbnail.md), que são imagens que representam o item. Por exemplo, um **thumbnailSet** podem incluir objetos **thumbnail**, como objetos comuns que incluem `small`, `medium` ou `large`.</span><span class="sxs-lookup"><span data-stu-id="0cf92-p101">A DriveItem can be represented by zero or more [ThumbnailSet](../resources/thumbnailset.md) resources. Each **thumbnailSet** can have one or more [**thumbnail**](../resources/thumbnail.md) objects, which are images that represent the item. For example, a **thumbnailSet** may include **thumbnail** objects, such as common ones including `small`, `medium`, or `large`.</span></span>

<span data-ttu-id="0cf92-p102">Há várias maneiras de trabalhar com miniaturas no OneDrive. Veja a seguir as mais comuns:</span><span class="sxs-lookup"><span data-stu-id="0cf92-p102">There are many ways to work with thumbnails on OneDrive. Here are the most common ones:</span></span>

* <span data-ttu-id="0cf92-111">Enumerar miniaturas disponíveis para um item</span><span class="sxs-lookup"><span data-stu-id="0cf92-111">Enumerate available thumbnails for an item</span></span>
* <span data-ttu-id="0cf92-112">Recuperar uma única miniatura para um item</span><span class="sxs-lookup"><span data-stu-id="0cf92-112">Retrieve a single thumbnail for an item</span></span>
* <span data-ttu-id="0cf92-113">Recuperar o conteúdo da miniatura</span><span class="sxs-lookup"><span data-stu-id="0cf92-113">Retrieve thumbnail content</span></span>
* <span data-ttu-id="0cf92-114">Recuperar miniaturas de vários itens em uma única solicitação</span><span class="sxs-lookup"><span data-stu-id="0cf92-114">Retrieve thumbnails for multiple items in a single request</span></span>
* <span data-ttu-id="0cf92-115">Recuperar tamanhos personalizados de miniaturas</span><span class="sxs-lookup"><span data-stu-id="0cf92-115">Retrieve custom thumbnail sizes</span></span>
* <span data-ttu-id="0cf92-116">Carregar uma miniatura personalizada para um item</span><span class="sxs-lookup"><span data-stu-id="0cf92-116">Upload a custom thumbnail for an item</span></span>
* <span data-ttu-id="0cf92-117">Determinar se uma miniatura personalizada carregada existe</span><span class="sxs-lookup"><span data-stu-id="0cf92-117">Determine if a custom uploaded thumbnail exists</span></span>

## <a name="permissions"></a><span data-ttu-id="0cf92-118">Permissões</span><span class="sxs-lookup"><span data-stu-id="0cf92-118">Permissions</span></span>

<span data-ttu-id="0cf92-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0cf92-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0cf92-121">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0cf92-121">Permission type</span></span>      | <span data-ttu-id="0cf92-122">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0cf92-122">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0cf92-123">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0cf92-123">Delegated (work or school account)</span></span> | <span data-ttu-id="0cf92-124">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0cf92-124">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="0cf92-125">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0cf92-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0cf92-126">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0cf92-126">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="0cf92-127">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0cf92-127">Application</span></span> | <span data-ttu-id="0cf92-128">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0cf92-128">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0cf92-129">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0cf92-129">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/thumbnails
GET /groups/{group-id}/drive/items/{item-id}/thumbnails
GET /me/drive/items/{item-id}/thumbnails
GET /sites/{site-id}/drive/items/{item-id}/thumbnails
GET /users/{user-id}/drive/items/{item-id}/thumbnails
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0cf92-130">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0cf92-130">Optional query parameters</span></span>

<span data-ttu-id="0cf92-131">Este método oferece suporte ao [Parâmetro de consulta OData](/graph/query-parameters) `$select` para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0cf92-131">This method supports the `$select` [OData puery parameter](/graph/query-parameters) to customize the response.</span></span>

<span data-ttu-id="0cf92-132">Além disso, esse método dá suporte à recuperação da miniatura com o valor EXIF de orientação original e sem a rotação aplicada, adicionando o parâmetro `originalOrientation=true` de consulta.</span><span class="sxs-lookup"><span data-stu-id="0cf92-132">Additionally, this method supports retrieving the thumbnail with the original orientation EXIF value and without the applied rotation by appending the `originalOrientation=true` query parameter.</span></span>
<span data-ttu-id="0cf92-133">No momento, só há suporte para isso no OneDrive pessoal.</span><span class="sxs-lookup"><span data-stu-id="0cf92-133">This is currently only supported on OneDrive Personal.</span></span>

## <a name="response"></a><span data-ttu-id="0cf92-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="0cf92-134">Response</span></span>

<span data-ttu-id="0cf92-135">Se for bem-sucedido, esse método retornará um código de resposta `200 OK` e uma coleção de objetos [ThumbnailSet](../resources/thumbnailset.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0cf92-135">If successful, this method returns a `200 OK` response code and collection of [ThumbnailSet](../resources/thumbnailset.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0cf92-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0cf92-136">Example</span></span>

<span data-ttu-id="0cf92-137">Veja um exemplo da solicitação que recupera as miniaturas disponíveis de um item no OneDrive atual do usuário.</span><span class="sxs-lookup"><span data-stu-id="0cf92-137">Here is an example of the request which retrieves available thumbnails for an item in the current user's OneDrive.</span></span>


# <a name="http"></a>[<span data-ttu-id="0cf92-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="0cf92-138">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "enum-item-thumbnails", "scopes": "files.read", "tags": "service.graph" } -->

```msgraph-interactive
GET /me/drive/items/{item-id}/thumbnails
```
# <a name="c"></a>[<span data-ttu-id="0cf92-139">C#</span><span class="sxs-lookup"><span data-stu-id="0cf92-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/enum-item-thumbnails-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0cf92-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0cf92-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/enum-item-thumbnails-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0cf92-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0cf92-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/enum-item-thumbnails-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0cf92-142">Java</span><span class="sxs-lookup"><span data-stu-id="0cf92-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/enum-item-thumbnails-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="0cf92-143">Isto retorna uma matriz de **thumbnailSets** disponíveis para o item.</span><span class="sxs-lookup"><span data-stu-id="0cf92-143">This returns an array of available **thumbnailSets** for the item.</span></span> <span data-ttu-id="0cf92-144">Qualquer item em uma unidade pode ter zero ou mais miniaturas.</span><span class="sxs-lookup"><span data-stu-id="0cf92-144">Any item in a drive can have zero or more thumbnails.</span></span>

<span data-ttu-id="0cf92-p106">**Observação:** Você pode usar o parâmetro da cadeia de caracteres de consulta _select_ para controlar quais tamanhos de miniatura são retornados no **ThumbnailSet**. Por exemplo, `/thumbnails?select=medium` recupera somente miniaturas de tamanho médio.</span><span class="sxs-lookup"><span data-stu-id="0cf92-p106">**Note:** You can use the _select_ query string parameter to control which thumbnail sizes are returned in the **ThumbnailSet**. For example, `/thumbnails?select=medium` retrieves only the medium sized thumbnails.</span></span>


### <a name="response"></a><span data-ttu-id="0cf92-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="0cf92-147">Response</span></span>

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

## <a name="get-a-single-thumbnail"></a><span data-ttu-id="0cf92-148">Obter uma única miniatura</span><span class="sxs-lookup"><span data-stu-id="0cf92-148">Get a single thumbnail</span></span>

<span data-ttu-id="0cf92-149">Recupere os metadados de uma única miniatura e tamanho tratando-os diretamente em uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="0cf92-149">Retrieve the metadata for a single thumbnail and size by addressing it directly in a request.</span></span>

### <a name="http-request"></a><span data-ttu-id="0cf92-150">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0cf92-150">HTTP request</span></span>


# <a name="http"></a>[<span data-ttu-id="0cf92-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="0cf92-151">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-one-thumbnail", "scopes": "files.read", "tags": "service.graph" } -->

```msgraph-interactive
GET /me/drive/items/{item-id}/thumbnails/{thumb-id}/{size}
```
# <a name="c"></a>[<span data-ttu-id="0cf92-152">C#</span><span class="sxs-lookup"><span data-stu-id="0cf92-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-one-thumbnail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0cf92-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0cf92-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-one-thumbnail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0cf92-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0cf92-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-one-thumbnail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0cf92-155">Java</span><span class="sxs-lookup"><span data-stu-id="0cf92-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-one-thumbnail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="path-parameters"></a><span data-ttu-id="0cf92-156">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="0cf92-156">Path parameters</span></span>

| <span data-ttu-id="0cf92-157">Nome</span><span class="sxs-lookup"><span data-stu-id="0cf92-157">Name</span></span>         | <span data-ttu-id="0cf92-158">Tipo</span><span class="sxs-lookup"><span data-stu-id="0cf92-158">Type</span></span>   | <span data-ttu-id="0cf92-159">Descrição</span><span class="sxs-lookup"><span data-stu-id="0cf92-159">Description</span></span>                                                                              |
|:-------------|:-------|:-----------------------------------------------------------------------------------------|
| <span data-ttu-id="0cf92-160">**item-id**</span><span class="sxs-lookup"><span data-stu-id="0cf92-160">**item-id**</span></span>  | <span data-ttu-id="0cf92-161">string</span><span class="sxs-lookup"><span data-stu-id="0cf92-161">string</span></span> | <span data-ttu-id="0cf92-162">O identificador exclusivo do item referenciado.</span><span class="sxs-lookup"><span data-stu-id="0cf92-162">The unique identifier for the item referenced.</span></span>                                           |
| <span data-ttu-id="0cf92-163">**thumb-id**</span><span class="sxs-lookup"><span data-stu-id="0cf92-163">**thumb-id**</span></span> | <span data-ttu-id="0cf92-164">number</span><span class="sxs-lookup"><span data-stu-id="0cf92-164">number</span></span> | <span data-ttu-id="0cf92-p107">O índice da miniatura, geralmente de 0 a 4. Se houver uma miniatura personalizada, seu índice será 0.</span><span class="sxs-lookup"><span data-stu-id="0cf92-p107">The index of the thumbnail, usually 0-4. If there is a custom thumbnail, its index is 0.</span></span> |
| <span data-ttu-id="0cf92-167">**size**</span><span class="sxs-lookup"><span data-stu-id="0cf92-167">**size**</span></span>     | <span data-ttu-id="0cf92-168">string</span><span class="sxs-lookup"><span data-stu-id="0cf92-168">string</span></span> | <span data-ttu-id="0cf92-169">O tamanho da miniatura solicitada.</span><span class="sxs-lookup"><span data-stu-id="0cf92-169">The size of the thumbnail requested.</span></span> <span data-ttu-id="0cf92-170">Pode ter um dos tamanhos padrão listados abaixo, ou um tamanho personalizado.</span><span class="sxs-lookup"><span data-stu-id="0cf92-170">This can be one of the standard sizes listed below or a custom size.</span></span> |

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

## <a name="retrieve-thumbnail-binary-content"></a><span data-ttu-id="0cf92-171">Recuperar o conteúdo binário da miniatura</span><span class="sxs-lookup"><span data-stu-id="0cf92-171">Retrieve thumbnail binary content</span></span>

<span data-ttu-id="0cf92-172">Você pode recuperar diretamente o conteúdo da miniatura solicitando a propriedade **content** dessa miniatura.</span><span class="sxs-lookup"><span data-stu-id="0cf92-172">You can directly retrieve the content of the thumbnail by requesting the **content** property of the thumbnail.</span></span>

### <a name="http-request"></a><span data-ttu-id="0cf92-173">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0cf92-173">HTTP request</span></span>


# <a name="http"></a>[<span data-ttu-id="0cf92-174">HTTP</span><span class="sxs-lookup"><span data-stu-id="0cf92-174">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name":"get-thumbnail-content", "scopes": "files.read", "tags": "service.graph" } -->

```msgraph-interactive
GET /me/drive/items/{item-id}/thumbnails/{thumb-id}/{size}/content
```
# <a name="c"></a>[<span data-ttu-id="0cf92-175">C#</span><span class="sxs-lookup"><span data-stu-id="0cf92-175">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-thumbnail-content-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0cf92-176">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0cf92-176">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-thumbnail-content-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0cf92-177">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0cf92-177">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-thumbnail-content-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0cf92-178">Java</span><span class="sxs-lookup"><span data-stu-id="0cf92-178">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-thumbnail-content-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0cf92-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="0cf92-179">Response</span></span>

<span data-ttu-id="0cf92-180">O serviço responde com um redirecionamento para a URL da miniatura.</span><span class="sxs-lookup"><span data-stu-id="0cf92-180">The service responds with a redirect to the thumbnail URL.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```

<span data-ttu-id="0cf92-181">URLs de miniaturas são seguras em cache.</span><span class="sxs-lookup"><span data-stu-id="0cf92-181">Thumbnail URLs are cache-safe.</span></span> <span data-ttu-id="0cf92-182">A URL mudará se o item for alterado de uma maneira que exigir que uma nova miniatura seja gerada.</span><span class="sxs-lookup"><span data-stu-id="0cf92-182">The URL will change, if the item changes in a way that requires a new thumbnail to be generated.</span></span>


## <a name="getting-thumbnails-while-listing-driveitems"></a><span data-ttu-id="0cf92-183">Obter miniaturas ao listar DriveItems</span><span class="sxs-lookup"><span data-stu-id="0cf92-183">Getting thumbnails while listing DriveItems</span></span>

<span data-ttu-id="0cf92-184">Se você estiver recuperando uma lista de recursos DriveItem para exibição, use o parâmetro de cadeia de consulta _$expand_ para incluir as miniaturas para esses recursos.</span><span class="sxs-lookup"><span data-stu-id="0cf92-184">If you are retrieving a list of DriveItem resources to display, you can use the _$expand_ query string parameter to also include the thumbnails for those resources.</span></span>
<span data-ttu-id="0cf92-185">Isso permite que seu aplicativo recupere miniaturas e itens em uma única solicitação, em vez de emitir muitas solicitações.</span><span class="sxs-lookup"><span data-stu-id="0cf92-185">This enables your app to retrieve thumbnails and items in a single request, instead of issuing many requests.</span></span>

### <a name="http-request"></a><span data-ttu-id="0cf92-186">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0cf92-186">HTTP request</span></span>


# <a name="http"></a>[<span data-ttu-id="0cf92-187">HTTP</span><span class="sxs-lookup"><span data-stu-id="0cf92-187">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name":"get-thumbnail-while-listing", "scopes": "files.read", "tags": "service.graph" } -->

```msgraph-interactive
GET /me/drive/items/{item-id}/children?$expand=thumbnails
```
# <a name="c"></a>[<span data-ttu-id="0cf92-188">C#</span><span class="sxs-lookup"><span data-stu-id="0cf92-188">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-thumbnail-while-listing-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0cf92-189">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0cf92-189">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-thumbnail-while-listing-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0cf92-190">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0cf92-190">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-thumbnail-while-listing-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0cf92-191">Java</span><span class="sxs-lookup"><span data-stu-id="0cf92-191">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-thumbnail-while-listing-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0cf92-192">Resposta</span><span class="sxs-lookup"><span data-stu-id="0cf92-192">Response</span></span>

<span data-ttu-id="0cf92-193">As respostas do serviço com a lista de DriveItems e suas miniaturas.</span><span class="sxs-lookup"><span data-stu-id="0cf92-193">The service responses with the list of DriveItems and their thumbnails.</span></span>

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

## <a name="size-options"></a><span data-ttu-id="0cf92-194">Opções de tamanho</span><span class="sxs-lookup"><span data-stu-id="0cf92-194">Size options</span></span>

<span data-ttu-id="0cf92-p111">Essa tabela define os possíveis tamanhos de miniaturas. Embora você possa solicitar qualquer tamanho de miniatura arbitrário, os valores definidos provavelmente existem e retornam um valor rapidamente:</span><span class="sxs-lookup"><span data-stu-id="0cf92-p111">This table defines the possible thumbnail sizes. While you can request any arbitrary thumbnail size, the defined values are likely to exist and return a value quickly:</span></span>

| <span data-ttu-id="0cf92-197">Nome</span><span class="sxs-lookup"><span data-stu-id="0cf92-197">Name</span></span>           | <span data-ttu-id="0cf92-198">Resolução</span><span class="sxs-lookup"><span data-stu-id="0cf92-198">Resolution</span></span>  | <span data-ttu-id="0cf92-199">Taxa de proporção</span><span class="sxs-lookup"><span data-stu-id="0cf92-199">Aspect Ratio</span></span> | <span data-ttu-id="0cf92-200">Descrição</span><span class="sxs-lookup"><span data-stu-id="0cf92-200">Description</span></span>                                                          |
|:---------------|:------------|:-------------|:---------------------------------------------------------------------|
| `small`        | <span data-ttu-id="0cf92-201">96 mais longa</span><span class="sxs-lookup"><span data-stu-id="0cf92-201">96 longest</span></span>  | <span data-ttu-id="0cf92-202">Original</span><span class="sxs-lookup"><span data-stu-id="0cf92-202">Original</span></span>     | <span data-ttu-id="0cf92-203">Miniatura pequena e altamente compactada, recortada em uma taxa de proporção quadrada.</span><span class="sxs-lookup"><span data-stu-id="0cf92-203">Small, highly compressed thumbnail cropped to a square aspect ratio.</span></span> |
| `medium`       | <span data-ttu-id="0cf92-204">176 mais longa</span><span class="sxs-lookup"><span data-stu-id="0cf92-204">176 longest</span></span> | <span data-ttu-id="0cf92-205">Original</span><span class="sxs-lookup"><span data-stu-id="0cf92-205">Original</span></span>     | <span data-ttu-id="0cf92-206">Recortada no tamanho do item padrão para o modo de exibição de Web do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="0cf92-206">Cropped to the standard item size for the OneDrive web view.</span></span>         |
| `large`        | <span data-ttu-id="0cf92-207">800 mais longa</span><span class="sxs-lookup"><span data-stu-id="0cf92-207">800 longest</span></span> | <span data-ttu-id="0cf92-208">Original</span><span class="sxs-lookup"><span data-stu-id="0cf92-208">Original</span></span>     | <span data-ttu-id="0cf92-209">Miniatura com a borda mais longa redimensionada para 800 pixels.</span><span class="sxs-lookup"><span data-stu-id="0cf92-209">Thumbnail with the longest edge resized to 800 pixels.</span></span>               |
| `smallSquare`  | <span data-ttu-id="0cf92-210">96x96</span><span class="sxs-lookup"><span data-stu-id="0cf92-210">96x96</span></span>       | <span data-ttu-id="0cf92-211">Corte quadrado</span><span class="sxs-lookup"><span data-stu-id="0cf92-211">Square Crop</span></span>  | <span data-ttu-id="0cf92-212">Miniatura quadrada pequena</span><span class="sxs-lookup"><span data-stu-id="0cf92-212">Small square thumbnail</span></span>                                               |
| `mediumSquare` | <span data-ttu-id="0cf92-213">176x176</span><span class="sxs-lookup"><span data-stu-id="0cf92-213">176x176</span></span>     | <span data-ttu-id="0cf92-214">Corte quadrado</span><span class="sxs-lookup"><span data-stu-id="0cf92-214">Square Crop</span></span>  | <span data-ttu-id="0cf92-215">Miniatura quadrada pequena</span><span class="sxs-lookup"><span data-stu-id="0cf92-215">Small square thumbnail</span></span>                                               |
| `largeSquare`  | <span data-ttu-id="0cf92-216">800x800</span><span class="sxs-lookup"><span data-stu-id="0cf92-216">800x800</span></span>     | <span data-ttu-id="0cf92-217">Corte quadrado</span><span class="sxs-lookup"><span data-stu-id="0cf92-217">Square Crop</span></span>  | <span data-ttu-id="0cf92-218">Miniatura quadrada grande</span><span class="sxs-lookup"><span data-stu-id="0cf92-218">Large square thumbnail</span></span>                                               |

## <a name="requesting-custom-thumbnail-sizes"></a><span data-ttu-id="0cf92-219">Solicitar tamanhos personalizados de miniaturas</span><span class="sxs-lookup"><span data-stu-id="0cf92-219">Requesting custom thumbnail sizes</span></span>

<span data-ttu-id="0cf92-220">Além dos tamanhos definidos, seu aplicativo pode solicitar um tamanho personalizado de miniatura, especificando as dimensões da miniatura prefixadas com `c`.</span><span class="sxs-lookup"><span data-stu-id="0cf92-220">In addition to the defined sizes, your app can request a custom thumbnail size by specifying the dimensions of the thumbnail prefixed with `c`.</span></span>
<span data-ttu-id="0cf92-221">Por exemplo, se o seu aplicativo precisar de miniaturas de 300 x 400, é possível solicitar esse tamanho desta forma:</span><span class="sxs-lookup"><span data-stu-id="0cf92-221">For example if your app needs thumbnails that are 300x400, it can request that size like this:</span></span>


# <a name="http"></a>[<span data-ttu-id="0cf92-222">HTTP</span><span class="sxs-lookup"><span data-stu-id="0cf92-222">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-thumbnail-custom-size", "scopes": "files.read", "tags": "service.graph" } -->

```msgraph-interactive
GET /me/drive/items/{item-id}/thumbnails?select=c300x400_Crop
```
# <a name="c"></a>[<span data-ttu-id="0cf92-223">C#</span><span class="sxs-lookup"><span data-stu-id="0cf92-223">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-thumbnail-custom-size-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0cf92-224">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0cf92-224">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-thumbnail-custom-size-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0cf92-225">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0cf92-225">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-thumbnail-custom-size-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0cf92-226">Java</span><span class="sxs-lookup"><span data-stu-id="0cf92-226">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-thumbnail-custom-size-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="0cf92-227">Que responde com o tamanho de miniatura personalizado selecionado:</span><span class="sxs-lookup"><span data-stu-id="0cf92-227">Which responds with just the custom thumbnail size selected:</span></span>

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

<span data-ttu-id="0cf92-228">Você pode especificar as seguintes opções após o tamanho de miniatura solicitado:</span><span class="sxs-lookup"><span data-stu-id="0cf92-228">You can specify the following options after the size of the thumbnail requested:</span></span>

### <a name="examples-of-custom-identifiers"></a><span data-ttu-id="0cf92-229">Exemplos de identificadores personalizados</span><span class="sxs-lookup"><span data-stu-id="0cf92-229">Examples of custom identifiers</span></span>

| <span data-ttu-id="0cf92-230">Identificador de miniatura</span><span class="sxs-lookup"><span data-stu-id="0cf92-230">Thumbnail identifier</span></span> | <span data-ttu-id="0cf92-231">Resolução</span><span class="sxs-lookup"><span data-stu-id="0cf92-231">Resolution</span></span>             | <span data-ttu-id="0cf92-232">Taxa de proporção</span><span class="sxs-lookup"><span data-stu-id="0cf92-232">Aspect ratio</span></span> | <span data-ttu-id="0cf92-233">Descrição</span><span class="sxs-lookup"><span data-stu-id="0cf92-233">Description</span></span>                                                                                                                                         |
|:---------------------|:-----------------------|:-------------|:----------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="0cf92-234">c300x400</span><span class="sxs-lookup"><span data-stu-id="0cf92-234">c300x400</span></span>             | <span data-ttu-id="0cf92-235">Limitado por uma caixa de 300 x 400</span><span class="sxs-lookup"><span data-stu-id="0cf92-235">Bounded by 300x400 box</span></span> | <span data-ttu-id="0cf92-236">Original</span><span class="sxs-lookup"><span data-stu-id="0cf92-236">Original</span></span>     | <span data-ttu-id="0cf92-237">Gere uma miniatura que se ajuste em uma caixa de 300 x 400 pixels, mantendo a taxa de proporção</span><span class="sxs-lookup"><span data-stu-id="0cf92-237">Generate a thumbnail that fits inside a 300x400 pixel box, maintaining aspect ratio</span></span>                                                                 |
| <span data-ttu-id="0cf92-238">c300x400_Crop</span><span class="sxs-lookup"><span data-stu-id="0cf92-238">c300x400_Crop</span></span>        | <span data-ttu-id="0cf92-239">300x400</span><span class="sxs-lookup"><span data-stu-id="0cf92-239">300x400</span></span>                | <span data-ttu-id="0cf92-240">Recortada</span><span class="sxs-lookup"><span data-stu-id="0cf92-240">Cropped</span></span>      | <span data-ttu-id="0cf92-p113">Gere uma miniatura de 300 x 400 pixels. Para isso, é preciso redimensionar a imagem para caber na caixa de 300 x 400 e recortar o que ficar fora da caixa.</span><span class="sxs-lookup"><span data-stu-id="0cf92-p113">Generate a thumbnail that is 300x400 pixels. This works by resizing the image to fill the 300x400 box and cropping whatever spills outside the box.</span></span> |

<span data-ttu-id="0cf92-243">**Observação:** talvez a miniatura retornada não corresponda exatamente às dimensões de pixel solicitadas, mas corresponderá com a taxa de proporção.</span><span class="sxs-lookup"><span data-stu-id="0cf92-243">**Note:** The thumbnail returned may not exactly match the pixel dimensions that was requested, but will match the aspect ratio.</span></span>
<span data-ttu-id="0cf92-244">Em alguns casos, uma miniatura maior do que a solicitada pode retornar, se a miniatura já existir, e pode ser facilmente dimensionada para coincidir com a resolução solicitada.</span><span class="sxs-lookup"><span data-stu-id="0cf92-244">In some cases, a larger thumbnail may be returned than was requested, if the thumbnail already exists and can easily be scaled to match the requested resolution.</span></span>

## <a name="remarks"></a><span data-ttu-id="0cf92-245">Comentários</span><span class="sxs-lookup"><span data-stu-id="0cf92-245">Remarks</span></span>

<span data-ttu-id="0cf92-246">**Observação** No OneDrive for Business e no SharePoint:</span><span class="sxs-lookup"><span data-stu-id="0cf92-246">**Note** In OneDrive for Business and SharePoint:</span></span>

<span data-ttu-id="0cf92-247">O uso dessas chamadas para expandir a coleção de miniaturas não funcionará:</span><span class="sxs-lookup"><span data-stu-id="0cf92-247">Using these calls to expand the thumbnails collection will not work:</span></span>

* `GET /drive/root:/{item-path}?expand=children(expand=thumbnails)`
* `GET /drive/items/{item-id}/children?expand=thumbnails`

<span data-ttu-id="0cf92-248">Não há suporte para miniaturas no SharePoint Server 2016.</span><span class="sxs-lookup"><span data-stu-id="0cf92-248">Thumbnails are not supported on SharePoint Server 2016.</span></span>

### <a name="error-responses"></a><span data-ttu-id="0cf92-249">Respostas de erros</span><span class="sxs-lookup"><span data-stu-id="0cf92-249">Error responses</span></span>

<span data-ttu-id="0cf92-250">Confira mais informações sobre como os erros são retornados em [Respostas de Erros][error-response].</span><span class="sxs-lookup"><span data-stu-id="0cf92-250">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Get metadata and content for thumbnails of multiple sizes for OneDrive items.",
  "keywords": "thumbnail,content,download,sizes",
  "section": "documentation",
  "suppressions": [
  ],
  "tocPath": "Items/Thumbnails"
} -->

