---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Foto
localization_priority: Normal
description: O recurso photo fornece propriedades de foto e câmera, por exemplo, metadados EXIF, em um driveItem.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 4e3f167384112c3c3354cdff88b41632f92e2637
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42534053"
---
# <a name="photo-resource-type"></a><span data-ttu-id="d3cef-103">Tipo de recurso Photo</span><span class="sxs-lookup"><span data-stu-id="d3cef-103">Photo resource type</span></span>

<span data-ttu-id="d3cef-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d3cef-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d3cef-105">O recurso **photo** fornece propriedades de foto e câmera, por exemplo, metadados EXIF, em um [driveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="d3cef-105">The **photo** resource provides photo and camera properties, for example, EXIF metadata, on a [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="d3cef-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d3cef-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="d3cef-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d3cef-107">Properties</span></span>

| <span data-ttu-id="d3cef-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d3cef-108">Property</span></span>                | <span data-ttu-id="d3cef-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="d3cef-109">Type</span></span>           | <span data-ttu-id="d3cef-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="d3cef-110">Description</span></span>
|:------------------------|:---------------|:----------------------------------
| <span data-ttu-id="d3cef-111">**takenDateTime**</span><span class="sxs-lookup"><span data-stu-id="d3cef-111">**takenDateTime**</span></span>       | <span data-ttu-id="d3cef-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d3cef-112">DateTimeOffset</span></span> | <span data-ttu-id="d3cef-p101">Representa a data e a hora em que a foto foi tirada. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d3cef-p101">Represents the date and time the photo was taken. Read-only.</span></span>
| <span data-ttu-id="d3cef-115">**cameraMake**</span><span class="sxs-lookup"><span data-stu-id="d3cef-115">**cameraMake**</span></span>          | <span data-ttu-id="d3cef-116">String</span><span class="sxs-lookup"><span data-stu-id="d3cef-116">String</span></span>         | <span data-ttu-id="d3cef-p102">Fabricante da câmera. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d3cef-p102">Camera manufacturer. Read-only.</span></span>
| <span data-ttu-id="d3cef-119">**cameraModel**</span><span class="sxs-lookup"><span data-stu-id="d3cef-119">**cameraModel**</span></span>         | <span data-ttu-id="d3cef-120">String</span><span class="sxs-lookup"><span data-stu-id="d3cef-120">String</span></span>         | <span data-ttu-id="d3cef-p103">Modelo da câmera. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d3cef-p103">Camera model. Read-only.</span></span>
| <span data-ttu-id="d3cef-123">**fNumber**</span><span class="sxs-lookup"><span data-stu-id="d3cef-123">**fNumber**</span></span>             | <span data-ttu-id="d3cef-124">Duplo</span><span class="sxs-lookup"><span data-stu-id="d3cef-124">Double</span></span>         | <span data-ttu-id="d3cef-p104">O valor de f-stop da câmera. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d3cef-p104">The F-stop value from the camera. Read-only.</span></span>
| <span data-ttu-id="d3cef-127">**exposureDenominator**</span><span class="sxs-lookup"><span data-stu-id="d3cef-127">**exposureDenominator**</span></span> | <span data-ttu-id="d3cef-128">Duplo</span><span class="sxs-lookup"><span data-stu-id="d3cef-128">Double</span></span>         | <span data-ttu-id="d3cef-p105">O denominador da fração do tempo de exposição da câmera. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d3cef-p105">The denominator for the exposure time fraction from the camera. Read-only.</span></span>
| <span data-ttu-id="d3cef-131">**exposureNumerator**</span><span class="sxs-lookup"><span data-stu-id="d3cef-131">**exposureNumerator**</span></span>   | <span data-ttu-id="d3cef-132">Duplo</span><span class="sxs-lookup"><span data-stu-id="d3cef-132">Double</span></span>         | <span data-ttu-id="d3cef-p106">O numerador da fração do tempo de exposição da câmera. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d3cef-p106">The numerator for the exposure time fraction from the camera. Read-only.</span></span>
| <span data-ttu-id="d3cef-135">**focalLength**</span><span class="sxs-lookup"><span data-stu-id="d3cef-135">**focalLength**</span></span>         | <span data-ttu-id="d3cef-136">Double</span><span class="sxs-lookup"><span data-stu-id="d3cef-136">Double</span></span>         | <span data-ttu-id="d3cef-p107">A distância focal da câmera. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d3cef-p107">The focal length from the camera. Read-only.</span></span>
| <span data-ttu-id="d3cef-139">**iso**</span><span class="sxs-lookup"><span data-stu-id="d3cef-139">**iso**</span></span>                 | <span data-ttu-id="d3cef-140">Int32</span><span class="sxs-lookup"><span data-stu-id="d3cef-140">Int32</span></span>          | <span data-ttu-id="d3cef-p108">O valor de ISO da câmera. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d3cef-p108">The ISO value from the camera. Read-only.</span></span>

## <a name="remarks"></a><span data-ttu-id="d3cef-143">Comentários</span><span class="sxs-lookup"><span data-stu-id="d3cef-143">Remarks</span></span>

<span data-ttu-id="d3cef-144">O OneDrive for Business e o SharePoint retornam apenas a propriedade **takenDateTime**.</span><span class="sxs-lookup"><span data-stu-id="d3cef-144">OneDrive for Business and SharePoint only return the **takenDateTime** property.</span></span>

<span data-ttu-id="d3cef-145">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="d3cef-145">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>
<!-- {
  "type": "#page.annotation",
  "description": "The photo facet provides details about the camera and settings on the camera for photos.",
  "keywords": "camera make,camera model, exposure, f-stop, iso",
  "section": "documentation",
  "tocPath": "Facets/Photo"
} -->
