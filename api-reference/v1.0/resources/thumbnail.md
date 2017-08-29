# <a name="thumbnail-resource-type"></a><span data-ttu-id="bc155-101">Tipo de recurso thumbnail</span><span class="sxs-lookup"><span data-stu-id="bc155-101">Thumbnail resource type</span></span>

<span data-ttu-id="bc155-102">O tipo de recurso **thumbnail** representa a miniatura de uma imagem, vídeo, documento ou qualquer item que tenha uma representação de bitmap.</span><span class="sxs-lookup"><span data-stu-id="bc155-102">The **thumbnail** resource type represents a thumbnail for an image, video, document, or any item that has a bitmap representation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="bc155-103">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bc155-103">JSON representation</span></span>

<span data-ttu-id="bc155-104">Veja a seguir uma representação JSON de um recurso **thumbnail**.</span><span class="sxs-lookup"><span data-stu-id="bc155-104">Here is a JSON representation of the **thumbnail** resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": ["content", "height", "width", "sourceItemId"],
  "@odata.type": "microsoft.graph.thumbnail"
}-->

```json
{
  "height": 1024,
  "sourceItemId": "string",
  "url": "string",
  "width": 1024,

  /* relationships */
  "content": "stream"
}
```

## <a name="properties"></a><span data-ttu-id="bc155-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bc155-105">Properties</span></span>

| <span data-ttu-id="bc155-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bc155-106">Property</span></span>     | <span data-ttu-id="bc155-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="bc155-107">Type</span></span>   | <span data-ttu-id="bc155-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="bc155-108">Description</span></span>                                                                                                                 |
| :----------- | :----- | :-------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="bc155-109">height</span><span class="sxs-lookup"><span data-stu-id="bc155-109">height</span></span>       | <span data-ttu-id="bc155-110">Int32</span><span class="sxs-lookup"><span data-stu-id="bc155-110">Int32</span></span>  | <span data-ttu-id="bc155-111">A altura da miniatura em pixels.</span><span class="sxs-lookup"><span data-stu-id="bc155-111">The height of the thumbnail, in pixels.</span></span>                                                                                     |
| <span data-ttu-id="bc155-112">sourceItemId</span><span class="sxs-lookup"><span data-stu-id="bc155-112">sourceItemId</span></span> | <span data-ttu-id="bc155-113">String</span><span class="sxs-lookup"><span data-stu-id="bc155-113">String</span></span> | <span data-ttu-id="bc155-p101">O identificador exclusivo do item que disponibilizou a miniatura. Só estará disponível quando for solicitada uma miniatura da pasta.</span><span class="sxs-lookup"><span data-stu-id="bc155-p101">The unique identifier of the item that provided the thumbnail. This is only available when a folder thumbnail is requested.</span></span> |
| <span data-ttu-id="bc155-116">url</span><span class="sxs-lookup"><span data-stu-id="bc155-116">url</span></span>          | <span data-ttu-id="bc155-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bc155-117">String</span></span> | <span data-ttu-id="bc155-118">A URL usada para buscar o conteúdo da miniatura.</span><span class="sxs-lookup"><span data-stu-id="bc155-118">The URL used to fetch the thumbnail content.</span></span>                                                                                |
| <span data-ttu-id="bc155-119">width</span><span class="sxs-lookup"><span data-stu-id="bc155-119">width</span></span>        | <span data-ttu-id="bc155-120">Int32</span><span class="sxs-lookup"><span data-stu-id="bc155-120">Int32</span></span>  | <span data-ttu-id="bc155-121">A largura da miniatura em pixels.</span><span class="sxs-lookup"><span data-stu-id="bc155-121">The width of the thumbnail, in pixels.</span></span>                                                                                      |

## <a name="relationships"></a><span data-ttu-id="bc155-122">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="bc155-122">Relationships</span></span>

| <span data-ttu-id="bc155-123">Nome</span><span class="sxs-lookup"><span data-stu-id="bc155-123">Name</span></span>    | <span data-ttu-id="bc155-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="bc155-124">Type</span></span>   | <span data-ttu-id="bc155-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="bc155-125">Description</span></span>                           |
| :------ | :----- | :------------------------------------ |
| <span data-ttu-id="bc155-126">content</span><span class="sxs-lookup"><span data-stu-id="bc155-126">content</span></span> | <span data-ttu-id="bc155-127">Fluxo</span><span class="sxs-lookup"><span data-stu-id="bc155-127">Stream</span></span> | <span data-ttu-id="bc155-128">O fluxo de conteúdo da miniatura.</span><span class="sxs-lookup"><span data-stu-id="bc155-128">The content stream for the thumbnail.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "thumbnail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
