# <a name="list-thumbnails-for-a-driveitem"></a><span data-ttu-id="59d0b-101">Listar miniaturas para um DriveItem</span><span class="sxs-lookup"><span data-stu-id="59d0b-101">List thumbnails for a DriveItem</span></span>

<span data-ttu-id="59d0b-102">Recupere uma coleção de recursos [ThumbnailSet](../resources/thumbnailset.md) para um recurso [DriveItem](../resources/driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="59d0b-102">Retrieve a collection of [ThumbnailSet](../resources/thumbnailset.md) resources for a [DriveItem](../resources/driveitem.md) resource.</span></span>

<span data-ttu-id="59d0b-p101">Um DriveItem pode ser representado por zero ou mais recursos [ThumbnailSet](../resources/thumbnailset.md). Cada **thumbnailSet** pode ter um ou mais objetos [**thumbnail**](../resources/thumbnail.md), que são imagens que representam o item. Por exemplo, um **thumbnailSet** podem incluir objetos **thumbnail**, como objetos comuns que incluem `small`, `medium` ou `large`.</span><span class="sxs-lookup"><span data-stu-id="59d0b-p101">A DriveItem can be represented by zero or more [ThumbnailSet](../resources/thumbnailset.md) resources. Each **thumbnailSet** can have one or more [**thumbnail**](../resources/thumbnail.md) objects, which are images that represent the item. For example, a **thumbnailSet** may include **thumbnail** objects, such as common ones including `small`, `medium`, or `large`.</span></span>

<span data-ttu-id="59d0b-p102">Há várias maneiras de trabalhar com miniaturas no OneDrive. Veja a seguir as mais comuns:</span><span class="sxs-lookup"><span data-stu-id="59d0b-p102">There are many ways to work with thumbnails on OneDrive. Here are the most common ones:</span></span>

* <span data-ttu-id="59d0b-108">Enumerar miniaturas disponíveis para um item</span><span class="sxs-lookup"><span data-stu-id="59d0b-108">Enumerate available thumbnails for an item</span></span>
* <span data-ttu-id="59d0b-109">Recuperar uma única miniatura para um item</span><span class="sxs-lookup"><span data-stu-id="59d0b-109">Retrieve a single thumbnail for an item</span></span>
* <span data-ttu-id="59d0b-110">Recuperar o conteúdo da miniatura</span><span class="sxs-lookup"><span data-stu-id="59d0b-110">Retrieve thumbnail content</span></span>
* <span data-ttu-id="59d0b-111">Recuperar miniaturas de vários itens em uma única solicitação</span><span class="sxs-lookup"><span data-stu-id="59d0b-111">Retrieve thumbnails for multiple items in a single request</span></span>
* <span data-ttu-id="59d0b-112">Recuperar tamanhos personalizados de miniaturas</span><span class="sxs-lookup"><span data-stu-id="59d0b-112">Retrieve custom thumbnail sizes</span></span>
* <span data-ttu-id="59d0b-113">Carregar uma miniatura personalizada para um item</span><span class="sxs-lookup"><span data-stu-id="59d0b-113">Upload a custom thumbnail for an item</span></span>
* <span data-ttu-id="59d0b-114">Determinar se uma miniatura personalizada carregada existe</span><span class="sxs-lookup"><span data-stu-id="59d0b-114">Determine if a custom uploaded thumbnail exists</span></span>


## <a name="prerequisites"></a><span data-ttu-id="59d0b-115">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="59d0b-115">Prerequisites</span></span>
<span data-ttu-id="59d0b-116">Um dos seguintes **escopos** é obrigatório para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="59d0b-116">One of the following **scopes** is required to execute this API:</span></span>

* <span data-ttu-id="59d0b-117">Files.Read</span><span class="sxs-lookup"><span data-stu-id="59d0b-117">Files.Read</span></span>
* <span data-ttu-id="59d0b-118">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="59d0b-118">Files.ReadWrite</span></span>
* <span data-ttu-id="59d0b-119">Files.Read.All</span><span class="sxs-lookup"><span data-stu-id="59d0b-119">Files.Read.All</span></span>
* <span data-ttu-id="59d0b-120">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59d0b-120">Files.ReadWrite.All</span></span>
* <span data-ttu-id="59d0b-121">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="59d0b-121">Sites.Read.All</span></span>
* <span data-ttu-id="59d0b-122">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59d0b-122">Sites.ReadWrite.All</span></span>


## <a name="http-request"></a><span data-ttu-id="59d0b-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="59d0b-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/root:/{item-path}:/thumbnails
GET /me/drive/items/{item-id}/thumbnails
GET /groups/{group-id}/drive/items/{item-id}/thumbnails
```

## <a name="optional-query-parameters"></a><span data-ttu-id="59d0b-124">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="59d0b-124">Optional query parameters</span></span>
<span data-ttu-id="59d0b-125">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="59d0b-125">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-body"></a><span data-ttu-id="59d0b-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="59d0b-126">Request body</span></span>
<span data-ttu-id="59d0b-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="59d0b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="59d0b-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="59d0b-128">Response</span></span>

<span data-ttu-id="59d0b-129">Se for bem-sucedido, esse método retornará um código de resposta `200 OK` e uma coleção de objetos [ThumbnailSet](../resources/thumbnailset.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="59d0b-129">If successful, this method returns a `200 OK` response code and collection of [ThumbnailSet](../resources/thumbnailset.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="59d0b-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="59d0b-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="59d0b-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="59d0b-131">Request</span></span>

<span data-ttu-id="59d0b-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="59d0b-132">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_thumbnails"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{item-id}/thumbnails
```


##### <a name="response"></a><span data-ttu-id="59d0b-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="59d0b-133">Response</span></span>
<span data-ttu-id="59d0b-134">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="59d0b-134">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.thumbnailSet",
  "isCollection": true
} -->
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

