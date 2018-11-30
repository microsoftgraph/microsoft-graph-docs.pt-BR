---
title: Tipo de recurso deviceGeoLocation
description: Localização do dispositivo
ms.openlocfilehash: 1bc72e4fb2d01c55d5d16ff2a45a020c5eaf99e5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006401"
---
# <a name="devicegeolocation-resource-type"></a><span data-ttu-id="ef046-103">Tipo de recurso deviceGeoLocation</span><span class="sxs-lookup"><span data-stu-id="ef046-103">deviceGeoLocation resource type</span></span>

> <span data-ttu-id="ef046-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="ef046-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ef046-105">Localização do dispositivo</span><span class="sxs-lookup"><span data-stu-id="ef046-105">Device location</span></span>
## <a name="properties"></a><span data-ttu-id="ef046-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ef046-106">Properties</span></span>
|<span data-ttu-id="ef046-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ef046-107">Property</span></span>|<span data-ttu-id="ef046-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="ef046-108">Type</span></span>|<span data-ttu-id="ef046-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="ef046-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ef046-110">lastCollectedDateTime</span><span class="sxs-lookup"><span data-stu-id="ef046-110">lastCollectedDateTime</span></span>|<span data-ttu-id="ef046-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ef046-111">DateTimeOffset</span></span>|<span data-ttu-id="ef046-112">Hora em que a localização foi registrada, em relação ao UTC</span><span class="sxs-lookup"><span data-stu-id="ef046-112">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="ef046-113">longitude</span><span class="sxs-lookup"><span data-stu-id="ef046-113">longitude</span></span>|<span data-ttu-id="ef046-114">Double</span><span class="sxs-lookup"><span data-stu-id="ef046-114">Double</span></span>|<span data-ttu-id="ef046-115">Coordenada de longitude da localização do dispositivo</span><span class="sxs-lookup"><span data-stu-id="ef046-115">Longitude coordinate of the device's location</span></span>|
|<span data-ttu-id="ef046-116">latitude</span><span class="sxs-lookup"><span data-stu-id="ef046-116">latitude</span></span>|<span data-ttu-id="ef046-117">Double</span><span class="sxs-lookup"><span data-stu-id="ef046-117">Double</span></span>|<span data-ttu-id="ef046-118">Coordenada de latitude da localização do dispositivo</span><span class="sxs-lookup"><span data-stu-id="ef046-118">Latitude coordinate of the device's location</span></span>|
|<span data-ttu-id="ef046-119">altitude</span><span class="sxs-lookup"><span data-stu-id="ef046-119">altitude</span></span>|<span data-ttu-id="ef046-120">Double</span><span class="sxs-lookup"><span data-stu-id="ef046-120">Double</span></span>|<span data-ttu-id="ef046-121">Altitude, especificada em metros acima do nível do mar</span><span class="sxs-lookup"><span data-stu-id="ef046-121">Altitude, given in meters above sea level</span></span>|
|<span data-ttu-id="ef046-122">horizontalAccuracy</span><span class="sxs-lookup"><span data-stu-id="ef046-122">horizontalAccuracy</span></span>|<span data-ttu-id="ef046-123">Double</span><span class="sxs-lookup"><span data-stu-id="ef046-123">Double</span></span>|<span data-ttu-id="ef046-124">Precisão da latitude e da longitude em metros</span><span class="sxs-lookup"><span data-stu-id="ef046-124">Accuracy of longitude and latitude in meters</span></span>|
|<span data-ttu-id="ef046-125">verticalAccuracy</span><span class="sxs-lookup"><span data-stu-id="ef046-125">verticalAccuracy</span></span>|<span data-ttu-id="ef046-126">Double</span><span class="sxs-lookup"><span data-stu-id="ef046-126">Double</span></span>|<span data-ttu-id="ef046-127">Precisão da altitude em metros</span><span class="sxs-lookup"><span data-stu-id="ef046-127">Accuracy of altitude in meters</span></span>|
|<span data-ttu-id="ef046-128">heading</span><span class="sxs-lookup"><span data-stu-id="ef046-128">heading</span></span>|<span data-ttu-id="ef046-129">Double</span><span class="sxs-lookup"><span data-stu-id="ef046-129">Double</span></span>|<span data-ttu-id="ef046-130">Direção em graus do norte verdadeiro</span><span class="sxs-lookup"><span data-stu-id="ef046-130">Heading in degrees from true north</span></span>|
|<span data-ttu-id="ef046-131">speed</span><span class="sxs-lookup"><span data-stu-id="ef046-131">speed</span></span>|<span data-ttu-id="ef046-132">Double</span><span class="sxs-lookup"><span data-stu-id="ef046-132">Double</span></span>|<span data-ttu-id="ef046-133">Velocidade na qual o dispositivo está viajando, em metros por segundo</span><span class="sxs-lookup"><span data-stu-id="ef046-133">Speed the device is traveling in meters per second</span></span>|

## <a name="relationships"></a><span data-ttu-id="ef046-134">Relações</span><span class="sxs-lookup"><span data-stu-id="ef046-134">Relationships</span></span>
<span data-ttu-id="ef046-135">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ef046-135">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ef046-136">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ef046-136">JSON Representation</span></span>
<span data-ttu-id="ef046-137">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ef046-137">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceGeoLocation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceGeoLocation",
  "lastCollectedDateTime": "String (timestamp)",
  "longitude": "<Unknown Primitive Type Edm.Double>",
  "latitude": "<Unknown Primitive Type Edm.Double>",
  "altitude": "<Unknown Primitive Type Edm.Double>",
  "horizontalAccuracy": "<Unknown Primitive Type Edm.Double>",
  "verticalAccuracy": "<Unknown Primitive Type Edm.Double>",
  "heading": "<Unknown Primitive Type Edm.Double>",
  "speed": "<Unknown Primitive Type Edm.Double>"
}
```



