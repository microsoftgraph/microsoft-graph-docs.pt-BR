---
author: JeremyKelley
description: O recurso GeoCoordinates fornece as coordenadas geográficas e a elevação de um local com base nos metadados contidos no arquivo.
ms.date: 09/10/2017
title: GeoCoordinates
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 98f9c09c4604311c0cc741028565be860eb996ef
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35971943"
---
# <a name="geocoordinates-resource-type"></a><span data-ttu-id="7b5f4-103">Tipo de recurso GeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="7b5f4-103">GeoCoordinates resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7b5f4-p101">O recurso **GeoCoordinates** fornece as coordenadas geográficas e a elevação de um local com base nos metadados contidos no arquivo. Se um [**DriveItem**](driveitem.md) tiver uma faceta **location** não nula, o item representa um arquivo com um local conhecido associado a ele.</span><span class="sxs-lookup"><span data-stu-id="7b5f4-p101">The **GeoCoordinates** resource provides geographic coordinates and elevation of a location based on metadata contained within the file. If a [**DriveItem**](driveitem.md) has a non-null **location** facet, the item represents a file with a known location assocaited with it.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7b5f4-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7b5f4-106">JSON representation</span></span>

<span data-ttu-id="7b5f4-107">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="7b5f4-107">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="7b5f4-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7b5f4-108">Properties</span></span>

| <span data-ttu-id="7b5f4-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7b5f4-109">Property</span></span>  | <span data-ttu-id="7b5f4-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="7b5f4-110">Type</span></span>   | <span data-ttu-id="7b5f4-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="7b5f4-111">Description</span></span>
|:----------|:-------|:--------------------------------------------------------
| <span data-ttu-id="7b5f4-112">altitude</span><span class="sxs-lookup"><span data-stu-id="7b5f4-112">altitude</span></span>  | <span data-ttu-id="7b5f4-113">Duplo</span><span class="sxs-lookup"><span data-stu-id="7b5f4-113">Double</span></span> | <span data-ttu-id="7b5f4-p102">Opcional. A altitude (altura), em pés, acima do nível do mar para o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7b5f4-p102">Optional. The altitude (height), in feet,  above sea level for the item. Read-only.</span></span>
| <span data-ttu-id="7b5f4-117">latitude</span><span class="sxs-lookup"><span data-stu-id="7b5f4-117">latitude</span></span>  | <span data-ttu-id="7b5f4-118">Duplo</span><span class="sxs-lookup"><span data-stu-id="7b5f4-118">Double</span></span> | <span data-ttu-id="7b5f4-p103">Opcional. A latitude, em valor decimal, para o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7b5f4-p103">Optional. The latitude, in decimal, for the item. Read-only.</span></span>
| <span data-ttu-id="7b5f4-122">longitude</span><span class="sxs-lookup"><span data-stu-id="7b5f4-122">longitude</span></span> | <span data-ttu-id="7b5f4-123">Double</span><span class="sxs-lookup"><span data-stu-id="7b5f4-123">Double</span></span> | <span data-ttu-id="7b5f4-p104">Opcional. A longitude, em valor decimal, para o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7b5f4-p104">Optional. The longitude, in decimal, for the item. Read-only.</span></span>

## <a name="remarks"></a><span data-ttu-id="7b5f4-127">Comentários</span><span class="sxs-lookup"><span data-stu-id="7b5f4-127">Remarks</span></span>

<span data-ttu-id="7b5f4-128">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="7b5f4-128">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The location facet provides geographic location related properties for an item",
  "keywords": "location,geographic,item,onedrive",
  "section": "documentation",
  "tocPath": "Facets/Location",
  "suppressions": []
}
-->
