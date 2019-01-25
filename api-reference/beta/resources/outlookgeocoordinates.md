---
title: Tipo de recurso outlookGeoCoordinates
description: As coordenadas geográficas, a elevação e o grau de precisão delas para um local físico.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 7ca63aa3df6a597aaacb81fbeacf275ac87064f1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511832"
---
# <a name="outlookgeocoordinates-resource-type"></a><span data-ttu-id="4dbbb-103">Tipo de recurso outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="4dbbb-103">outlookGeoCoordinates resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4dbbb-104">As coordenadas geográficas, a elevação e o grau de precisão delas para um local físico.</span><span class="sxs-lookup"><span data-stu-id="4dbbb-104">The geographic coordinates, elevation, and their degree of accuracy for a physical location.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4dbbb-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4dbbb-105">JSON representation</span></span>

<span data-ttu-id="4dbbb-106">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4dbbb-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="4dbbb-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4dbbb-107">Properties</span></span>
| <span data-ttu-id="4dbbb-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4dbbb-108">Property</span></span>     | <span data-ttu-id="4dbbb-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="4dbbb-109">Type</span></span>   |<span data-ttu-id="4dbbb-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="4dbbb-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4dbbb-111">accuracy</span><span class="sxs-lookup"><span data-stu-id="4dbbb-111">accuracy</span></span>|<span data-ttu-id="4dbbb-112">double</span><span class="sxs-lookup"><span data-stu-id="4dbbb-112">double</span></span>|<span data-ttu-id="4dbbb-113">A precisão da latitude e da longitude.</span><span class="sxs-lookup"><span data-stu-id="4dbbb-113">The accuracy of the latitude and longitude.</span></span> <span data-ttu-id="4dbbb-114">Por exemplo, a precisão pode ser medida em metros, como a precisão da latitude e da longitude em um raio de 50 metros.</span><span class="sxs-lookup"><span data-stu-id="4dbbb-114">As an example, the accuracy can be measured in meters, such as the latitude and longitude are accurate to within 50 meters.</span></span>|
|<span data-ttu-id="4dbbb-115">altitude</span><span class="sxs-lookup"><span data-stu-id="4dbbb-115">altitude</span></span>|<span data-ttu-id="4dbbb-116">double</span><span class="sxs-lookup"><span data-stu-id="4dbbb-116">double</span></span>|<span data-ttu-id="4dbbb-117">A altitude do local.</span><span class="sxs-lookup"><span data-stu-id="4dbbb-117">The altitude of the location.</span></span>|
|<span data-ttu-id="4dbbb-118">altitudeAccuracy</span><span class="sxs-lookup"><span data-stu-id="4dbbb-118">altitudeAccuracy</span></span>|<span data-ttu-id="4dbbb-119">double</span><span class="sxs-lookup"><span data-stu-id="4dbbb-119">double</span></span>|<span data-ttu-id="4dbbb-120">A precisão da altitude.</span><span class="sxs-lookup"><span data-stu-id="4dbbb-120">The accuracy of the altitude.</span></span>|
|<span data-ttu-id="4dbbb-121">latitude</span><span class="sxs-lookup"><span data-stu-id="4dbbb-121">latitude</span></span>|<span data-ttu-id="4dbbb-122">double</span><span class="sxs-lookup"><span data-stu-id="4dbbb-122">double</span></span>|<span data-ttu-id="4dbbb-123">A latitude do local.</span><span class="sxs-lookup"><span data-stu-id="4dbbb-123">The latitude of the location.</span></span>|
|<span data-ttu-id="4dbbb-124">longitude</span><span class="sxs-lookup"><span data-stu-id="4dbbb-124">longitude</span></span>|<span data-ttu-id="4dbbb-125">double</span><span class="sxs-lookup"><span data-stu-id="4dbbb-125">double</span></span>|<span data-ttu-id="4dbbb-126">A longitude do local.</span><span class="sxs-lookup"><span data-stu-id="4dbbb-126">The longitude of the location.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "outlookGeoCoordinates resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/outlookgeocoordinates.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
