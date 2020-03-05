---
title: Tipo de recurso outlookGeoCoordinates
description: As coordenadas geográficas, a elevação e o grau de precisão delas para um local físico.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 1926d398a07bb38f27f46b8886ba7454321d5796
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447266"
---
# <a name="outlookgeocoordinates-resource-type"></a><span data-ttu-id="3fbc1-103">Tipo de recurso outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="3fbc1-103">outlookGeoCoordinates resource type</span></span>

<span data-ttu-id="3fbc1-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="3fbc1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3fbc1-105">As coordenadas geográficas, a elevação e o grau de precisão delas para um local físico.</span><span class="sxs-lookup"><span data-stu-id="3fbc1-105">The geographic coordinates, elevation, and their degree of accuracy for a physical location.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3fbc1-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3fbc1-106">JSON representation</span></span>

<span data-ttu-id="3fbc1-107">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3fbc1-107">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="3fbc1-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3fbc1-108">Properties</span></span>
| <span data-ttu-id="3fbc1-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3fbc1-109">Property</span></span>     | <span data-ttu-id="3fbc1-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="3fbc1-110">Type</span></span>   |<span data-ttu-id="3fbc1-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="3fbc1-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3fbc1-112">accuracy</span><span class="sxs-lookup"><span data-stu-id="3fbc1-112">accuracy</span></span>|<span data-ttu-id="3fbc1-113">double</span><span class="sxs-lookup"><span data-stu-id="3fbc1-113">double</span></span>|<span data-ttu-id="3fbc1-114">A precisão da latitude e da longitude.</span><span class="sxs-lookup"><span data-stu-id="3fbc1-114">The accuracy of the latitude and longitude.</span></span> <span data-ttu-id="3fbc1-115">Por exemplo, a precisão pode ser medida em metros, como a precisão da latitude e da longitude em um raio de 50 metros.</span><span class="sxs-lookup"><span data-stu-id="3fbc1-115">As an example, the accuracy can be measured in meters, such as the latitude and longitude are accurate to within 50 meters.</span></span>|
|<span data-ttu-id="3fbc1-116">altitude</span><span class="sxs-lookup"><span data-stu-id="3fbc1-116">altitude</span></span>|<span data-ttu-id="3fbc1-117">double</span><span class="sxs-lookup"><span data-stu-id="3fbc1-117">double</span></span>|<span data-ttu-id="3fbc1-118">A altitude do local.</span><span class="sxs-lookup"><span data-stu-id="3fbc1-118">The altitude of the location.</span></span>|
|<span data-ttu-id="3fbc1-119">altitudeAccuracy</span><span class="sxs-lookup"><span data-stu-id="3fbc1-119">altitudeAccuracy</span></span>|<span data-ttu-id="3fbc1-120">double</span><span class="sxs-lookup"><span data-stu-id="3fbc1-120">double</span></span>|<span data-ttu-id="3fbc1-121">A precisão da altitude.</span><span class="sxs-lookup"><span data-stu-id="3fbc1-121">The accuracy of the altitude.</span></span>|
|<span data-ttu-id="3fbc1-122">latitude</span><span class="sxs-lookup"><span data-stu-id="3fbc1-122">latitude</span></span>|<span data-ttu-id="3fbc1-123">double</span><span class="sxs-lookup"><span data-stu-id="3fbc1-123">double</span></span>|<span data-ttu-id="3fbc1-124">A latitude do local.</span><span class="sxs-lookup"><span data-stu-id="3fbc1-124">The latitude of the location.</span></span>|
|<span data-ttu-id="3fbc1-125">longitude</span><span class="sxs-lookup"><span data-stu-id="3fbc1-125">longitude</span></span>|<span data-ttu-id="3fbc1-126">double</span><span class="sxs-lookup"><span data-stu-id="3fbc1-126">double</span></span>|<span data-ttu-id="3fbc1-127">A longitude do local.</span><span class="sxs-lookup"><span data-stu-id="3fbc1-127">The longitude of the location.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookGeoCoordinates resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
