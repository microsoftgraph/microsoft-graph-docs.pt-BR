# <a name="photo-resource-type"></a><span data-ttu-id="9c730-101">Tipo de recurso Photo</span><span class="sxs-lookup"><span data-stu-id="9c730-101">Photo resource type</span></span>

<span data-ttu-id="9c730-102">O recurso **photo** fornece propriedades de foto e câmera, por exemplo, metadados EXIF, em um [driveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="9c730-102">The **photo** resource provides photo and camera properties, for example, EXIF metadata, on a [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="9c730-103">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9c730-103">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.photo"
}-->
```json
{
  "cameraMake": "string",
  "cameraModel": "string",
  "exposureDenominator": 1024,
  "exposureNumerator": 1024,
  "fNumber": 1024,
  "focalLength": 1024,
  "iso": 1024,
  "takenDateTime": "String (timestamp)"
}
```

## <a name="properties"></a><span data-ttu-id="9c730-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9c730-104">Properties</span></span>
| <span data-ttu-id="9c730-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9c730-105">Property</span></span>                | <span data-ttu-id="9c730-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="9c730-106">Type</span></span>                      | <span data-ttu-id="9c730-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="9c730-107">Description</span></span>                                                     |
|:------------------------|:--------------------------|:----------------------------------------------------------------|
| <span data-ttu-id="9c730-108">**takenDateTime**</span><span class="sxs-lookup"><span data-stu-id="9c730-108">**takenDateTime**</span></span>       | <span data-ttu-id="9c730-109">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9c730-109">DateTimeOffset</span></span>            | <span data-ttu-id="9c730-p101">Representa a data e a hora em que a foto foi tirada. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9c730-p101">Represents the date and time the photo was taken. Read-only.</span></span>               |
| <span data-ttu-id="9c730-112">**cameraMake**</span><span class="sxs-lookup"><span data-stu-id="9c730-112">**cameraMake**</span></span>          | <span data-ttu-id="9c730-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9c730-113">String</span></span>                    | <span data-ttu-id="9c730-p102">Fabricante da câmera. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9c730-p102">Camera manufacturer. Read-only.</span></span>                                            |
| <span data-ttu-id="9c730-116">**cameraModel**</span><span class="sxs-lookup"><span data-stu-id="9c730-116">**cameraModel**</span></span>         | <span data-ttu-id="9c730-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9c730-117">String</span></span>                    | <span data-ttu-id="9c730-p103">Modelo da câmera. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9c730-p103">Camera model. Read-only.</span></span>                                                   |
| <span data-ttu-id="9c730-120">**fNumber**</span><span class="sxs-lookup"><span data-stu-id="9c730-120">**fNumber**</span></span>             | <span data-ttu-id="9c730-121">Double</span><span class="sxs-lookup"><span data-stu-id="9c730-121">Double</span></span>                    | <span data-ttu-id="9c730-p104">O valor de f-stop da câmera. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9c730-p104">The F-stop value from the camera. Read-only.</span></span>                               |
| <span data-ttu-id="9c730-124">**exposureDenominator**</span><span class="sxs-lookup"><span data-stu-id="9c730-124">**exposureDenominator**</span></span> | <span data-ttu-id="9c730-125">Int32</span><span class="sxs-lookup"><span data-stu-id="9c730-125">Int32</span></span>                     | <span data-ttu-id="9c730-p105">O denominador da fração do tempo de exposição da câmera. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9c730-p105">The denominator for the exposure time fraction from the camera. Read-only.</span></span> |
| <span data-ttu-id="9c730-128">**exposureNumerator**</span><span class="sxs-lookup"><span data-stu-id="9c730-128">**exposureNumerator**</span></span>   | <span data-ttu-id="9c730-129">Int32</span><span class="sxs-lookup"><span data-stu-id="9c730-129">Int32</span></span>                     | <span data-ttu-id="9c730-p106">O numerador da fração do tempo de exposição da câmera. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9c730-p106">The numerator for the exposure time fraction from the camera. Read-only.</span></span>   |
| <span data-ttu-id="9c730-132">**focalLength**</span><span class="sxs-lookup"><span data-stu-id="9c730-132">**focalLength**</span></span>         | <span data-ttu-id="9c730-133">Double</span><span class="sxs-lookup"><span data-stu-id="9c730-133">Double</span></span>                    | <span data-ttu-id="9c730-p107">A distância focal da câmera. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9c730-p107">The focal length from the camera. Read-only.</span></span>                               |
| <span data-ttu-id="9c730-136">**iso**</span><span class="sxs-lookup"><span data-stu-id="9c730-136">**iso**</span></span>                 | <span data-ttu-id="9c730-137">Int32</span><span class="sxs-lookup"><span data-stu-id="9c730-137">Int32</span></span>                     | <span data-ttu-id="9c730-p108">O valor de ISO da câmera. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9c730-p108">The ISO value from the camera. Read-only.</span></span>                                  |

## <a name="remarks"></a><span data-ttu-id="9c730-140">Comentários</span><span class="sxs-lookup"><span data-stu-id="9c730-140">Remarks</span></span>
<span data-ttu-id="9c730-141">O OneDrive for Business e o SharePoint retornam apenas a propriedade **takenDateTime**.</span><span class="sxs-lookup"><span data-stu-id="9c730-141">OneDrive for Business and SharePoint only return the **takenDateTime** property.</span></span>

<span data-ttu-id="9c730-142">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="9c730-142">For more information about the facets on a [driveItem](driveitem.md), see driveItem.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "photo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
