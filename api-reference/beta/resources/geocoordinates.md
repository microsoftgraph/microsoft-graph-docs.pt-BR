---
author: JeremyKelley
description: O recurso GeoCoordinates fornece coordenadas geográficas e a elevação de um local com base nos metadados contidos no arquivo.
ms.date: 09/10/2017
title: GeoCoordinates
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 07b0a39155b8c9c4dc02d6cff1e0a93c1a9cd418
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42497633"
---
# <a name="geocoordinates-resource-type"></a><span data-ttu-id="9b79f-103">tipo de recurso GeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="9b79f-103">geoCoordinates resource type</span></span>

<span data-ttu-id="9b79f-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="9b79f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9b79f-105">Fornece coordenadas geográficas e a elevação de um local com base nos metadados contidos no arquivo.</span><span class="sxs-lookup"><span data-stu-id="9b79f-105">Provides geographic coordinates and elevation of a location based on metadata contained within the file.</span></span>
<span data-ttu-id="9b79f-106">Se um [**driveItem**](driveitem.md) tiver uma faceta de **local** não nula, o item representará um arquivo com um local conhecido associada com ele.</span><span class="sxs-lookup"><span data-stu-id="9b79f-106">If a [**driveItem**](driveitem.md) has a non-null **location** facet, the item represents a file with a known location assocaited with it.</span></span>

> [!NOTE]
> <span data-ttu-id="9b79f-107">Ao atualizar a latitude e a longitude de uma foto, um recurso de [foto](photo.md) (vazio ou ou outro) deve ser fornecido.</span><span class="sxs-lookup"><span data-stu-id="9b79f-107">When updating the latitude and longitude of a photo, a [photo](photo.md) resource (empty or otherwise) must be provided.</span></span>

## <a name="properties"></a><span data-ttu-id="9b79f-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9b79f-108">Properties</span></span>

| <span data-ttu-id="9b79f-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9b79f-109">Property</span></span>  | <span data-ttu-id="9b79f-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="9b79f-110">Type</span></span>   | <span data-ttu-id="9b79f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="9b79f-111">Description</span></span>
|:----------|:-------|:--------------------------------------------------------
| <span data-ttu-id="9b79f-112">altitude</span><span class="sxs-lookup"><span data-stu-id="9b79f-112">altitude</span></span>  | <span data-ttu-id="9b79f-113">Duplo</span><span class="sxs-lookup"><span data-stu-id="9b79f-113">Double</span></span> | <span data-ttu-id="9b79f-p102">Opcional. A altitude (altura), em pés, acima do nível do mar para o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9b79f-p102">Optional. The altitude (height), in feet,  above sea level for the item. Read-only.</span></span>
| <span data-ttu-id="9b79f-117">latitude</span><span class="sxs-lookup"><span data-stu-id="9b79f-117">latitude</span></span>  | <span data-ttu-id="9b79f-118">Double</span><span class="sxs-lookup"><span data-stu-id="9b79f-118">Double</span></span> | <span data-ttu-id="9b79f-119">Opcional.</span><span class="sxs-lookup"><span data-stu-id="9b79f-119">Optional.</span></span> <span data-ttu-id="9b79f-120">A latitude, em valor decimal, para o item.</span><span class="sxs-lookup"><span data-stu-id="9b79f-120">The latitude, in decimal, for the item.</span></span> <span data-ttu-id="9b79f-121">Gravável no OneDrive Personal.</span><span class="sxs-lookup"><span data-stu-id="9b79f-121">Writable on OneDrive Personal.</span></span>
| <span data-ttu-id="9b79f-122">longitude</span><span class="sxs-lookup"><span data-stu-id="9b79f-122">longitude</span></span> | <span data-ttu-id="9b79f-123">Double</span><span class="sxs-lookup"><span data-stu-id="9b79f-123">Double</span></span> | <span data-ttu-id="9b79f-124">Opcional.</span><span class="sxs-lookup"><span data-stu-id="9b79f-124">Optional.</span></span> <span data-ttu-id="9b79f-125">A longitude, em valor decimal, para o item.</span><span class="sxs-lookup"><span data-stu-id="9b79f-125">The longitude, in decimal, for the item.</span></span> <span data-ttu-id="9b79f-126">Gravável no OneDrive Personal.</span><span class="sxs-lookup"><span data-stu-id="9b79f-126">Writable on OneDrive Personal.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9b79f-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9b79f-127">JSON representation</span></span>

<span data-ttu-id="9b79f-128">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="9b79f-128">Here is a JSON representation of the resource</span></span>

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