## <a name="retrieve-a-single-thumbnail"></a><span data-ttu-id="59d0b-135">Recuperar uma única miniatura</span><span class="sxs-lookup"><span data-stu-id="59d0b-135">Retrieve a single thumbnail</span></span>

<span data-ttu-id="59d0b-136">Recupere os metadados de uma única miniatura e tamanho tratando-os diretamente em uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="59d0b-136">Retrieve the metadata for a single thumbnail and size by addressing it directly in a request.</span></span>

## <a name="http-request"></a><span data-ttu-id="59d0b-137">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="59d0b-137">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-one-thumbnail" } -->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{item-id}/thumbnails/{thumb-id}/{size}
```

## <a name="path-parameters"></a><span data-ttu-id="59d0b-138">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="59d0b-138">Path parameters</span></span>

| <span data-ttu-id="59d0b-139">Nome</span><span class="sxs-lookup"><span data-stu-id="59d0b-139">Name</span></span>         | <span data-ttu-id="59d0b-140">Tipo</span><span class="sxs-lookup"><span data-stu-id="59d0b-140">Type</span></span>   | <span data-ttu-id="59d0b-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="59d0b-141">Description</span></span>                                                                         |
|:-------------|:-------|:------------------------------------------------------------------------------------|
| <span data-ttu-id="59d0b-142">**item-id**</span><span class="sxs-lookup"><span data-stu-id="59d0b-142">**item-id**</span></span>  | <span data-ttu-id="59d0b-143">string</span><span class="sxs-lookup"><span data-stu-id="59d0b-143">string</span></span> | <span data-ttu-id="59d0b-144">O identificador exclusivo do item referenciado.</span><span class="sxs-lookup"><span data-stu-id="59d0b-144">The unique identifier for the item referenced.</span></span>                                      |
| <span data-ttu-id="59d0b-145">**thumb-id**</span><span class="sxs-lookup"><span data-stu-id="59d0b-145">**thumb-id**</span></span> | <span data-ttu-id="59d0b-146">number</span><span class="sxs-lookup"><span data-stu-id="59d0b-146">number</span></span> | <span data-ttu-id="59d0b-147">O índice da miniatura, geralmente de 0 a 4.</span><span class="sxs-lookup"><span data-stu-id="59d0b-147">The index of the thumbnail, usually 0-4.</span></span>                                            |
| <span data-ttu-id="59d0b-148">**size**</span><span class="sxs-lookup"><span data-stu-id="59d0b-148">**size**</span></span>     | <span data-ttu-id="59d0b-149">string</span><span class="sxs-lookup"><span data-stu-id="59d0b-149">string</span></span> | <span data-ttu-id="59d0b-p103">O tamanho da miniatura solicitada. Ele deve ser um dos tamanhos padrão listados.</span><span class="sxs-lookup"><span data-stu-id="59d0b-p103">The size of the thumbnail requested. This must be one of the standard sizes listed.</span></span> |


<!-- { "blockType": "response", "@odata.type": "microsoft.graph.thumbnail" } -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "width": 100,
  "height": 100,
  "url": "http://onedrive.com/asd123a/asdjlkasjdkasdjlk.jpg"
}
```

## <a name="retrieve-thumbnail-content"></a><span data-ttu-id="59d0b-152">Recuperar o conteúdo da miniatura</span><span class="sxs-lookup"><span data-stu-id="59d0b-152">Retrieve thumbnail content</span></span>

<span data-ttu-id="59d0b-153">Você pode recuperar diretamente o conteúdo da miniatura solicitando a propriedade **content** dessa miniatura.</span><span class="sxs-lookup"><span data-stu-id="59d0b-153">You can directly retrieve the content of the thumbnail by requesting the **content** property of the thumbnail.</span></span>

## <a name="http-request"></a><span data-ttu-id="59d0b-154">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="59d0b-154">HTTP request</span></span>

