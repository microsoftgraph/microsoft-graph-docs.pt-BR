---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: GeoCoordinates
localization_priority: Normal
ms.openlocfilehash: 33390fa893e99ffb0d7c44642c42751c66265ec8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27885509"
---
# <a name="geocoordinates-resource-type"></a><span data-ttu-id="49bdf-102">Tipo de recurso GeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="49bdf-102">GeoCoordinates resource type</span></span>

<span data-ttu-id="49bdf-p101">O recurso **GeoCoordinates** fornece as coordenadas geográficas e a elevação de um local com base nos metadados contidos no arquivo. Se um [**DriveItem**](driveitem.md) tiver uma faceta **location** não nula, o item representa um arquivo com um local conhecido associado a ele.</span><span class="sxs-lookup"><span data-stu-id="49bdf-p101">The **GeoCoordinates** resource provides geographic coordinates and elevation of a location based on metadata contained within the file. If a [**DriveItem**](driveitem.md) has a non-null **location** facet, the item represents a file with a known location assocaited with it.</span></span>

## <a name="json-representation"></a><span data-ttu-id="49bdf-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="49bdf-105">JSON representation</span></span>

<span data-ttu-id="49bdf-106">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="49bdf-106">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="49bdf-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="49bdf-107">Properties</span></span>

| <span data-ttu-id="49bdf-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="49bdf-108">Property</span></span>  | <span data-ttu-id="49bdf-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="49bdf-109">Type</span></span>   | <span data-ttu-id="49bdf-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="49bdf-110">Description</span></span>
|:----------|:-------|:--------------------------------------------------------
| <span data-ttu-id="49bdf-111">altitude</span><span class="sxs-lookup"><span data-stu-id="49bdf-111">altitude</span></span>  | <span data-ttu-id="49bdf-112">Double</span><span class="sxs-lookup"><span data-stu-id="49bdf-112">Double</span></span> | <span data-ttu-id="49bdf-p102">Opcional. A altitude (altura), em pés, acima do nível do mar para o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="49bdf-p102">Optional. The altitude (height), in feet,  above sea level for the item. Read-only.</span></span>
| <span data-ttu-id="49bdf-116">latitude</span><span class="sxs-lookup"><span data-stu-id="49bdf-116">latitude</span></span>  | <span data-ttu-id="49bdf-117">Double</span><span class="sxs-lookup"><span data-stu-id="49bdf-117">Double</span></span> | <span data-ttu-id="49bdf-p103">Opcional. A latitude, em valor decimal, para o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="49bdf-p103">Optional. The latitude, in decimal, for the item. Read-only.</span></span>
| <span data-ttu-id="49bdf-121">longitude</span><span class="sxs-lookup"><span data-stu-id="49bdf-121">longitude</span></span> | <span data-ttu-id="49bdf-122">Double</span><span class="sxs-lookup"><span data-stu-id="49bdf-122">Double</span></span> | <span data-ttu-id="49bdf-p104">Opcional. A longitude, em valor decimal, para o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="49bdf-p104">Optional. The longitude, in decimal, for the item. Read-only.</span></span>

## <a name="remarks"></a><span data-ttu-id="49bdf-126">Comentários</span><span class="sxs-lookup"><span data-stu-id="49bdf-126">Remarks</span></span>

<span data-ttu-id="49bdf-127">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="49bdf-127">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The location facet provides geographic location related properties for an item",
  "keywords": "location,geographic,item,onedrive",
  "section": "documentation",
  "tocPath": "Facets/Location"
} -->
