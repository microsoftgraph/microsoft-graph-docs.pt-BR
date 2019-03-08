---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Foto
localization_priority: Normal
ms.openlocfilehash: d14777b0f39983d6ccf83ae387896c6587635e66
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2019
ms.locfileid: "30480912"
---
# <a name="photo-resource-type"></a><span data-ttu-id="9c943-102">Tipo de recurso Photo</span><span class="sxs-lookup"><span data-stu-id="9c943-102">Photo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9c943-103">O recurso **photo** fornece propriedades de foto e câmera, por exemplo, metadados EXIF, em um [driveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="9c943-103">The **photo** resource provides photo and camera properties, for example, EXIF metadata, on a [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="9c943-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9c943-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="9c943-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9c943-105">Properties</span></span>

| <span data-ttu-id="9c943-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9c943-106">Property</span></span>                | <span data-ttu-id="9c943-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="9c943-107">Type</span></span>           | <span data-ttu-id="9c943-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="9c943-108">Description</span></span>
|:------------------------|:---------------|:----------------------------------
| <span data-ttu-id="9c943-109">**takenDateTime**</span><span class="sxs-lookup"><span data-stu-id="9c943-109">**takenDateTime**</span></span>       | <span data-ttu-id="9c943-110">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9c943-110">DateTimeOffset</span></span> | <span data-ttu-id="9c943-p101">Representa a data e a hora em que a foto foi tirada. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9c943-p101">Represents the date and time the photo was taken. Read-only.</span></span>
| <span data-ttu-id="9c943-113">**cameraMake**</span><span class="sxs-lookup"><span data-stu-id="9c943-113">**cameraMake**</span></span>          | <span data-ttu-id="9c943-114">String</span><span class="sxs-lookup"><span data-stu-id="9c943-114">String</span></span>         | <span data-ttu-id="9c943-p102">Fabricante da câmera. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9c943-p102">Camera manufacturer. Read-only.</span></span>
| <span data-ttu-id="9c943-117">**cameraModel**</span><span class="sxs-lookup"><span data-stu-id="9c943-117">**cameraModel**</span></span>         | <span data-ttu-id="9c943-118">String</span><span class="sxs-lookup"><span data-stu-id="9c943-118">String</span></span>         | <span data-ttu-id="9c943-p103">Modelo da câmera. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9c943-p103">Camera model. Read-only.</span></span>
| <span data-ttu-id="9c943-121">**fNumber**</span><span class="sxs-lookup"><span data-stu-id="9c943-121">**fNumber**</span></span>             | <span data-ttu-id="9c943-122">Duplo</span><span class="sxs-lookup"><span data-stu-id="9c943-122">Double</span></span>         | <span data-ttu-id="9c943-p104">O valor de f-stop da câmera. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9c943-p104">The F-stop value from the camera. Read-only.</span></span>
| <span data-ttu-id="9c943-125">**exposureDenominator**</span><span class="sxs-lookup"><span data-stu-id="9c943-125">**exposureDenominator**</span></span> | <span data-ttu-id="9c943-126">Duplo</span><span class="sxs-lookup"><span data-stu-id="9c943-126">Double</span></span>         | <span data-ttu-id="9c943-p105">O denominador da fração do tempo de exposição da câmera. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9c943-p105">The denominator for the exposure time fraction from the camera. Read-only.</span></span>
| <span data-ttu-id="9c943-129">**exposureNumerator**</span><span class="sxs-lookup"><span data-stu-id="9c943-129">**exposureNumerator**</span></span>   | <span data-ttu-id="9c943-130">Duplo</span><span class="sxs-lookup"><span data-stu-id="9c943-130">Double</span></span>         | <span data-ttu-id="9c943-p106">O numerador da fração do tempo de exposição da câmera. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9c943-p106">The numerator for the exposure time fraction from the camera. Read-only.</span></span>
| <span data-ttu-id="9c943-133">**focalLength**</span><span class="sxs-lookup"><span data-stu-id="9c943-133">**focalLength**</span></span>         | <span data-ttu-id="9c943-134">Double</span><span class="sxs-lookup"><span data-stu-id="9c943-134">Double</span></span>         | <span data-ttu-id="9c943-p107">A distância focal da câmera. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9c943-p107">The focal length from the camera. Read-only.</span></span>
| <span data-ttu-id="9c943-137">**iso**</span><span class="sxs-lookup"><span data-stu-id="9c943-137">**iso**</span></span>                 | <span data-ttu-id="9c943-138">Int64</span><span class="sxs-lookup"><span data-stu-id="9c943-138">Int64</span></span>          | <span data-ttu-id="9c943-p108">O valor de ISO da câmera. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9c943-p108">The ISO value from the camera. Read-only.</span></span>

## <a name="remarks"></a><span data-ttu-id="9c943-141">Comentários</span><span class="sxs-lookup"><span data-stu-id="9c943-141">Remarks</span></span>
<span data-ttu-id="9c943-142">O OneDrive for Business e o SharePoint retornam apenas a propriedade **takenDateTime**.</span><span class="sxs-lookup"><span data-stu-id="9c943-142">OneDrive for Business and SharePoint only return the **takenDateTime** property.</span></span>

<span data-ttu-id="9c943-143">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="9c943-143">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>
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
