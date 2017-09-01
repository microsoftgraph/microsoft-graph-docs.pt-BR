# <a name="image-resource-type"></a><span data-ttu-id="2d4c0-101">Tipo de recurso Image</span><span class="sxs-lookup"><span data-stu-id="2d4c0-101">Image resource type</span></span>

<span data-ttu-id="2d4c0-p101">O recurso **Image** agrupa propriedades relacionadas a imagens em uma única estrutura. Se um [**DriveItem**](driveitem.md) tiver uma faceta **image** não nula, o item representa uma imagem bitmap.</span><span class="sxs-lookup"><span data-stu-id="2d4c0-p101">The **Image** resource groups image-related properties into a single structure. If a [**DriveItem**](driveitem.md) has a non-null **image** facet, the item represents a bitmap image.</span></span>

<span data-ttu-id="2d4c0-104">**Observação:** se o serviço não puder determinar a largura e a altura da imagem, o recurso **Image** poderá ficar vazio.</span><span class="sxs-lookup"><span data-stu-id="2d4c0-104">**Note:** If the service is unable to determine the width and height of the image, the **Image** resource may be empty.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2d4c0-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2d4c0-105">JSON representation</span></span>

<span data-ttu-id="2d4c0-106">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2d4c0-106">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@odata.type": "microsoft.graph.image"
}-->

```json
{
  "height": 1024,
  "width": 1024
}
```

## <a name="properties"></a><span data-ttu-id="2d4c0-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2d4c0-107">Properties</span></span>

| <span data-ttu-id="2d4c0-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2d4c0-108">Property</span></span>   | <span data-ttu-id="2d4c0-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="2d4c0-109">Type</span></span>  | <span data-ttu-id="2d4c0-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="2d4c0-110">Description</span></span>                                |
|:-----------|:------|:-------------------------------------------|
| <span data-ttu-id="2d4c0-111">**height**</span><span class="sxs-lookup"><span data-stu-id="2d4c0-111">**height**</span></span> | <span data-ttu-id="2d4c0-112">Int32</span><span class="sxs-lookup"><span data-stu-id="2d4c0-112">Int32</span></span> | <span data-ttu-id="2d4c0-p102">Opcional. A altura da imagem em pixels. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2d4c0-p102">Optional. Height of the image, in pixels. Read-only.</span></span> |
| <span data-ttu-id="2d4c0-116">**width**</span><span class="sxs-lookup"><span data-stu-id="2d4c0-116">**width**</span></span>  | <span data-ttu-id="2d4c0-117">Int32</span><span class="sxs-lookup"><span data-stu-id="2d4c0-117">Int32</span></span> | <span data-ttu-id="2d4c0-p103">Opcional. A largura da imagem em pixels. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2d4c0-p103">Optional. Width of the image, in pixels. Read-only.</span></span>  |

## <a name="remarks"></a><span data-ttu-id="2d4c0-121">Comentários</span><span class="sxs-lookup"><span data-stu-id="2d4c0-121">Remarks</span></span>

<span data-ttu-id="2d4c0-p104">No OneDrive for Business, esse recurso retorna em itens que devem ser imagens com base na extensão de arquivo. Este recurso não retorna propriedades no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="2d4c0-p104">In OneDrive for Business, this resource is returned on items that are expected to be images based on file extension. This resource returns no properties in OneDrive for Business.</span></span>

<span data-ttu-id="2d4c0-124">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="2d4c0-124">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "image resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
