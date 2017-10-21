---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Foto
ms.openlocfilehash: a4284caa7c20e266d87e22e9b3d729e17bc88abf
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/28/2017
---
# <a name="photo-resource-type"></a><span data-ttu-id="ea75b-102">Tipo de recurso Photo</span><span class="sxs-lookup"><span data-stu-id="ea75b-102">Photo resource type</span></span>

<span data-ttu-id="ea75b-103">O recurso **photo** fornece propriedades de foto e câmera, por exemplo, metadados EXIF, em um [driveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="ea75b-103">The **photo** resource provides photo and camera properties, for example, EXIF metadata, on a [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="ea75b-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ea75b-104">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.photo"
}-->
```json
{
  "cameraMake": "string",
  "cameraModel": "string",
  "exposureDenominator": 1000.0,
  "exposureNumerator": 1.0,
  "fNumber": 1.8,
  "focalLength": 22.5,
  "iso": 100,
  "takenDateTime": "String (timestamp)"
}
```

## <a name="properties"></a><span data-ttu-id="ea75b-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ea75b-105">Properties</span></span>

| <span data-ttu-id="ea75b-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ea75b-106">Property</span></span>                | <span data-ttu-id="ea75b-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="ea75b-107">Type</span></span>           | <span data-ttu-id="ea75b-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="ea75b-108">Description</span></span>
|:------------------------|:---------------|:----------------------------------
| <span data-ttu-id="ea75b-109">**takenDateTime**</span><span class="sxs-lookup"><span data-stu-id="ea75b-109">**takenDateTime**</span></span>       | <span data-ttu-id="ea75b-110">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ea75b-110">DateTimeOffset</span></span> | <span data-ttu-id="ea75b-p101">Representa a data e a hora em que a foto foi tirada. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ea75b-p101">Represents the date and time the photo was taken. Read-only.</span></span>
| <span data-ttu-id="ea75b-113">**cameraMake**</span><span class="sxs-lookup"><span data-stu-id="ea75b-113">**cameraMake**</span></span>          | <span data-ttu-id="ea75b-114">String</span><span class="sxs-lookup"><span data-stu-id="ea75b-114">String</span></span>         | <span data-ttu-id="ea75b-p102">Fabricante da câmera. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ea75b-p102">Camera manufacturer. Read-only.</span></span>
| <span data-ttu-id="ea75b-117">**cameraModel**</span><span class="sxs-lookup"><span data-stu-id="ea75b-117">**cameraModel**</span></span>         | <span data-ttu-id="ea75b-118">String</span><span class="sxs-lookup"><span data-stu-id="ea75b-118">String</span></span>         | <span data-ttu-id="ea75b-p103">Modelo da câmera. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ea75b-p103">Camera model. Read-only.</span></span>
| <span data-ttu-id="ea75b-121">**fNumber**</span><span class="sxs-lookup"><span data-stu-id="ea75b-121">**fNumber**</span></span>             | <span data-ttu-id="ea75b-122">Double</span><span class="sxs-lookup"><span data-stu-id="ea75b-122">Double</span></span>         | <span data-ttu-id="ea75b-p104">O valor de f-stop da câmera. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ea75b-p104">The F-stop value from the camera. Read-only.</span></span>
| <span data-ttu-id="ea75b-125">**exposureDenominator**</span><span class="sxs-lookup"><span data-stu-id="ea75b-125">**exposureDenominator**</span></span> | <span data-ttu-id="ea75b-126">Duplo</span><span class="sxs-lookup"><span data-stu-id="ea75b-126">Double</span></span>         | <span data-ttu-id="ea75b-p105">O denominador da fração do tempo de exposição da câmera. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ea75b-p105">The denominator for the exposure time fraction from the camera. Read-only.</span></span>
| <span data-ttu-id="ea75b-129">**exposureNumerator**</span><span class="sxs-lookup"><span data-stu-id="ea75b-129">**exposureNumerator**</span></span>   | <span data-ttu-id="ea75b-130">Duplo</span><span class="sxs-lookup"><span data-stu-id="ea75b-130">Double</span></span>         | <span data-ttu-id="ea75b-p106">O numerador da fração do tempo de exposição da câmera. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ea75b-p106">The numerator for the exposure time fraction from the camera. Read-only.</span></span>
| <span data-ttu-id="ea75b-133">**focalLength**</span><span class="sxs-lookup"><span data-stu-id="ea75b-133">**focalLength**</span></span>         | <span data-ttu-id="ea75b-134">Double</span><span class="sxs-lookup"><span data-stu-id="ea75b-134">Double</span></span>         | <span data-ttu-id="ea75b-p107">A distância focal da câmera. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ea75b-p107">The focal length from the camera. Read-only.</span></span>
| <span data-ttu-id="ea75b-137">**iso**</span><span class="sxs-lookup"><span data-stu-id="ea75b-137">**iso**</span></span>                 | <span data-ttu-id="ea75b-138">Int64</span><span class="sxs-lookup"><span data-stu-id="ea75b-138">Int64</span></span>          | <span data-ttu-id="ea75b-p108">O valor de ISO da câmera. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ea75b-p108">The ISO value from the camera. Read-only.</span></span>

## <a name="remarks"></a><span data-ttu-id="ea75b-141">Comentários</span><span class="sxs-lookup"><span data-stu-id="ea75b-141">Remarks</span></span>
<span data-ttu-id="ea75b-142">O OneDrive for Business e o SharePoint retornam apenas a propriedade **takenDateTime**.</span><span class="sxs-lookup"><span data-stu-id="ea75b-142">OneDrive for Business and SharePoint only return the **takenDateTime** property.</span></span>

<span data-ttu-id="ea75b-143">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="ea75b-143">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>
<!-- {
  "type": "#page.annotation",
  "description": "The photo facet provides details about the camera and settings on the camera for photos.",
  "keywords": "camera make,camera model, exposure, f-stop, iso",
  "section": "documentation",
  "tocPath": "Facets/Photo"
} -->
