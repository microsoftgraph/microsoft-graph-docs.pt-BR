---
author: JeremyKelley
description: O recurso geoCoordinates fornece coordenadas geográficas e elevação de um local com base nos metadados contidos no arquivo.
ms.date: 09/10/2017
title: GeoCoordinates
localization_priority: Normal
doc_type: resourcePageType
ms.prod: identity-and-access-reports
ms.openlocfilehash: e3b0ac4f616afe648b5c30dc9d15978036a7ab80
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50129419"
---
# <a name="geocoordinates-resource-type"></a><span data-ttu-id="5499b-103">Tipo de recurso geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="5499b-103">geoCoordinates resource type</span></span>

<span data-ttu-id="5499b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5499b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5499b-105">Fornece coordenadas geográficas e elevação de um local com base nos metadados contidos no arquivo.</span><span class="sxs-lookup"><span data-stu-id="5499b-105">Provides geographic coordinates and elevation of a location based on metadata contained within the file.</span></span>
<span data-ttu-id="5499b-106">Se um [**driveItem**](driveitem.md) tiver  uma faceta de local não nulo, o item representará um arquivo com um local conhecido com ele.</span><span class="sxs-lookup"><span data-stu-id="5499b-106">If a [**driveItem**](driveitem.md) has a non-null **location** facet, the item represents a file with a known location assocaited with it.</span></span>

> [!NOTE]
> <span data-ttu-id="5499b-107">Ao atualizar a latitude e a longitude de uma foto, um recurso [de](photo.md) foto (vazio ou não) deve ser fornecido.</span><span class="sxs-lookup"><span data-stu-id="5499b-107">When updating the latitude and longitude of a photo, a [photo](photo.md) resource (empty or otherwise) must be provided.</span></span>

## <a name="properties"></a><span data-ttu-id="5499b-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5499b-108">Properties</span></span>

| <span data-ttu-id="5499b-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5499b-109">Property</span></span>  | <span data-ttu-id="5499b-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="5499b-110">Type</span></span>   | <span data-ttu-id="5499b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="5499b-111">Description</span></span>
|:----------|:-------|:--------------------------------------------------------
| <span data-ttu-id="5499b-112">altitude</span><span class="sxs-lookup"><span data-stu-id="5499b-112">altitude</span></span>  | <span data-ttu-id="5499b-113">Double</span><span class="sxs-lookup"><span data-stu-id="5499b-113">Double</span></span> | <span data-ttu-id="5499b-p102">Opcional. A altitude (altura), em pés, acima do nível do mar para o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5499b-p102">Optional. The altitude (height), in feet,  above sea level for the item. Read-only.</span></span>
| <span data-ttu-id="5499b-117">latitude</span><span class="sxs-lookup"><span data-stu-id="5499b-117">latitude</span></span>  | <span data-ttu-id="5499b-118">Double</span><span class="sxs-lookup"><span data-stu-id="5499b-118">Double</span></span> | <span data-ttu-id="5499b-119">Opcional.</span><span class="sxs-lookup"><span data-stu-id="5499b-119">Optional.</span></span> <span data-ttu-id="5499b-120">A latitude, em valor decimal, para o item.</span><span class="sxs-lookup"><span data-stu-id="5499b-120">The latitude, in decimal, for the item.</span></span> <span data-ttu-id="5499b-121">Writable no OneDrive Personal.</span><span class="sxs-lookup"><span data-stu-id="5499b-121">Writable on OneDrive Personal.</span></span>
| <span data-ttu-id="5499b-122">longitude</span><span class="sxs-lookup"><span data-stu-id="5499b-122">longitude</span></span> | <span data-ttu-id="5499b-123">Double</span><span class="sxs-lookup"><span data-stu-id="5499b-123">Double</span></span> | <span data-ttu-id="5499b-124">Opcional.</span><span class="sxs-lookup"><span data-stu-id="5499b-124">Optional.</span></span> <span data-ttu-id="5499b-125">A longitude, em valor decimal, para o item.</span><span class="sxs-lookup"><span data-stu-id="5499b-125">The longitude, in decimal, for the item.</span></span> <span data-ttu-id="5499b-126">Writable no OneDrive Personal.</span><span class="sxs-lookup"><span data-stu-id="5499b-126">Writable on OneDrive Personal.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5499b-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5499b-127">JSON representation</span></span>

<span data-ttu-id="5499b-128">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="5499b-128">Here is a JSON representation of the resource</span></span>

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


