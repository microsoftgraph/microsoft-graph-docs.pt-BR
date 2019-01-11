---
title: Tipo de recurso outlookGeoCoordinates
description: As coordenadas geográficas, a elevação e o grau de precisão delas para um local físico.
localization_priority: Normal
ms.openlocfilehash: 2522410cd55705411084945b0519738871dedaa0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845357"
---
# <a name="outlookgeocoordinates-resource-type"></a><span data-ttu-id="a726d-103">Tipo de recurso outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="a726d-103">outlookGeoCoordinates resource type</span></span>

> <span data-ttu-id="a726d-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a726d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a726d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a726d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a726d-106">As coordenadas geográficas, a elevação e o grau de precisão delas para um local físico.</span><span class="sxs-lookup"><span data-stu-id="a726d-106">The geographic coordinates, elevation, and their degree of accuracy for a physical location.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a726d-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a726d-107">JSON representation</span></span>

<span data-ttu-id="a726d-108">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a726d-108">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="a726d-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a726d-109">Properties</span></span>
| <span data-ttu-id="a726d-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a726d-110">Property</span></span>     | <span data-ttu-id="a726d-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="a726d-111">Type</span></span>   |<span data-ttu-id="a726d-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="a726d-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a726d-113">accuracy</span><span class="sxs-lookup"><span data-stu-id="a726d-113">accuracy</span></span>|<span data-ttu-id="a726d-114">double</span><span class="sxs-lookup"><span data-stu-id="a726d-114">double</span></span>|<span data-ttu-id="a726d-115">A precisão da latitude e da longitude.</span><span class="sxs-lookup"><span data-stu-id="a726d-115">The accuracy of the latitude and longitude.</span></span> <span data-ttu-id="a726d-116">Por exemplo, a precisão pode ser medida em metros, como a precisão da latitude e da longitude em um raio de 50 metros.</span><span class="sxs-lookup"><span data-stu-id="a726d-116">As an example, the accuracy can be measured in meters, such as the latitude and longitude are accurate to within 50 meters.</span></span>|
|<span data-ttu-id="a726d-117">altitude</span><span class="sxs-lookup"><span data-stu-id="a726d-117">altitude</span></span>|<span data-ttu-id="a726d-118">double</span><span class="sxs-lookup"><span data-stu-id="a726d-118">double</span></span>|<span data-ttu-id="a726d-119">A altitude do local.</span><span class="sxs-lookup"><span data-stu-id="a726d-119">The altitude of the location.</span></span>|
|<span data-ttu-id="a726d-120">altitudeAccuracy</span><span class="sxs-lookup"><span data-stu-id="a726d-120">altitudeAccuracy</span></span>|<span data-ttu-id="a726d-121">double</span><span class="sxs-lookup"><span data-stu-id="a726d-121">double</span></span>|<span data-ttu-id="a726d-122">A precisão da altitude.</span><span class="sxs-lookup"><span data-stu-id="a726d-122">The accuracy of the altitude.</span></span>|
|<span data-ttu-id="a726d-123">latitude</span><span class="sxs-lookup"><span data-stu-id="a726d-123">latitude</span></span>|<span data-ttu-id="a726d-124">double</span><span class="sxs-lookup"><span data-stu-id="a726d-124">double</span></span>|<span data-ttu-id="a726d-125">A latitude do local.</span><span class="sxs-lookup"><span data-stu-id="a726d-125">The latitude of the location.</span></span>|
|<span data-ttu-id="a726d-126">longitude</span><span class="sxs-lookup"><span data-stu-id="a726d-126">longitude</span></span>|<span data-ttu-id="a726d-127">double</span><span class="sxs-lookup"><span data-stu-id="a726d-127">double</span></span>|<span data-ttu-id="a726d-128">A longitude do local.</span><span class="sxs-lookup"><span data-stu-id="a726d-128">The longitude of the location.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookGeoCoordinates resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
