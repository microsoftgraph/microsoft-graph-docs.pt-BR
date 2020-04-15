---
title: Tipo de recurso outlookGeoCoordinates
description: As coordenadas geográficas, a elevação e o grau de precisão delas para um local físico.
localization_priority: Normal
author: harini84
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: ae101814d7e32be67ae7becc6e2032ff4e2026d2
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43353846"
---
# <a name="outlookgeocoordinates-resource-type"></a><span data-ttu-id="2598a-103">Tipo de recurso outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="2598a-103">outlookGeoCoordinates resource type</span></span>

<span data-ttu-id="2598a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2598a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2598a-105">As coordenadas geográficas, a elevação e o grau de precisão delas para um local físico.</span><span class="sxs-lookup"><span data-stu-id="2598a-105">The geographic coordinates, elevation, and their degree of accuracy for a physical location.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2598a-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2598a-106">JSON representation</span></span>

<span data-ttu-id="2598a-107">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2598a-107">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.outlookGeoCoordinates"
}-->

```json
{
  "accuracy": 1024.13,
  "altitude": 1024.13,
  "altitudeAccuracy": 1024.13,
  "latitude": 1024.13,
  "longitude": 1024.13
}

```
## <a name="properties"></a><span data-ttu-id="2598a-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2598a-108">Properties</span></span>
| <span data-ttu-id="2598a-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2598a-109">Property</span></span>     | <span data-ttu-id="2598a-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="2598a-110">Type</span></span>   |<span data-ttu-id="2598a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="2598a-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2598a-112">accuracy</span><span class="sxs-lookup"><span data-stu-id="2598a-112">accuracy</span></span>|<span data-ttu-id="2598a-113">double</span><span class="sxs-lookup"><span data-stu-id="2598a-113">double</span></span>|<span data-ttu-id="2598a-114">A precisão da latitude e da longitude.</span><span class="sxs-lookup"><span data-stu-id="2598a-114">The accuracy of the latitude and longitude.</span></span> <span data-ttu-id="2598a-115">Por exemplo, a precisão pode ser medida em metros, como a precisão da latitude e da longitude em um raio de 50 metros.</span><span class="sxs-lookup"><span data-stu-id="2598a-115">As an example, the accuracy can be measured in meters, such as the latitude and longitude are accurate to within 50 meters.</span></span>|
|<span data-ttu-id="2598a-116">altitude</span><span class="sxs-lookup"><span data-stu-id="2598a-116">altitude</span></span>|<span data-ttu-id="2598a-117">double</span><span class="sxs-lookup"><span data-stu-id="2598a-117">double</span></span>|<span data-ttu-id="2598a-118">A altitude do local.</span><span class="sxs-lookup"><span data-stu-id="2598a-118">The altitude of the location.</span></span>|
|<span data-ttu-id="2598a-119">altitudeAccuracy</span><span class="sxs-lookup"><span data-stu-id="2598a-119">altitudeAccuracy</span></span>|<span data-ttu-id="2598a-120">double</span><span class="sxs-lookup"><span data-stu-id="2598a-120">double</span></span>|<span data-ttu-id="2598a-121">A precisão da altitude.</span><span class="sxs-lookup"><span data-stu-id="2598a-121">The accuracy of the altitude.</span></span>|
|<span data-ttu-id="2598a-122">latitude</span><span class="sxs-lookup"><span data-stu-id="2598a-122">latitude</span></span>|<span data-ttu-id="2598a-123">double</span><span class="sxs-lookup"><span data-stu-id="2598a-123">double</span></span>|<span data-ttu-id="2598a-124">A latitude do local.</span><span class="sxs-lookup"><span data-stu-id="2598a-124">The latitude of the location.</span></span>|
|<span data-ttu-id="2598a-125">longitude</span><span class="sxs-lookup"><span data-stu-id="2598a-125">longitude</span></span>|<span data-ttu-id="2598a-126">double</span><span class="sxs-lookup"><span data-stu-id="2598a-126">double</span></span>|<span data-ttu-id="2598a-127">A longitude do local.</span><span class="sxs-lookup"><span data-stu-id="2598a-127">The longitude of the location.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookGeoCoordinates resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
