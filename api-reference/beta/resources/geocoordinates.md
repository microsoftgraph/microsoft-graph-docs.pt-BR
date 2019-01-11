---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: GeoCoordinates
localization_priority: Normal
ms.openlocfilehash: d49142ed414ad82ec149792e11e5a8c42d9837dc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27852637"
---
# <a name="geocoordinates-resource-type"></a><span data-ttu-id="78163-102">Tipo de recurso GeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="78163-102">GeoCoordinates resource type</span></span>

> <span data-ttu-id="78163-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="78163-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="78163-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="78163-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="78163-p102">O recurso **GeoCoordinates** fornece as coordenadas geográficas e a elevação de um local com base nos metadados contidos no arquivo. Se um [**DriveItem**](driveitem.md) tiver uma faceta **location** não nula, o item representa um arquivo com um local conhecido associado a ele.</span><span class="sxs-lookup"><span data-stu-id="78163-p102">The **GeoCoordinates** resource provides geographic coordinates and elevation of a location based on metadata contained within the file. If a [**DriveItem**](driveitem.md) has a non-null **location** facet, the item represents a file with a known location assocaited with it.</span></span>

## <a name="json-representation"></a><span data-ttu-id="78163-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="78163-107">JSON representation</span></span>

<span data-ttu-id="78163-108">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="78163-108">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="78163-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="78163-109">Properties</span></span>

| <span data-ttu-id="78163-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="78163-110">Property</span></span>  | <span data-ttu-id="78163-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="78163-111">Type</span></span>   | <span data-ttu-id="78163-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="78163-112">Description</span></span>
|:----------|:-------|:--------------------------------------------------------
| <span data-ttu-id="78163-113">altitude</span><span class="sxs-lookup"><span data-stu-id="78163-113">altitude</span></span>  | <span data-ttu-id="78163-114">Double</span><span class="sxs-lookup"><span data-stu-id="78163-114">Double</span></span> | <span data-ttu-id="78163-p103">Opcional. A altitude (altura), em pés, acima do nível do mar para o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="78163-p103">Optional. The altitude (height), in feet,  above sea level for the item. Read-only.</span></span>
| <span data-ttu-id="78163-118">latitude</span><span class="sxs-lookup"><span data-stu-id="78163-118">latitude</span></span>  | <span data-ttu-id="78163-119">Double</span><span class="sxs-lookup"><span data-stu-id="78163-119">Double</span></span> | <span data-ttu-id="78163-p104">Opcional. A latitude, em valor decimal, para o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="78163-p104">Optional. The latitude, in decimal, for the item. Read-only.</span></span>
| <span data-ttu-id="78163-123">longitude</span><span class="sxs-lookup"><span data-stu-id="78163-123">longitude</span></span> | <span data-ttu-id="78163-124">Double</span><span class="sxs-lookup"><span data-stu-id="78163-124">Double</span></span> | <span data-ttu-id="78163-p105">Opcional. A longitude, em valor decimal, para o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="78163-p105">Optional. The longitude, in decimal, for the item. Read-only.</span></span>

## <a name="remarks"></a><span data-ttu-id="78163-128">Comentários</span><span class="sxs-lookup"><span data-stu-id="78163-128">Remarks</span></span>

<span data-ttu-id="78163-129">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="78163-129">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The location facet provides geographic location related properties for an item",
  "keywords": "location,geographic,item,onedrive",
  "section": "documentation",
  "tocPath": "Facets/Location"
} -->
