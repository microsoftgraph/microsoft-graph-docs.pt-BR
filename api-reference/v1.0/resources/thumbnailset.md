# <a name="thumbnailset-resource-type"></a><span data-ttu-id="10e36-101">Tipo de recurso ThumbnailSet</span><span class="sxs-lookup"><span data-stu-id="10e36-101">ThumbnailSet resource type</span></span>

<span data-ttu-id="10e36-p101">O recurso **ThumbnailSet** é uma coleção com chave dos recursos [thumbnail](thumbnail.md). Ele é usado para representar um conjunto de miniaturas associado a um DriveItem.</span><span class="sxs-lookup"><span data-stu-id="10e36-p101">The **ThumbnailSet** resource is a keyed collection of [thumbnail](thumbnail.md) resources. It is used to represent a set of thumbnails associated with a DriveItem.</span></span>

## <a name="json-representation"></a><span data-ttu-id="10e36-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="10e36-104">JSON representation</span></span>

<span data-ttu-id="10e36-105">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="10e36-105">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": ["source", "small", "medium", "large"],
  "openType": true,
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.thumbnailSet"
} -->

```json
{
  "id": "string (identifier)",
  "large": {"@odata.type": "microsoft.graph.thumbnail"},
  "medium": {"@odata.type": "microsoft.graph.thumbnail"},
  "small": {"@odata.type": "microsoft.graph.thumbnail"},
  "source": {"@odata.type": "microsoft.graph.thumbnail"}
}
```

## <a name="properties"></a><span data-ttu-id="10e36-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="10e36-106">Properties</span></span>

| <span data-ttu-id="10e36-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="10e36-107">Property</span></span> | <span data-ttu-id="10e36-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="10e36-108">Type</span></span>                      | <span data-ttu-id="10e36-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="10e36-109">Description</span></span>                                                                       |
|:---------|:--------------------------|:----------------------------------------------------------------------------------|
| <span data-ttu-id="10e36-110">id</span><span class="sxs-lookup"><span data-stu-id="10e36-110">id</span></span>       | <span data-ttu-id="10e36-111">String</span><span class="sxs-lookup"><span data-stu-id="10e36-111">String</span></span>                    | <span data-ttu-id="10e36-p102">A id de dentro do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="10e36-p102">The id within the item. Read-only.</span></span>                                                |
| <span data-ttu-id="10e36-114">large</span><span class="sxs-lookup"><span data-stu-id="10e36-114">large</span></span>    | [<span data-ttu-id="10e36-115">Thumbnail</span><span class="sxs-lookup"><span data-stu-id="10e36-115">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="10e36-116">Uma miniatura em escala 1920 x 1920.</span><span class="sxs-lookup"><span data-stu-id="10e36-116">A 1920x1920 scaled thumbnail.</span></span>                                                     |
| <span data-ttu-id="10e36-117">medium</span><span class="sxs-lookup"><span data-stu-id="10e36-117">medium</span></span>   | [<span data-ttu-id="10e36-118">Thumbnail</span><span class="sxs-lookup"><span data-stu-id="10e36-118">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="10e36-119">Uma miniatura em escala 176 x 176.</span><span class="sxs-lookup"><span data-stu-id="10e36-119">A 176x176 scaled thumbnail.</span></span>                                                       |
| <span data-ttu-id="10e36-120">small</span><span class="sxs-lookup"><span data-stu-id="10e36-120">small</span></span>    | [<span data-ttu-id="10e36-121">Thumbnail</span><span class="sxs-lookup"><span data-stu-id="10e36-121">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="10e36-122">Uma miniatura cortada em 48 x 48.</span><span class="sxs-lookup"><span data-stu-id="10e36-122">A 48x48 cropped thumbnail.</span></span>                                                        |
| <span data-ttu-id="10e36-123">source</span><span class="sxs-lookup"><span data-stu-id="10e36-123">source</span></span>   | [<span data-ttu-id="10e36-124">Thumbnail</span><span class="sxs-lookup"><span data-stu-id="10e36-124">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="10e36-125">Uma imagem em miniatura personalizada ou a imagem original usada para gerar outras miniaturas.</span><span class="sxs-lookup"><span data-stu-id="10e36-125">A custom thumbnail image or the original image used to generate other thumbnails.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "thumbnailSet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
