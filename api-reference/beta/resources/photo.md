---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Foto
localization_priority: Normal
ms.openlocfilehash: 91b893fe3d6c78e3c3e16cbc41c7d7543b08f8d7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29527623"
---
# <a name="photo-resource-type"></a><span data-ttu-id="ac258-102">Tipo de recurso Photo</span><span class="sxs-lookup"><span data-stu-id="ac258-102">Photo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ac258-103">O recurso **photo** fornece propriedades de foto e câmera, por exemplo, metadados EXIF, em um [driveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="ac258-103">The **photo** resource provides photo and camera properties, for example, EXIF metadata, on a [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="ac258-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ac258-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="ac258-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ac258-105">Properties</span></span>

| <span data-ttu-id="ac258-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ac258-106">Property</span></span>                | <span data-ttu-id="ac258-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="ac258-107">Type</span></span>           | <span data-ttu-id="ac258-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="ac258-108">Description</span></span>
|:------------------------|:---------------|:----------------------------------
| <span data-ttu-id="ac258-109">**takenDateTime**</span><span class="sxs-lookup"><span data-stu-id="ac258-109">**takenDateTime**</span></span>       | <span data-ttu-id="ac258-110">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ac258-110">DateTimeOffset</span></span> | <span data-ttu-id="ac258-p101">Representa a data e a hora em que a foto foi tirada. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ac258-p101">Represents the date and time the photo was taken. Read-only.</span></span>
| <span data-ttu-id="ac258-113">**cameraMake**</span><span class="sxs-lookup"><span data-stu-id="ac258-113">**cameraMake**</span></span>          | <span data-ttu-id="ac258-114">String</span><span class="sxs-lookup"><span data-stu-id="ac258-114">String</span></span>         | <span data-ttu-id="ac258-p102">Fabricante da câmera. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ac258-p102">Camera manufacturer. Read-only.</span></span>
| <span data-ttu-id="ac258-117">**cameraModel**</span><span class="sxs-lookup"><span data-stu-id="ac258-117">**cameraModel**</span></span>         | <span data-ttu-id="ac258-118">String</span><span class="sxs-lookup"><span data-stu-id="ac258-118">String</span></span>         | <span data-ttu-id="ac258-p103">Modelo da câmera. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ac258-p103">Camera model. Read-only.</span></span>
| <span data-ttu-id="ac258-121">**fNumber**</span><span class="sxs-lookup"><span data-stu-id="ac258-121">**fNumber**</span></span>             | <span data-ttu-id="ac258-122">Double</span><span class="sxs-lookup"><span data-stu-id="ac258-122">Double</span></span>         | <span data-ttu-id="ac258-p104">O valor de f-stop da câmera. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ac258-p104">The F-stop value from the camera. Read-only.</span></span>
| <span data-ttu-id="ac258-125">**exposureDenominator**</span><span class="sxs-lookup"><span data-stu-id="ac258-125">**exposureDenominator**</span></span> | <span data-ttu-id="ac258-126">Duplo</span><span class="sxs-lookup"><span data-stu-id="ac258-126">Double</span></span>         | <span data-ttu-id="ac258-p105">O denominador da fração do tempo de exposição da câmera. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ac258-p105">The denominator for the exposure time fraction from the camera. Read-only.</span></span>
| <span data-ttu-id="ac258-129">**exposureNumerator**</span><span class="sxs-lookup"><span data-stu-id="ac258-129">**exposureNumerator**</span></span>   | <span data-ttu-id="ac258-130">Duplo</span><span class="sxs-lookup"><span data-stu-id="ac258-130">Double</span></span>         | <span data-ttu-id="ac258-p106">O numerador da fração do tempo de exposição da câmera. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ac258-p106">The numerator for the exposure time fraction from the camera. Read-only.</span></span>
| <span data-ttu-id="ac258-133">**focalLength**</span><span class="sxs-lookup"><span data-stu-id="ac258-133">**focalLength**</span></span>         | <span data-ttu-id="ac258-134">Double</span><span class="sxs-lookup"><span data-stu-id="ac258-134">Double</span></span>         | <span data-ttu-id="ac258-p107">A distância focal da câmera. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ac258-p107">The focal length from the camera. Read-only.</span></span>
| <span data-ttu-id="ac258-137">**iso**</span><span class="sxs-lookup"><span data-stu-id="ac258-137">**iso**</span></span>                 | <span data-ttu-id="ac258-138">Int64</span><span class="sxs-lookup"><span data-stu-id="ac258-138">Int64</span></span>          | <span data-ttu-id="ac258-p108">O valor de ISO da câmera. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ac258-p108">The ISO value from the camera. Read-only.</span></span>

## <a name="remarks"></a><span data-ttu-id="ac258-141">Comentários</span><span class="sxs-lookup"><span data-stu-id="ac258-141">Remarks</span></span>
<span data-ttu-id="ac258-142">O OneDrive for Business e o SharePoint retornam apenas a propriedade **takenDateTime**.</span><span class="sxs-lookup"><span data-stu-id="ac258-142">OneDrive for Business and SharePoint only return the **takenDateTime** property.</span></span>

<span data-ttu-id="ac258-143">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="ac258-143">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>
<!--
{
  "type": "#page.annotation",
  "description": "The photo facet provides details about the camera and settings on the camera for photos.",
  "keywords": "camera make,camera model, exposure, f-stop, iso",
  "section": "documentation",
  "tocPath": "Facets/Photo",
  "suppressions": [
    "Error: /api-reference/beta/resources/photo.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
