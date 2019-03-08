---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: GeoCoordinates
localization_priority: Normal
ms.openlocfilehash: 221037578e055e5bb57987058a190bc3026b3e0c
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2019
ms.locfileid: "30482354"
---
# <a name="geocoordinates-resource-type"></a><span data-ttu-id="8f774-102">Tipo de recurso GeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="8f774-102">GeoCoordinates resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8f774-p101">O recurso **GeoCoordinates** fornece as coordenadas geográficas e a elevação de um local com base nos metadados contidos no arquivo. Se um [**DriveItem**](driveitem.md) tiver uma faceta **location** não nula, o item representa um arquivo com um local conhecido associado a ele.</span><span class="sxs-lookup"><span data-stu-id="8f774-p101">The **GeoCoordinates** resource provides geographic coordinates and elevation of a location based on metadata contained within the file. If a [**DriveItem**](driveitem.md) has a non-null **location** facet, the item represents a file with a known location assocaited with it.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8f774-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8f774-105">JSON representation</span></span>

<span data-ttu-id="8f774-106">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="8f774-106">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="8f774-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8f774-107">Properties</span></span>

| <span data-ttu-id="8f774-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8f774-108">Property</span></span>  | <span data-ttu-id="8f774-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="8f774-109">Type</span></span>   | <span data-ttu-id="8f774-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="8f774-110">Description</span></span>
|:----------|:-------|:--------------------------------------------------------
| <span data-ttu-id="8f774-111">altitude</span><span class="sxs-lookup"><span data-stu-id="8f774-111">altitude</span></span>  | <span data-ttu-id="8f774-112">Duplo</span><span class="sxs-lookup"><span data-stu-id="8f774-112">Double</span></span> | <span data-ttu-id="8f774-p102">Opcional. A altitude (altura), em pés, acima do nível do mar para o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8f774-p102">Optional. The altitude (height), in feet,  above sea level for the item. Read-only.</span></span>
| <span data-ttu-id="8f774-116">latitude</span><span class="sxs-lookup"><span data-stu-id="8f774-116">latitude</span></span>  | <span data-ttu-id="8f774-117">Duplo</span><span class="sxs-lookup"><span data-stu-id="8f774-117">Double</span></span> | <span data-ttu-id="8f774-p103">Opcional. A latitude, em valor decimal, para o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8f774-p103">Optional. The latitude, in decimal, for the item. Read-only.</span></span>
| <span data-ttu-id="8f774-121">longitude</span><span class="sxs-lookup"><span data-stu-id="8f774-121">longitude</span></span> | <span data-ttu-id="8f774-122">Double</span><span class="sxs-lookup"><span data-stu-id="8f774-122">Double</span></span> | <span data-ttu-id="8f774-p104">Opcional. A longitude, em valor decimal, para o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8f774-p104">Optional. The longitude, in decimal, for the item. Read-only.</span></span>

## <a name="remarks"></a><span data-ttu-id="8f774-126">Comentários</span><span class="sxs-lookup"><span data-stu-id="8f774-126">Remarks</span></span>

<span data-ttu-id="8f774-127">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="8f774-127">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The location facet provides geographic location related properties for an item",
  "keywords": "location,geographic,item,onedrive",
  "section": "documentation",
  "tocPath": "Facets/Location",
  "suppressions": [
    "Error: /api-reference/beta/resources/geocoordinates.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
