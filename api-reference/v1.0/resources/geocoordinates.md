---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: GeoCoordinates
localization_priority: Normal
description: O recurso GeoCoordinates fornece as coordenadas geográficas e a elevação de um local com base nos metadados contidos no arquivo.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 64b81bc2946658ffc8617662879bc6cb20e25047
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029306"
---
# <a name="geocoordinates-resource-type"></a><span data-ttu-id="7388a-103">Tipo de recurso GeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="7388a-103">GeoCoordinates resource type</span></span>

<span data-ttu-id="7388a-p101">O recurso **GeoCoordinates** fornece as coordenadas geográficas e a elevação de um local com base nos metadados contidos no arquivo. Se um [**DriveItem**](driveitem.md) tiver uma faceta **location** não nula, o item representa um arquivo com um local conhecido associado a ele.</span><span class="sxs-lookup"><span data-stu-id="7388a-p101">The **GeoCoordinates** resource provides geographic coordinates and elevation of a location based on metadata contained within the file. If a [**DriveItem**](driveitem.md) has a non-null **location** facet, the item represents a file with a known location assocaited with it.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7388a-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7388a-106">JSON representation</span></span>

<span data-ttu-id="7388a-107">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="7388a-107">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.geoCoordinates"
}-->

```json
{
  "altitude": 1024.13,
  "latitude": 26.13246,
  "longitude": 24.34616
}
```

## <a name="properties"></a><span data-ttu-id="7388a-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7388a-108">Properties</span></span>

| <span data-ttu-id="7388a-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7388a-109">Property</span></span>  | <span data-ttu-id="7388a-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="7388a-110">Type</span></span>   | <span data-ttu-id="7388a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="7388a-111">Description</span></span>
|:----------|:-------|:--------------------------------------------------------
| <span data-ttu-id="7388a-112">altitude</span><span class="sxs-lookup"><span data-stu-id="7388a-112">altitude</span></span>  | <span data-ttu-id="7388a-113">Duplo</span><span class="sxs-lookup"><span data-stu-id="7388a-113">Double</span></span> | <span data-ttu-id="7388a-p102">Opcional. A altitude (altura), em pés, acima do nível do mar para o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7388a-p102">Optional. The altitude (height), in feet,  above sea level for the item. Read-only.</span></span>
| <span data-ttu-id="7388a-117">latitude</span><span class="sxs-lookup"><span data-stu-id="7388a-117">latitude</span></span>  | <span data-ttu-id="7388a-118">Duplo</span><span class="sxs-lookup"><span data-stu-id="7388a-118">Double</span></span> | <span data-ttu-id="7388a-p103">Opcional. A latitude, em valor decimal, para o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7388a-p103">Optional. The latitude, in decimal, for the item. Read-only.</span></span>
| <span data-ttu-id="7388a-122">longitude</span><span class="sxs-lookup"><span data-stu-id="7388a-122">longitude</span></span> | <span data-ttu-id="7388a-123">Double</span><span class="sxs-lookup"><span data-stu-id="7388a-123">Double</span></span> | <span data-ttu-id="7388a-p104">Opcional. A longitude, em valor decimal, para o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7388a-p104">Optional. The longitude, in decimal, for the item. Read-only.</span></span>

## <a name="remarks"></a><span data-ttu-id="7388a-127">Comentários</span><span class="sxs-lookup"><span data-stu-id="7388a-127">Remarks</span></span>

<span data-ttu-id="7388a-128">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="7388a-128">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The location facet provides geographic location related properties for an item",
  "keywords": "location,geographic,item,onedrive",
  "section": "documentation",
  "tocPath": "Facets/Location"
} -->
