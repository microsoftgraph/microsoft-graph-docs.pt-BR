---
title: tipo de recurso Photo
description: O recurso photo fornece propriedades de foto e câmera, por exemplo, metadados EXIF, em um driveItem.
ms.date: 09/10/2017
localization_priority: Normal
author: JeremyKelley
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 920d6e69367517b1324b6cb66b755b6b58192219
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47997820"
---
# <a name="photo-resource-type"></a><span data-ttu-id="b8ec9-103">tipo de recurso Photo</span><span class="sxs-lookup"><span data-stu-id="b8ec9-103">photo resource type</span></span>

<span data-ttu-id="b8ec9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b8ec9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b8ec9-105">O recurso **photo** fornece propriedades de foto e câmera, por exemplo, metadados EXIF, em um [driveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="b8ec9-105">The **photo** resource provides photo and camera properties, for example, EXIF metadata, on a [driveItem](driveitem.md).</span></span>

> [!NOTE]
> <span data-ttu-id="b8ec9-106">Atualmente, apenas o **takenDateTime** está disponível no onedrive for Business e no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="b8ec9-106">Currently, only **takenDateTime** is available on OneDrive for Business and SharePoint.</span></span>

## <a name="properties"></a><span data-ttu-id="b8ec9-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b8ec9-107">Properties</span></span>

| <span data-ttu-id="b8ec9-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b8ec9-108">Property</span></span>          | <span data-ttu-id="b8ec9-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="b8ec9-109">Type</span></span>          | <span data-ttu-id="b8ec9-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="b8ec9-110">Description</span></span>                                                                |
|:------------------|:--------------|:---------------------------------------------------------------------------|
|<span data-ttu-id="b8ec9-111">cameraMake</span><span class="sxs-lookup"><span data-stu-id="b8ec9-111">cameraMake</span></span>         |<span data-ttu-id="b8ec9-112">String</span><span class="sxs-lookup"><span data-stu-id="b8ec9-112">String</span></span>         | <span data-ttu-id="b8ec9-p101">Fabricante da câmera. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b8ec9-p101">Camera manufacturer. Read-only.</span></span>                                            |
|<span data-ttu-id="b8ec9-115">cameraModel</span><span class="sxs-lookup"><span data-stu-id="b8ec9-115">cameraModel</span></span>        |<span data-ttu-id="b8ec9-116">String</span><span class="sxs-lookup"><span data-stu-id="b8ec9-116">String</span></span>         | <span data-ttu-id="b8ec9-p102">Modelo da câmera. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b8ec9-p102">Camera model. Read-only.</span></span>                                                   |
|<span data-ttu-id="b8ec9-119">exposureDenominator</span><span class="sxs-lookup"><span data-stu-id="b8ec9-119">exposureDenominator</span></span>|<span data-ttu-id="b8ec9-120">Duplo</span><span class="sxs-lookup"><span data-stu-id="b8ec9-120">Double</span></span>         | <span data-ttu-id="b8ec9-p103">O denominador da fração do tempo de exposição da câmera. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b8ec9-p103">The denominator for the exposure time fraction from the camera. Read-only.</span></span> |
|<span data-ttu-id="b8ec9-123">exposureNumerator</span><span class="sxs-lookup"><span data-stu-id="b8ec9-123">exposureNumerator</span></span>  |<span data-ttu-id="b8ec9-124">Duplo</span><span class="sxs-lookup"><span data-stu-id="b8ec9-124">Double</span></span>         | <span data-ttu-id="b8ec9-p104">O numerador da fração do tempo de exposição da câmera. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b8ec9-p104">The numerator for the exposure time fraction from the camera. Read-only.</span></span>   |
|<span data-ttu-id="b8ec9-127">fNumber</span><span class="sxs-lookup"><span data-stu-id="b8ec9-127">fNumber</span></span>            |<span data-ttu-id="b8ec9-128">Double</span><span class="sxs-lookup"><span data-stu-id="b8ec9-128">Double</span></span>         | <span data-ttu-id="b8ec9-p105">O valor de f-stop da câmera. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b8ec9-p105">The F-stop value from the camera. Read-only.</span></span>                               |
|<span data-ttu-id="b8ec9-131">focalLength</span><span class="sxs-lookup"><span data-stu-id="b8ec9-131">focalLength</span></span>        |<span data-ttu-id="b8ec9-132">Double</span><span class="sxs-lookup"><span data-stu-id="b8ec9-132">Double</span></span>         | <span data-ttu-id="b8ec9-p106">A distância focal da câmera. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b8ec9-p106">The focal length from the camera. Read-only.</span></span>                               |
|<span data-ttu-id="b8ec9-135">iso</span><span class="sxs-lookup"><span data-stu-id="b8ec9-135">iso</span></span>                |<span data-ttu-id="b8ec9-136">Int32</span><span class="sxs-lookup"><span data-stu-id="b8ec9-136">Int32</span></span>          | <span data-ttu-id="b8ec9-p107">O valor de ISO da câmera. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b8ec9-p107">The ISO value from the camera. Read-only.</span></span>                                  |
|<span data-ttu-id="b8ec9-139">orientation</span><span class="sxs-lookup"><span data-stu-id="b8ec9-139">orientation</span></span>        |<span data-ttu-id="b8ec9-140">Int16</span><span class="sxs-lookup"><span data-stu-id="b8ec9-140">Int16</span></span>          | <span data-ttu-id="b8ec9-141">O valor da orientação da câmera.</span><span class="sxs-lookup"><span data-stu-id="b8ec9-141">The orientation value from the camera.</span></span> <span data-ttu-id="b8ec9-142">Gravável no OneDrive Personal.</span><span class="sxs-lookup"><span data-stu-id="b8ec9-142">Writable on OneDrive Personal.</span></span>      |
|<span data-ttu-id="b8ec9-143">takenDateTime</span><span class="sxs-lookup"><span data-stu-id="b8ec9-143">takenDateTime</span></span>      |<span data-ttu-id="b8ec9-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b8ec9-144">DateTimeOffset</span></span> | <span data-ttu-id="b8ec9-145">A data e a hora em que a foto foi tirada no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="b8ec9-145">The date and time the photo was taken in UTC time.</span></span> <span data-ttu-id="b8ec9-146">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b8ec9-146">Read-only.</span></span>              |

## <a name="json-representation"></a><span data-ttu-id="b8ec9-147">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b8ec9-147">JSON representation</span></span>

<span data-ttu-id="b8ec9-148">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b8ec9-148">The following is a JSON representation of the resource.</span></span>

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


