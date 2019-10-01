---
title: tipo de recurso Photo
description: O recurso photo fornece propriedades de foto e câmera, por exemplo, metadados EXIF, em um driveItem.
ms.date: 09/10/2017
localization_priority: Normal
author: JeremyKelley
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: ed3d60fabfd367668b5c7a8230bba0f19f7d88f5
ms.sourcegitcommit: 2fb178ae78b5ecc47207d2b19d0c5a46e07e0960
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/01/2019
ms.locfileid: "37333238"
---
# <a name="photo-resource-type"></a><span data-ttu-id="516ba-103">tipo de recurso Photo</span><span class="sxs-lookup"><span data-stu-id="516ba-103">photo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="516ba-104">O recurso **photo** fornece propriedades de foto e câmera, por exemplo, metadados EXIF, em um [driveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="516ba-104">The **photo** resource provides photo and camera properties, for example, EXIF metadata, on a [driveItem](driveitem.md).</span></span>

> [!NOTE]
> <span data-ttu-id="516ba-105">Atualmente, apenas o **takenDateTime** está disponível no onedrive for Business e no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="516ba-105">Currently, only **takenDateTime** is available on OneDrive for Business and SharePoint.</span></span>

## <a name="properties"></a><span data-ttu-id="516ba-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="516ba-106">Properties</span></span>

| <span data-ttu-id="516ba-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="516ba-107">Property</span></span>          | <span data-ttu-id="516ba-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="516ba-108">Type</span></span>          | <span data-ttu-id="516ba-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="516ba-109">Description</span></span>                                                                |
|:------------------|:--------------|:---------------------------------------------------------------------------|
|<span data-ttu-id="516ba-110">cameraMake</span><span class="sxs-lookup"><span data-stu-id="516ba-110">cameraMake</span></span>         |<span data-ttu-id="516ba-111">String</span><span class="sxs-lookup"><span data-stu-id="516ba-111">String</span></span>         | <span data-ttu-id="516ba-p101">Fabricante da câmera. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="516ba-p101">Camera manufacturer. Read-only.</span></span>                                            |
|<span data-ttu-id="516ba-114">cameraModel</span><span class="sxs-lookup"><span data-stu-id="516ba-114">cameraModel</span></span>        |<span data-ttu-id="516ba-115">String</span><span class="sxs-lookup"><span data-stu-id="516ba-115">String</span></span>         | <span data-ttu-id="516ba-p102">Modelo da câmera. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="516ba-p102">Camera model. Read-only.</span></span>                                                   |
|<span data-ttu-id="516ba-118">exposureDenominator</span><span class="sxs-lookup"><span data-stu-id="516ba-118">exposureDenominator</span></span>|<span data-ttu-id="516ba-119">Duplo</span><span class="sxs-lookup"><span data-stu-id="516ba-119">Double</span></span>         | <span data-ttu-id="516ba-p103">O denominador da fração do tempo de exposição da câmera. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="516ba-p103">The denominator for the exposure time fraction from the camera. Read-only.</span></span> |
|<span data-ttu-id="516ba-122">exposureNumerator</span><span class="sxs-lookup"><span data-stu-id="516ba-122">exposureNumerator</span></span>  |<span data-ttu-id="516ba-123">Duplo</span><span class="sxs-lookup"><span data-stu-id="516ba-123">Double</span></span>         | <span data-ttu-id="516ba-p104">O numerador da fração do tempo de exposição da câmera. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="516ba-p104">The numerator for the exposure time fraction from the camera. Read-only.</span></span>   |
|<span data-ttu-id="516ba-126">fNumber</span><span class="sxs-lookup"><span data-stu-id="516ba-126">fNumber</span></span>            |<span data-ttu-id="516ba-127">Duplo</span><span class="sxs-lookup"><span data-stu-id="516ba-127">Double</span></span>         | <span data-ttu-id="516ba-p105">O valor de f-stop da câmera. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="516ba-p105">The F-stop value from the camera. Read-only.</span></span>                               |
|<span data-ttu-id="516ba-130">focalLength</span><span class="sxs-lookup"><span data-stu-id="516ba-130">focalLength</span></span>        |<span data-ttu-id="516ba-131">Double</span><span class="sxs-lookup"><span data-stu-id="516ba-131">Double</span></span>         | <span data-ttu-id="516ba-p106">A distância focal da câmera. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="516ba-p106">The focal length from the camera. Read-only.</span></span>                               |
|<span data-ttu-id="516ba-134">iso</span><span class="sxs-lookup"><span data-stu-id="516ba-134">iso</span></span>                |<span data-ttu-id="516ba-135">Int32</span><span class="sxs-lookup"><span data-stu-id="516ba-135">Int32</span></span>          | <span data-ttu-id="516ba-p107">O valor de ISO da câmera. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="516ba-p107">The ISO value from the camera. Read-only.</span></span>                                  |
|<span data-ttu-id="516ba-138">orientation</span><span class="sxs-lookup"><span data-stu-id="516ba-138">orientation</span></span>        |<span data-ttu-id="516ba-139">Int16</span><span class="sxs-lookup"><span data-stu-id="516ba-139">Int16</span></span>          | <span data-ttu-id="516ba-140">O valor da orientação da câmera.</span><span class="sxs-lookup"><span data-stu-id="516ba-140">The orientation value from the camera.</span></span> <span data-ttu-id="516ba-141">Gravável no OneDrive Personal.</span><span class="sxs-lookup"><span data-stu-id="516ba-141">Writable on OneDrive Personal.</span></span>      |
|<span data-ttu-id="516ba-142">takenDateTime</span><span class="sxs-lookup"><span data-stu-id="516ba-142">takenDateTime</span></span>      |<span data-ttu-id="516ba-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="516ba-143">DateTimeOffset</span></span> | <span data-ttu-id="516ba-144">A data e a hora em que a foto foi tirada no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="516ba-144">The date and time the photo was taken in UTC time.</span></span> <span data-ttu-id="516ba-145">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="516ba-145">Read-only.</span></span>              |

## <a name="json-representation"></a><span data-ttu-id="516ba-146">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="516ba-146">JSON representation</span></span>

<span data-ttu-id="516ba-147">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="516ba-147">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.photo",
  "baseType": null
}-->

```json
{
  "cameraMake": "String",
  "cameraModel": "String",
  "exposureDenominator": 1000.0,
  "exposureNumerator": 1.0,
  "fNumber": 1.8,
  "focalLength": 22.5,
  "iso": 100,
  "orientation": 3,
  "takenDateTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The photo resource provides details about the camera and settings on the camera for photos.",
  "keywords": "camera make,camera model, exposure, f-stop, iso, orientation",
  "section": "documentation",
  "tocPath": ""
}-->
