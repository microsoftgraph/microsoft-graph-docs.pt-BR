# <a name="geocoordinates-resource-type"></a><span data-ttu-id="f2366-101">Tipo de recurso GeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="f2366-101">GeoCoordinates resource type</span></span>

<span data-ttu-id="f2366-p101">O recurso **GeoCoordinates** fornece as coordenadas geográficas e a elevação de um local com base nos metadados contidos no arquivo. Se um [**DriveItem**](driveitem.md) tiver uma faceta **location** não nula, o item representa um arquivo com um local conhecido associado a ele.</span><span class="sxs-lookup"><span data-stu-id="f2366-p101">The **GeoCoordinates** resource provides geographic coordinates and elevation of a location based on metadata contained within the file. If a [**DriveItem**](driveitem.md) has a non-null **location** facet, the item represents a file with a known location assocaited with it.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f2366-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f2366-104">JSON representation</span></span>

<span data-ttu-id="f2366-105">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="f2366-105">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.geoCoordinates"
}-->

```json
{
  "altitude": 1024.13,
  "latitude": 26.13246,
  "longitude": 24.34616
}
```

## <a name="properties"></a><span data-ttu-id="f2366-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f2366-106">Properties</span></span>

| <span data-ttu-id="f2366-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f2366-107">Property</span></span>  | <span data-ttu-id="f2366-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="f2366-108">Type</span></span>   | <span data-ttu-id="f2366-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="f2366-109">Description</span></span>                                                    |
|:----------|:-------|:---------------------------------------------------------------|
| <span data-ttu-id="f2366-110">altitude</span><span class="sxs-lookup"><span data-stu-id="f2366-110">altitude</span></span>  | <span data-ttu-id="f2366-111">Double</span><span class="sxs-lookup"><span data-stu-id="f2366-111">Double</span></span> | <span data-ttu-id="f2366-p102">Opcional. A altitude (altura), em pés, acima do nível do mar para o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f2366-p102">Optional. The altitude (height), in feet,  above sea level for the item. Read-only.</span></span> |
| <span data-ttu-id="f2366-115">latitude</span><span class="sxs-lookup"><span data-stu-id="f2366-115">latitude</span></span>  | <span data-ttu-id="f2366-116">Double</span><span class="sxs-lookup"><span data-stu-id="f2366-116">Double</span></span> | <span data-ttu-id="f2366-p103">Opcional. A latitude, em valor decimal, para o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f2366-p103">Optional. The latitude, in decimal, for the item. Read-only.</span></span>   |
| <span data-ttu-id="f2366-120">longitude</span><span class="sxs-lookup"><span data-stu-id="f2366-120">longitude</span></span> | <span data-ttu-id="f2366-121">Double</span><span class="sxs-lookup"><span data-stu-id="f2366-121">Double</span></span> | <span data-ttu-id="f2366-p104">Opcional. A longitude, em valor decimal, para o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f2366-p104">Optional. The longitude, in decimal, for the item. Read-only.</span></span>  |

## <a name="remarks"></a><span data-ttu-id="f2366-125">Comentários</span><span class="sxs-lookup"><span data-stu-id="f2366-125">Remarks</span></span>

<span data-ttu-id="f2366-126">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="f2366-126">For more information about the facets on a [driveItem](driveitem.md), see driveItem.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "geoCoordinates resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
