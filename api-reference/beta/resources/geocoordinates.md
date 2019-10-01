---
author: JeremyKelley
description: O recurso GeoCoordinates fornece coordenadas geográficas e a elevação de um local com base nos metadados contidos no arquivo.
ms.date: 09/10/2017
title: GeoCoordinates
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 86de97358591df8dc446b91d0be7a8192c7346f8
ms.sourcegitcommit: 2fb178ae78b5ecc47207d2b19d0c5a46e07e0960
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/01/2019
ms.locfileid: "37333250"
---
# <a name="geocoordinates-resource-type"></a><span data-ttu-id="29691-103">tipo de recurso GeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="29691-103">geoCoordinates resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="29691-104">Fornece coordenadas geográficas e a elevação de um local com base nos metadados contidos no arquivo.</span><span class="sxs-lookup"><span data-stu-id="29691-104">Provides geographic coordinates and elevation of a location based on metadata contained within the file.</span></span>
<span data-ttu-id="29691-105">Se um [**driveItem**](driveitem.md) tiver uma faceta de **local** não nula, o item representará um arquivo com um local conhecido associada com ele.</span><span class="sxs-lookup"><span data-stu-id="29691-105">If a [**driveItem**](driveitem.md) has a non-null **location** facet, the item represents a file with a known location assocaited with it.</span></span>

> [!NOTE]
> <span data-ttu-id="29691-106">Ao atualizar a latitude e a longitude de uma foto, um recurso de [foto](photo.md) (vazio ou ou outro) deve ser fornecido.</span><span class="sxs-lookup"><span data-stu-id="29691-106">When updating the latitude and longitude of a photo, a [photo](photo.md) resource (empty or otherwise) must be provided.</span></span>

## <a name="properties"></a><span data-ttu-id="29691-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="29691-107">Properties</span></span>

| <span data-ttu-id="29691-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="29691-108">Property</span></span>  | <span data-ttu-id="29691-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="29691-109">Type</span></span>   | <span data-ttu-id="29691-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="29691-110">Description</span></span>
|:----------|:-------|:--------------------------------------------------------
| <span data-ttu-id="29691-111">altitude</span><span class="sxs-lookup"><span data-stu-id="29691-111">altitude</span></span>  | <span data-ttu-id="29691-112">Duplo</span><span class="sxs-lookup"><span data-stu-id="29691-112">Double</span></span> | <span data-ttu-id="29691-p102">Opcional. A altitude (altura), em pés, acima do nível do mar para o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="29691-p102">Optional. The altitude (height), in feet,  above sea level for the item. Read-only.</span></span>
| <span data-ttu-id="29691-116">latitude</span><span class="sxs-lookup"><span data-stu-id="29691-116">latitude</span></span>  | <span data-ttu-id="29691-117">Double</span><span class="sxs-lookup"><span data-stu-id="29691-117">Double</span></span> | <span data-ttu-id="29691-118">Opcional.</span><span class="sxs-lookup"><span data-stu-id="29691-118">Optional.</span></span> <span data-ttu-id="29691-119">A latitude, em valor decimal, para o item.</span><span class="sxs-lookup"><span data-stu-id="29691-119">The latitude, in decimal, for the item.</span></span> <span data-ttu-id="29691-120">Gravável no OneDrive Personal.</span><span class="sxs-lookup"><span data-stu-id="29691-120">Writable on OneDrive Personal.</span></span>
| <span data-ttu-id="29691-121">longitude</span><span class="sxs-lookup"><span data-stu-id="29691-121">longitude</span></span> | <span data-ttu-id="29691-122">Double</span><span class="sxs-lookup"><span data-stu-id="29691-122">Double</span></span> | <span data-ttu-id="29691-123">Opcional.</span><span class="sxs-lookup"><span data-stu-id="29691-123">Optional.</span></span> <span data-ttu-id="29691-124">A longitude, em valor decimal, para o item.</span><span class="sxs-lookup"><span data-stu-id="29691-124">The longitude, in decimal, for the item.</span></span> <span data-ttu-id="29691-125">Gravável no OneDrive Personal.</span><span class="sxs-lookup"><span data-stu-id="29691-125">Writable on OneDrive Personal.</span></span>

## <a name="json-representation"></a><span data-ttu-id="29691-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="29691-126">JSON representation</span></span>

<span data-ttu-id="29691-127">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="29691-127">Here is a JSON representation of the resource</span></span>

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
