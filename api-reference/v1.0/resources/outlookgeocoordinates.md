---
title: Tipo de recurso outlookGeoCoordinates
description: As coordenadas geográficas, a elevação e o grau de precisão delas para um local físico.
localization_priority: Normal
ms.openlocfilehash: b6c3c8d6336cd301caba0def2853f498f488816b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27837426"
---
# <a name="outlookgeocoordinates-resource-type"></a><span data-ttu-id="ed971-103">Tipo de recurso outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="ed971-103">outlookGeoCoordinates resource type</span></span>

<span data-ttu-id="ed971-104">As coordenadas geográficas, a elevação e o grau de precisão delas para um local físico.</span><span class="sxs-lookup"><span data-stu-id="ed971-104">The geographic coordinates, elevation, and their degree of accuracy for a physical location.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ed971-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ed971-105">JSON representation</span></span>

<span data-ttu-id="ed971-106">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ed971-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="ed971-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ed971-107">Properties</span></span>
| <span data-ttu-id="ed971-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ed971-108">Property</span></span>     | <span data-ttu-id="ed971-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="ed971-109">Type</span></span>   |<span data-ttu-id="ed971-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="ed971-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ed971-111">accuracy</span><span class="sxs-lookup"><span data-stu-id="ed971-111">accuracy</span></span>|<span data-ttu-id="ed971-112">double</span><span class="sxs-lookup"><span data-stu-id="ed971-112">double</span></span>|<span data-ttu-id="ed971-113">A precisão da latitude e da longitude.</span><span class="sxs-lookup"><span data-stu-id="ed971-113">The accuracy of the latitude and longitude.</span></span> <span data-ttu-id="ed971-114">Por exemplo, a precisão pode ser medida em metros, como a precisão da latitude e da longitude em um raio de 50 metros.</span><span class="sxs-lookup"><span data-stu-id="ed971-114">As an example, the accuracy can be measured in meters, such as the latitude and longitude are accurate to within 50 meters.</span></span>|
|<span data-ttu-id="ed971-115">altitude</span><span class="sxs-lookup"><span data-stu-id="ed971-115">altitude</span></span>|<span data-ttu-id="ed971-116">double</span><span class="sxs-lookup"><span data-stu-id="ed971-116">double</span></span>|<span data-ttu-id="ed971-117">A altitude do local.</span><span class="sxs-lookup"><span data-stu-id="ed971-117">The altitude of the location.</span></span>|
|<span data-ttu-id="ed971-118">altitudeAccuracy</span><span class="sxs-lookup"><span data-stu-id="ed971-118">altitudeAccuracy</span></span>|<span data-ttu-id="ed971-119">double</span><span class="sxs-lookup"><span data-stu-id="ed971-119">double</span></span>|<span data-ttu-id="ed971-120">A precisão da altitude.</span><span class="sxs-lookup"><span data-stu-id="ed971-120">The accuracy of the altitude.</span></span>|
|<span data-ttu-id="ed971-121">latitude</span><span class="sxs-lookup"><span data-stu-id="ed971-121">latitude</span></span>|<span data-ttu-id="ed971-122">double</span><span class="sxs-lookup"><span data-stu-id="ed971-122">double</span></span>|<span data-ttu-id="ed971-123">A latitude do local.</span><span class="sxs-lookup"><span data-stu-id="ed971-123">The latitude of the location.</span></span>|
|<span data-ttu-id="ed971-124">longitude</span><span class="sxs-lookup"><span data-stu-id="ed971-124">longitude</span></span>|<span data-ttu-id="ed971-125">double</span><span class="sxs-lookup"><span data-stu-id="ed971-125">double</span></span>|<span data-ttu-id="ed971-126">A longitude do local.</span><span class="sxs-lookup"><span data-stu-id="ed971-126">The longitude of the location.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookGeoCoordinates resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
