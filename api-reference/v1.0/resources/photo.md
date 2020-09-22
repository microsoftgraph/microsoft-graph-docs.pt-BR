---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Photo
localization_priority: Normal
description: O recurso photo fornece propriedades de foto e câmera, por exemplo, metadados EXIF, em um driveItem.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 362d4f76f56fa5824985a3580d6008d8c5081a7c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48072848"
---
# <a name="photo-resource-type"></a><span data-ttu-id="f473d-103">Tipo de recurso Photo</span><span class="sxs-lookup"><span data-stu-id="f473d-103">Photo resource type</span></span>

<span data-ttu-id="f473d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f473d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f473d-105">O recurso **photo** fornece propriedades de foto e câmera, por exemplo, metadados EXIF, em um [driveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="f473d-105">The **photo** resource provides photo and camera properties, for example, EXIF metadata, on a [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="f473d-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f473d-106">JSON representation</span></span>

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
  "orientation": 3,
  "takenDateTime": "String (timestamp)"
}
```

## <a name="properties"></a><span data-ttu-id="f473d-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f473d-107">Properties</span></span>

| <span data-ttu-id="f473d-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f473d-108">Property</span></span>                | <span data-ttu-id="f473d-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="f473d-109">Type</span></span>           | <span data-ttu-id="f473d-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="f473d-110">Description</span></span>
|:------------------------|:---------------|:----------------------------------
| <span data-ttu-id="f473d-111">**takenDateTime**</span><span class="sxs-lookup"><span data-stu-id="f473d-111">**takenDateTime**</span></span>       | <span data-ttu-id="f473d-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f473d-112">DateTimeOffset</span></span> | <span data-ttu-id="f473d-p101">Representa a data e a hora em que a foto foi tirada. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f473d-p101">Represents the date and time the photo was taken. Read-only.</span></span>
| <span data-ttu-id="f473d-115">**cameraMake**</span><span class="sxs-lookup"><span data-stu-id="f473d-115">**cameraMake**</span></span>          | <span data-ttu-id="f473d-116">String</span><span class="sxs-lookup"><span data-stu-id="f473d-116">String</span></span>         | <span data-ttu-id="f473d-p102">Fabricante da câmera. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f473d-p102">Camera manufacturer. Read-only.</span></span>
| <span data-ttu-id="f473d-119">**cameraModel**</span><span class="sxs-lookup"><span data-stu-id="f473d-119">**cameraModel**</span></span>         | <span data-ttu-id="f473d-120">String</span><span class="sxs-lookup"><span data-stu-id="f473d-120">String</span></span>         | <span data-ttu-id="f473d-p103">Modelo da câmera. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f473d-p103">Camera model. Read-only.</span></span>
| <span data-ttu-id="f473d-123">**fNumber**</span><span class="sxs-lookup"><span data-stu-id="f473d-123">**fNumber**</span></span>             | <span data-ttu-id="f473d-124">Double</span><span class="sxs-lookup"><span data-stu-id="f473d-124">Double</span></span>         | <span data-ttu-id="f473d-p104">O valor de f-stop da câmera. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f473d-p104">The F-stop value from the camera. Read-only.</span></span>
| <span data-ttu-id="f473d-127">**exposureDenominator**</span><span class="sxs-lookup"><span data-stu-id="f473d-127">**exposureDenominator**</span></span> | <span data-ttu-id="f473d-128">Duplo</span><span class="sxs-lookup"><span data-stu-id="f473d-128">Double</span></span>         | <span data-ttu-id="f473d-p105">O denominador da fração do tempo de exposição da câmera. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f473d-p105">The denominator for the exposure time fraction from the camera. Read-only.</span></span>
| <span data-ttu-id="f473d-131">**exposureNumerator**</span><span class="sxs-lookup"><span data-stu-id="f473d-131">**exposureNumerator**</span></span>   | <span data-ttu-id="f473d-132">Duplo</span><span class="sxs-lookup"><span data-stu-id="f473d-132">Double</span></span>         | <span data-ttu-id="f473d-p106">O numerador da fração do tempo de exposição da câmera. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f473d-p106">The numerator for the exposure time fraction from the camera. Read-only.</span></span>
| <span data-ttu-id="f473d-135">**focalLength**</span><span class="sxs-lookup"><span data-stu-id="f473d-135">**focalLength**</span></span>         | <span data-ttu-id="f473d-136">Double</span><span class="sxs-lookup"><span data-stu-id="f473d-136">Double</span></span>         | <span data-ttu-id="f473d-p107">A distância focal da câmera. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f473d-p107">The focal length from the camera. Read-only.</span></span>
| <span data-ttu-id="f473d-139">**iso**</span><span class="sxs-lookup"><span data-stu-id="f473d-139">**iso**</span></span>                 | <span data-ttu-id="f473d-140">Int32</span><span class="sxs-lookup"><span data-stu-id="f473d-140">Int32</span></span>          | <span data-ttu-id="f473d-p108">O valor de ISO da câmera. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f473d-p108">The ISO value from the camera. Read-only.</span></span>
| <span data-ttu-id="f473d-143">**orientation**</span><span class="sxs-lookup"><span data-stu-id="f473d-143">**orientation**</span></span>         | <span data-ttu-id="f473d-144">Int16</span><span class="sxs-lookup"><span data-stu-id="f473d-144">Int16</span></span>          | <span data-ttu-id="f473d-145">O valor da orientação da câmera.</span><span class="sxs-lookup"><span data-stu-id="f473d-145">The orientation value from the camera.</span></span> <span data-ttu-id="f473d-146">Gravável no OneDrive Personal.</span><span class="sxs-lookup"><span data-stu-id="f473d-146">Writable on OneDrive Personal.</span></span>      |

## <a name="remarks"></a><span data-ttu-id="f473d-147">Comentários</span><span class="sxs-lookup"><span data-stu-id="f473d-147">Remarks</span></span>

<span data-ttu-id="f473d-148">O OneDrive for Business e o SharePoint retornam apenas a propriedade **takenDateTime**.</span><span class="sxs-lookup"><span data-stu-id="f473d-148">OneDrive for Business and SharePoint only return the **takenDateTime** property.</span></span>

<span data-ttu-id="f473d-149">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="f473d-149">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>
<!-- {
  "type": "#page.annotation",
  "description": "The photo facet provides details about the camera and settings on the camera for photos.",
  "keywords": "camera make,camera model, exposure, f-stop, iso, orientation",
  "section": "documentation",
  "tocPath": "Facets/Photo"
} -->

