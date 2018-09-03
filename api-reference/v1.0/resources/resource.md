# <a name="onenoteresource-resource-type"></a><span data-ttu-id="4fc1f-101">Tipo de recurso OneNoteResource</span><span class="sxs-lookup"><span data-stu-id="4fc1f-101">OneNoteResource resource type</span></span>

<span data-ttu-id="4fc1f-102">Uma imagem ou outro recurso de arquivo em uma página do OneNote.</span><span class="sxs-lookup"><span data-stu-id="4fc1f-102">An image or other file resource on a OneNote page.</span></span> 

<span data-ttu-id="4fc1f-103">É possível obter os dados binários de um recurso, mas não há suporte para obter uma representação JSON de um objeto de recurso ou uma coleção de recursos.</span><span class="sxs-lookup"><span data-stu-id="4fc1f-103">You can get the binary data of a resource, but getting a JSON representation of a resource object or a resource collection is not supported.</span></span>

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.onenoteEntityBaseModel",
  "optionalProperties": [],
  "isMediaEntity": true,
  "@odata.type": "microsoft.graph.onenoteResource"
}-->

```json
{
  "content": { "@odata.type": "Edm.Stream" },
  "contentUrl": "string (url)"
}
```

<span data-ttu-id="4fc1f-104">Obtenha os dados binários de um recurso específico enviando uma solicitação GET para o ponto de extremidade `content` do recurso:</span><span class="sxs-lookup"><span data-stu-id="4fc1f-104">Get the binary data of a specific resource by sending a GET request to the resource's `content` endpoint:</span></span>

```
GET ../onenote/resources/{id}/content
```

<span data-ttu-id="4fc1f-105">O URI de recurso do arquivo é retornado quando você recebe um conteúdo HTML da página usando a seguinte solicitação:</span><span class="sxs-lookup"><span data-stu-id="4fc1f-105">The file's resource URI is returned when you get a page's HTML content using the following request:</span></span>

```
GET ../onenote/pages/{id}/content
```

<span data-ttu-id="4fc1f-106">Na página HTML, uma marca `img` inclui os pontos de extremidade do recurso de imagem original no atributo `data-fullres-src` e a imagem otimizada no atributo `src`:</span><span class="sxs-lookup"><span data-stu-id="4fc1f-106">In the page HTML, an `img` tag includes endpoints for the original image resource in the `data-fullres-src` attribute and the optimized image in the `src` attribute:</span></span>
```
<img 
    src="image-resource-url"  
    data-src-type="media-type"
    data-fullres-src="image-resource-url"  
    data-fullres-src-type="media-type" ... />
```

<span data-ttu-id="4fc1f-107">Uma marca `object` (que representa arquivos como PDF, DOCX e PNG) inclui o ponto de extremidade para o recurso do arquivo no atributo `data`:</span><span class="sxs-lookup"><span data-stu-id="4fc1f-107">An `object` tag (which represents files such as PDF, DOCX, and PNG) includes the endpoint for the file resource in the `data` attribute:</span></span>

```
<object
    data="file-resource-url"
    data-attachment="file-name.file-type" 
    type="media-type" ... />
```

## <a name="properties"></a><span data-ttu-id="4fc1f-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4fc1f-108">Properties</span></span>

| <span data-ttu-id="4fc1f-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4fc1f-109">Property</span></span>             | <span data-ttu-id="4fc1f-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="4fc1f-110">Type</span></span>            | <span data-ttu-id="4fc1f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="4fc1f-111">Description</span></span>
|:---------------------|:----------------|:---------------------------------
| <span data-ttu-id="4fc1f-112">content</span><span class="sxs-lookup"><span data-stu-id="4fc1f-112">content</span></span>              | <span data-ttu-id="4fc1f-113">Fluxo</span><span class="sxs-lookup"><span data-stu-id="4fc1f-113">Stream</span></span>          | <span data-ttu-id="4fc1f-114">O fluxo de conteúdo</span><span class="sxs-lookup"><span data-stu-id="4fc1f-114">The content stream.</span></span>
| <span data-ttu-id="4fc1f-115">contentUrl</span><span class="sxs-lookup"><span data-stu-id="4fc1f-115">contentUrl</span></span>           | <span data-ttu-id="4fc1f-116">String (url)</span><span class="sxs-lookup"><span data-stu-id="4fc1f-116">string (url)</span></span>    | <span data-ttu-id="4fc1f-117">A URL para baixar o conteúdo</span><span class="sxs-lookup"><span data-stu-id="4fc1f-117">The URL for the page's HTML content.  Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="4fc1f-118">Relações</span><span class="sxs-lookup"><span data-stu-id="4fc1f-118">Relationships</span></span>
<span data-ttu-id="4fc1f-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4fc1f-119">None.</span></span>


## <a name="methods"></a><span data-ttu-id="4fc1f-120">Métodos</span><span class="sxs-lookup"><span data-stu-id="4fc1f-120">Methods</span></span>
| <span data-ttu-id="4fc1f-121">Método</span><span class="sxs-lookup"><span data-stu-id="4fc1f-121">Method</span></span>           | <span data-ttu-id="4fc1f-122">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="4fc1f-122">Return Type</span></span>    |<span data-ttu-id="4fc1f-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="4fc1f-123">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4fc1f-124">Get resource binary data</span><span class="sxs-lookup"><span data-stu-id="4fc1f-124">Get resource binary data</span></span>](../api/resource_get.md) | <span data-ttu-id="4fc1f-125">Fluxo</span><span class="sxs-lookup"><span data-stu-id="4fc1f-125">Stream</span></span> |<span data-ttu-id="4fc1f-126">Recupere os dados binários de um recurso de arquivo ou imagem.</span><span class="sxs-lookup"><span data-stu-id="4fc1f-126">Retrieve the binary data of a file or image resource.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "resource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->