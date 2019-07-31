---
author: JeremyKelley
description: O recurso photo fornece propriedades de foto e câmera, por exemplo, metadados EXIF, em um driveItem.
ms.date: 09/10/2017
title: Foto
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 6713e66b5ca14cfa6605b9e67d4bec152a321f33
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009220"
---
# <a name="photo-resource-type"></a><span data-ttu-id="44bcb-103">Tipo de recurso Photo</span><span class="sxs-lookup"><span data-stu-id="44bcb-103">Photo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="44bcb-104">O recurso **photo** fornece propriedades de foto e câmera, por exemplo, metadados EXIF, em um [driveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="44bcb-104">The **photo** resource provides photo and camera properties, for example, EXIF metadata, on a [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="44bcb-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="44bcb-105">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="44bcb-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="44bcb-106">Properties</span></span>

| <span data-ttu-id="44bcb-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="44bcb-107">Property</span></span>                | <span data-ttu-id="44bcb-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="44bcb-108">Type</span></span>           | <span data-ttu-id="44bcb-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="44bcb-109">Description</span></span>
|:------------------------|:---------------|:----------------------------------
| <span data-ttu-id="44bcb-110">**takenDateTime**</span><span class="sxs-lookup"><span data-stu-id="44bcb-110">**takenDateTime**</span></span>       | <span data-ttu-id="44bcb-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="44bcb-111">DateTimeOffset</span></span> | <span data-ttu-id="44bcb-p101">Representa a data e a hora em que a foto foi tirada. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="44bcb-p101">Represents the date and time the photo was taken. Read-only.</span></span>
| <span data-ttu-id="44bcb-114">**cameraMake**</span><span class="sxs-lookup"><span data-stu-id="44bcb-114">**cameraMake**</span></span>          | <span data-ttu-id="44bcb-115">String</span><span class="sxs-lookup"><span data-stu-id="44bcb-115">String</span></span>         | <span data-ttu-id="44bcb-p102">Fabricante da câmera. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="44bcb-p102">Camera manufacturer. Read-only.</span></span>
| <span data-ttu-id="44bcb-118">**cameraModel**</span><span class="sxs-lookup"><span data-stu-id="44bcb-118">**cameraModel**</span></span>         | <span data-ttu-id="44bcb-119">String</span><span class="sxs-lookup"><span data-stu-id="44bcb-119">String</span></span>         | <span data-ttu-id="44bcb-p103">Modelo da câmera. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="44bcb-p103">Camera model. Read-only.</span></span>
| <span data-ttu-id="44bcb-122">**fNumber**</span><span class="sxs-lookup"><span data-stu-id="44bcb-122">**fNumber**</span></span>             | <span data-ttu-id="44bcb-123">Duplo</span><span class="sxs-lookup"><span data-stu-id="44bcb-123">Double</span></span>         | <span data-ttu-id="44bcb-p104">O valor de f-stop da câmera. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="44bcb-p104">The F-stop value from the camera. Read-only.</span></span>
| <span data-ttu-id="44bcb-126">**exposureDenominator**</span><span class="sxs-lookup"><span data-stu-id="44bcb-126">**exposureDenominator**</span></span> | <span data-ttu-id="44bcb-127">Duplo</span><span class="sxs-lookup"><span data-stu-id="44bcb-127">Double</span></span>         | <span data-ttu-id="44bcb-p105">O denominador da fração do tempo de exposição da câmera. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="44bcb-p105">The denominator for the exposure time fraction from the camera. Read-only.</span></span>
| <span data-ttu-id="44bcb-130">**exposureNumerator**</span><span class="sxs-lookup"><span data-stu-id="44bcb-130">**exposureNumerator**</span></span>   | <span data-ttu-id="44bcb-131">Duplo</span><span class="sxs-lookup"><span data-stu-id="44bcb-131">Double</span></span>         | <span data-ttu-id="44bcb-p106">O numerador da fração do tempo de exposição da câmera. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="44bcb-p106">The numerator for the exposure time fraction from the camera. Read-only.</span></span>
| <span data-ttu-id="44bcb-134">**focalLength**</span><span class="sxs-lookup"><span data-stu-id="44bcb-134">**focalLength**</span></span>         | <span data-ttu-id="44bcb-135">Double</span><span class="sxs-lookup"><span data-stu-id="44bcb-135">Double</span></span>         | <span data-ttu-id="44bcb-p107">A distância focal da câmera. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="44bcb-p107">The focal length from the camera. Read-only.</span></span>
| <span data-ttu-id="44bcb-138">**iso**</span><span class="sxs-lookup"><span data-stu-id="44bcb-138">**iso**</span></span>                 | <span data-ttu-id="44bcb-139">Int64</span><span class="sxs-lookup"><span data-stu-id="44bcb-139">Int64</span></span>          | <span data-ttu-id="44bcb-p108">O valor de ISO da câmera. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="44bcb-p108">The ISO value from the camera. Read-only.</span></span>

## <a name="remarks"></a><span data-ttu-id="44bcb-142">Comentários</span><span class="sxs-lookup"><span data-stu-id="44bcb-142">Remarks</span></span>
<span data-ttu-id="44bcb-143">O OneDrive for Business e o SharePoint retornam apenas a propriedade **takenDateTime**.</span><span class="sxs-lookup"><span data-stu-id="44bcb-143">OneDrive for Business and SharePoint only return the **takenDateTime** property.</span></span>

<span data-ttu-id="44bcb-144">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="44bcb-144">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>
<!--
{
  "type": "#page.annotation",
  "description": "The photo facet provides details about the camera and settings on the camera for photos.",
  "keywords": "camera make,camera model, exposure, f-stop, iso",
  "section": "documentation",
  "tocPath": "Facets/Photo",
  "suppressions": []
}
-->