<!-- { "blockType": "request", "name":"get-thumbnail-content" } -->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{item-id}/thumbnails/{thumb-id}/{size}/content
```

## <a name="response"></a><span data-ttu-id="59d0b-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="59d0b-155">Response</span></span>

<span data-ttu-id="59d0b-156">O serviço responde com um redirecionamento para a URL da miniatura.</span><span class="sxs-lookup"><span data-stu-id="59d0b-156">The service responds with a redirect to the thumbnail URL.</span></span>

<!-- { "blockType": "response" } -->
```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```

<span data-ttu-id="59d0b-p104">URLs de conteúdo de miniaturas são pré-autenticadas e não exigem o download de um cabeçalho de autorização. Essas URLs são de curta duração, permanecem válidas somente por algumas horas e não devem ser armazenadas em cache por aplicativos.</span><span class="sxs-lookup"><span data-stu-id="59d0b-p104">Thumbnail content URLs are pre-authenticated and do not require an authorization header to be downloaded. These URLs are short lived and only valid for a few hours and should not be cached by apps.</span></span>


## <a name="size-values"></a><span data-ttu-id="59d0b-159">Valores de tamanho</span><span class="sxs-lookup"><span data-stu-id="59d0b-159">Size values</span></span>

<span data-ttu-id="59d0b-p105">Essa tabela define os possíveis tamanhos de miniaturas. Embora você possa solicitar qualquer tamanho de miniatura arbitrário, os valores definidos provavelmente existem e retornam um valor rapidamente:</span><span class="sxs-lookup"><span data-stu-id="59d0b-p105">This table defines the possible thumbnail sizes. While you can request any arbitrary thumbnail size, the defined values are likely to exist and return a value quickly:</span></span>

| <span data-ttu-id="59d0b-162">Nome</span><span class="sxs-lookup"><span data-stu-id="59d0b-162">Name</span></span>           | <span data-ttu-id="59d0b-163">Resolução</span><span class="sxs-lookup"><span data-stu-id="59d0b-163">Resolution</span></span>  | <span data-ttu-id="59d0b-164">Taxa de proporção</span><span class="sxs-lookup"><span data-stu-id="59d0b-164">Aspect Ratio</span></span> | <span data-ttu-id="59d0b-165">Descrição</span><span class="sxs-lookup"><span data-stu-id="59d0b-165">Description</span></span>                                                          |
|:---------------|:------------|:-------------|:---------------------------------------------------------------------|
| `small`        | <span data-ttu-id="59d0b-166">96 mais longa</span><span class="sxs-lookup"><span data-stu-id="59d0b-166">96 longest</span></span>  | <span data-ttu-id="59d0b-167">Original</span><span class="sxs-lookup"><span data-stu-id="59d0b-167">Original</span></span>     | <span data-ttu-id="59d0b-168">Miniatura pequena e altamente compactada, recortada em uma taxa de proporção quadrada.</span><span class="sxs-lookup"><span data-stu-id="59d0b-168">Small, highly compressed thumbnail cropped to a square aspect ratio.</span></span> |
| `medium`       | <span data-ttu-id="59d0b-169">176 mais longa</span><span class="sxs-lookup"><span data-stu-id="59d0b-169">176 longest</span></span> | <span data-ttu-id="59d0b-170">Original</span><span class="sxs-lookup"><span data-stu-id="59d0b-170">Original</span></span>     | <span data-ttu-id="59d0b-171">Recortada no tamanho do item padrão para o modo de exibição de Web do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="59d0b-171">Cropped to the standard item size for the OneDrive web view.</span></span>         |
| `large`        | <span data-ttu-id="59d0b-172">800 mais longa</span><span class="sxs-lookup"><span data-stu-id="59d0b-172">800 longest</span></span> | <span data-ttu-id="59d0b-173">Original</span><span class="sxs-lookup"><span data-stu-id="59d0b-173">Original</span></span>     | <span data-ttu-id="59d0b-174">Miniatura com a borda mais longa redimensionada para 800 pixels.</span><span class="sxs-lookup"><span data-stu-id="59d0b-174">Thumbnail with the longest edge resized to 800 pixels.</span></span>               |

## <a name="remarks"></a><span data-ttu-id="59d0b-175">Comentários</span><span class="sxs-lookup"><span data-stu-id="59d0b-175">Remarks</span></span>

<span data-ttu-id="59d0b-176">**Observação** No OneDrive for Business e no SharePoint:</span><span class="sxs-lookup"><span data-stu-id="59d0b-176">**Note** In OneDrive for Business and SharePoint:</span></span>

* <span data-ttu-id="59d0b-177">O uso dessas chamadas para expandir a coleção de miniaturas não funcionará: `GET /drive/root:/{item-path}?expand=children(expand=thumbnails)`
  `GET /drive/items/{item-id}/children?expand=thumbnails`</span><span class="sxs-lookup"><span data-stu-id="59d0b-177">Using these calls to expand the thumbnails collection will not work: `GET /drive/root:/{item-path}?expand=children(expand=thumbnails)`
  `GET /drive/items/{item-id}/children?expand=thumbnails`</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get metadata and content for thumbnails of multiple sizes for OneDrive items.",
  "keywords": "thumbnail,content,download,sizes",
  "section": "documentation",
  "tocPath": "OneDrive/Item/List thumbnails"
} -->
