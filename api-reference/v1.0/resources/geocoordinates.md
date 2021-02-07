---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: GeoCoordinates
localization_priority: Normal
description: O recurso GeoCoordinates fornece as coordenadas geográficas e a elevação de um local com base nos metadados contidos no arquivo.
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 048fefc8938a789a0aae06f3dd6f50c25c305c31
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50130505"
---
# <a name="geocoordinates-resource-type"></a><span data-ttu-id="66633-103">Tipo de recurso GeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="66633-103">GeoCoordinates resource type</span></span>

<span data-ttu-id="66633-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="66633-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="66633-p101">O recurso **GeoCoordinates** fornece as coordenadas geográficas e a elevação de um local com base nos metadados contidos no arquivo. Se um [**DriveItem**](driveitem.md) tiver uma faceta **location** não nula, o item representa um arquivo com um local conhecido associado a ele.</span><span class="sxs-lookup"><span data-stu-id="66633-p101">The **GeoCoordinates** resource provides geographic coordinates and elevation of a location based on metadata contained within the file. If a [**DriveItem**](driveitem.md) has a non-null **location** facet, the item represents a file with a known location assocaited with it.</span></span>

## <a name="json-representation"></a><span data-ttu-id="66633-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="66633-107">JSON representation</span></span>

<span data-ttu-id="66633-108">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="66633-108">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="66633-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="66633-109">Properties</span></span>

| <span data-ttu-id="66633-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="66633-110">Property</span></span>  | <span data-ttu-id="66633-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="66633-111">Type</span></span>   | <span data-ttu-id="66633-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="66633-112">Description</span></span>
|:----------|:-------|:--------------------------------------------------------
| <span data-ttu-id="66633-113">altitude</span><span class="sxs-lookup"><span data-stu-id="66633-113">altitude</span></span>  | <span data-ttu-id="66633-114">Double</span><span class="sxs-lookup"><span data-stu-id="66633-114">Double</span></span> | <span data-ttu-id="66633-p102">Opcional. A altitude (altura), em pés, acima do nível do mar para o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="66633-p102">Optional. The altitude (height), in feet,  above sea level for the item. Read-only.</span></span>
| <span data-ttu-id="66633-118">latitude</span><span class="sxs-lookup"><span data-stu-id="66633-118">latitude</span></span>  | <span data-ttu-id="66633-119">Double</span><span class="sxs-lookup"><span data-stu-id="66633-119">Double</span></span> | <span data-ttu-id="66633-p103">Opcional. A latitude, em valor decimal, para o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="66633-p103">Optional. The latitude, in decimal, for the item. Read-only.</span></span>
| <span data-ttu-id="66633-123">longitude</span><span class="sxs-lookup"><span data-stu-id="66633-123">longitude</span></span> | <span data-ttu-id="66633-124">Double</span><span class="sxs-lookup"><span data-stu-id="66633-124">Double</span></span> | <span data-ttu-id="66633-p104">Opcional. A longitude, em valor decimal, para o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="66633-p104">Optional. The longitude, in decimal, for the item. Read-only.</span></span>

## <a name="remarks"></a><span data-ttu-id="66633-128">Comentários</span><span class="sxs-lookup"><span data-stu-id="66633-128">Remarks</span></span>

<span data-ttu-id="66633-129">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="66633-129">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The location facet provides geographic location related properties for an item",
  "keywords": "location,geographic,item,onedrive",
  "section": "documentation",
  "tocPath": "Facets/Location"
} -->

