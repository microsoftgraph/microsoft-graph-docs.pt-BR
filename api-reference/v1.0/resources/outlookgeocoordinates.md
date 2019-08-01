---
title: Tipo de recurso outlookGeoCoordinates
description: As coordenadas geográficas, a elevação e o grau de precisão delas para um local físico.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 6cfa08c15318fdaa58ac71e01a940b621b207f12
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035669"
---
# <a name="outlookgeocoordinates-resource-type"></a><span data-ttu-id="11838-103">Tipo de recurso outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="11838-103">outlookGeoCoordinates resource type</span></span>

<span data-ttu-id="11838-104">As coordenadas geográficas, a elevação e o grau de precisão delas para um local físico.</span><span class="sxs-lookup"><span data-stu-id="11838-104">The geographic coordinates, elevation, and their degree of accuracy for a physical location.</span></span>

## <a name="json-representation"></a><span data-ttu-id="11838-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="11838-105">JSON representation</span></span>

<span data-ttu-id="11838-106">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="11838-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="11838-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="11838-107">Properties</span></span>
| <span data-ttu-id="11838-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="11838-108">Property</span></span>     | <span data-ttu-id="11838-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="11838-109">Type</span></span>   |<span data-ttu-id="11838-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="11838-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="11838-111">accuracy</span><span class="sxs-lookup"><span data-stu-id="11838-111">accuracy</span></span>|<span data-ttu-id="11838-112">double</span><span class="sxs-lookup"><span data-stu-id="11838-112">double</span></span>|<span data-ttu-id="11838-113">A precisão da latitude e da longitude.</span><span class="sxs-lookup"><span data-stu-id="11838-113">The accuracy of the latitude and longitude.</span></span> <span data-ttu-id="11838-114">Por exemplo, a precisão pode ser medida em metros, como a precisão da latitude e da longitude em um raio de 50 metros.</span><span class="sxs-lookup"><span data-stu-id="11838-114">As an example, the accuracy can be measured in meters, such as the latitude and longitude are accurate to within 50 meters.</span></span>|
|<span data-ttu-id="11838-115">altitude</span><span class="sxs-lookup"><span data-stu-id="11838-115">altitude</span></span>|<span data-ttu-id="11838-116">double</span><span class="sxs-lookup"><span data-stu-id="11838-116">double</span></span>|<span data-ttu-id="11838-117">A altitude do local.</span><span class="sxs-lookup"><span data-stu-id="11838-117">The altitude of the location.</span></span>|
|<span data-ttu-id="11838-118">altitudeAccuracy</span><span class="sxs-lookup"><span data-stu-id="11838-118">altitudeAccuracy</span></span>|<span data-ttu-id="11838-119">double</span><span class="sxs-lookup"><span data-stu-id="11838-119">double</span></span>|<span data-ttu-id="11838-120">A precisão da altitude.</span><span class="sxs-lookup"><span data-stu-id="11838-120">The accuracy of the altitude.</span></span>|
|<span data-ttu-id="11838-121">latitude</span><span class="sxs-lookup"><span data-stu-id="11838-121">latitude</span></span>|<span data-ttu-id="11838-122">double</span><span class="sxs-lookup"><span data-stu-id="11838-122">double</span></span>|<span data-ttu-id="11838-123">A latitude do local.</span><span class="sxs-lookup"><span data-stu-id="11838-123">The latitude of the location.</span></span>|
|<span data-ttu-id="11838-124">longitude</span><span class="sxs-lookup"><span data-stu-id="11838-124">longitude</span></span>|<span data-ttu-id="11838-125">double</span><span class="sxs-lookup"><span data-stu-id="11838-125">double</span></span>|<span data-ttu-id="11838-126">A longitude do local.</span><span class="sxs-lookup"><span data-stu-id="11838-126">The longitude of the location.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookGeoCoordinates resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
