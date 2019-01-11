---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Foto
localization_priority: Normal
ms.openlocfilehash: ed891f917ba8018aac349976df0455adfd269fdb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27869377"
---
# <a name="photo-resource-type"></a><span data-ttu-id="56aa8-102">Tipo de recurso Photo</span><span class="sxs-lookup"><span data-stu-id="56aa8-102">Photo resource type</span></span>

> <span data-ttu-id="56aa8-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="56aa8-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="56aa8-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="56aa8-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="56aa8-105">O recurso **photo** fornece propriedades de foto e câmera, por exemplo, metadados EXIF, em um [driveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="56aa8-105">The **photo** resource provides photo and camera properties, for example, EXIF metadata, on a [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="56aa8-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="56aa8-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="56aa8-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="56aa8-107">Properties</span></span>

| <span data-ttu-id="56aa8-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="56aa8-108">Property</span></span>                | <span data-ttu-id="56aa8-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="56aa8-109">Type</span></span>           | <span data-ttu-id="56aa8-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="56aa8-110">Description</span></span>
|:------------------------|:---------------|:----------------------------------
| <span data-ttu-id="56aa8-111">**takenDateTime**</span><span class="sxs-lookup"><span data-stu-id="56aa8-111">**takenDateTime**</span></span>       | <span data-ttu-id="56aa8-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="56aa8-112">DateTimeOffset</span></span> | <span data-ttu-id="56aa8-p102">Representa a data e a hora em que a foto foi tirada. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="56aa8-p102">Represents the date and time the photo was taken. Read-only.</span></span>
| <span data-ttu-id="56aa8-115">**cameraMake**</span><span class="sxs-lookup"><span data-stu-id="56aa8-115">**cameraMake**</span></span>          | <span data-ttu-id="56aa8-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="56aa8-116">String</span></span>         | <span data-ttu-id="56aa8-p103">Fabricante da câmera. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="56aa8-p103">Camera manufacturer. Read-only.</span></span>
| <span data-ttu-id="56aa8-119">**cameraModel**</span><span class="sxs-lookup"><span data-stu-id="56aa8-119">**cameraModel**</span></span>         | <span data-ttu-id="56aa8-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="56aa8-120">String</span></span>         | <span data-ttu-id="56aa8-p104">Modelo da câmera. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="56aa8-p104">Camera model. Read-only.</span></span>
| <span data-ttu-id="56aa8-123">**fNumber**</span><span class="sxs-lookup"><span data-stu-id="56aa8-123">**fNumber**</span></span>             | <span data-ttu-id="56aa8-124">Double</span><span class="sxs-lookup"><span data-stu-id="56aa8-124">Double</span></span>         | <span data-ttu-id="56aa8-p105">O valor de f-stop da câmera. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="56aa8-p105">The F-stop value from the camera. Read-only.</span></span>
| <span data-ttu-id="56aa8-127">**exposureDenominator**</span><span class="sxs-lookup"><span data-stu-id="56aa8-127">**exposureDenominator**</span></span> | <span data-ttu-id="56aa8-128">Duplo</span><span class="sxs-lookup"><span data-stu-id="56aa8-128">Double</span></span>         | <span data-ttu-id="56aa8-p106">O denominador da fração do tempo de exposição da câmera. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="56aa8-p106">The denominator for the exposure time fraction from the camera. Read-only.</span></span>
| <span data-ttu-id="56aa8-131">**exposureNumerator**</span><span class="sxs-lookup"><span data-stu-id="56aa8-131">**exposureNumerator**</span></span>   | <span data-ttu-id="56aa8-132">Duplo</span><span class="sxs-lookup"><span data-stu-id="56aa8-132">Double</span></span>         | <span data-ttu-id="56aa8-p107">O numerador da fração do tempo de exposição da câmera. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="56aa8-p107">The numerator for the exposure time fraction from the camera. Read-only.</span></span>
| <span data-ttu-id="56aa8-135">**focalLength**</span><span class="sxs-lookup"><span data-stu-id="56aa8-135">**focalLength**</span></span>         | <span data-ttu-id="56aa8-136">Double</span><span class="sxs-lookup"><span data-stu-id="56aa8-136">Double</span></span>         | <span data-ttu-id="56aa8-p108">A distância focal da câmera. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="56aa8-p108">The focal length from the camera. Read-only.</span></span>
| <span data-ttu-id="56aa8-139">**iso**</span><span class="sxs-lookup"><span data-stu-id="56aa8-139">**iso**</span></span>                 | <span data-ttu-id="56aa8-140">Int64</span><span class="sxs-lookup"><span data-stu-id="56aa8-140">Int64</span></span>          | <span data-ttu-id="56aa8-p109">O valor de ISO da câmera. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="56aa8-p109">The ISO value from the camera. Read-only.</span></span>

## <a name="remarks"></a><span data-ttu-id="56aa8-143">Comentários</span><span class="sxs-lookup"><span data-stu-id="56aa8-143">Remarks</span></span>
<span data-ttu-id="56aa8-144">O OneDrive for Business e o SharePoint retornam apenas a propriedade **takenDateTime**.</span><span class="sxs-lookup"><span data-stu-id="56aa8-144">OneDrive for Business and SharePoint only return the **takenDateTime** property.</span></span>

<span data-ttu-id="56aa8-145">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="56aa8-145">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>
<!-- {
  "type": "#page.annotation",
  "description": "The photo facet provides details about the camera and settings on the camera for photos.",
  "keywords": "camera make,camera model, exposure, f-stop, iso",
  "section": "documentation",
  "tocPath": "Facets/Photo"
} -->
