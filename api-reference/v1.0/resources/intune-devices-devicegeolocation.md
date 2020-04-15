---
title: Tipo de recurso deviceGeoLocation
description: Localização do dispositivo
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 091ef44a52e20acb987adddbac1c561087db718c
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43368309"
---
# <a name="devicegeolocation-resource-type"></a><span data-ttu-id="5cf63-103">Tipo de recurso deviceGeoLocation</span><span class="sxs-lookup"><span data-stu-id="5cf63-103">deviceGeoLocation resource type</span></span>

<span data-ttu-id="5cf63-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5cf63-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5cf63-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5cf63-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5cf63-106">Localização do dispositivo</span><span class="sxs-lookup"><span data-stu-id="5cf63-106">Device location</span></span>

## <a name="properties"></a><span data-ttu-id="5cf63-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5cf63-107">Properties</span></span>
|<span data-ttu-id="5cf63-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5cf63-108">Property</span></span>|<span data-ttu-id="5cf63-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="5cf63-109">Type</span></span>|<span data-ttu-id="5cf63-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="5cf63-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5cf63-111">lastCollectedDateTime</span><span class="sxs-lookup"><span data-stu-id="5cf63-111">lastCollectedDateTime</span></span>|<span data-ttu-id="5cf63-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5cf63-112">DateTimeOffset</span></span>|<span data-ttu-id="5cf63-113">Hora em que a localização foi registrada, em relação ao UTC</span><span class="sxs-lookup"><span data-stu-id="5cf63-113">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="5cf63-114">longitude</span><span class="sxs-lookup"><span data-stu-id="5cf63-114">longitude</span></span>|<span data-ttu-id="5cf63-115">Duplo</span><span class="sxs-lookup"><span data-stu-id="5cf63-115">Double</span></span>|<span data-ttu-id="5cf63-116">Coordenada de longitude da localização do dispositivo</span><span class="sxs-lookup"><span data-stu-id="5cf63-116">Longitude coordinate of the device's location</span></span>|
|<span data-ttu-id="5cf63-117">latitude</span><span class="sxs-lookup"><span data-stu-id="5cf63-117">latitude</span></span>|<span data-ttu-id="5cf63-118">Duplo</span><span class="sxs-lookup"><span data-stu-id="5cf63-118">Double</span></span>|<span data-ttu-id="5cf63-119">Coordenada de latitude da localização do dispositivo</span><span class="sxs-lookup"><span data-stu-id="5cf63-119">Latitude coordinate of the device's location</span></span>|
|<span data-ttu-id="5cf63-120">altitude</span><span class="sxs-lookup"><span data-stu-id="5cf63-120">altitude</span></span>|<span data-ttu-id="5cf63-121">Duplo</span><span class="sxs-lookup"><span data-stu-id="5cf63-121">Double</span></span>|<span data-ttu-id="5cf63-122">Altitude, especificada em metros acima do nível do mar</span><span class="sxs-lookup"><span data-stu-id="5cf63-122">Altitude, given in meters above sea level</span></span>|
|<span data-ttu-id="5cf63-123">horizontalAccuracy</span><span class="sxs-lookup"><span data-stu-id="5cf63-123">horizontalAccuracy</span></span>|<span data-ttu-id="5cf63-124">Duplo</span><span class="sxs-lookup"><span data-stu-id="5cf63-124">Double</span></span>|<span data-ttu-id="5cf63-125">Precisão da latitude e da longitude em metros</span><span class="sxs-lookup"><span data-stu-id="5cf63-125">Accuracy of longitude and latitude in meters</span></span>|
|<span data-ttu-id="5cf63-126">verticalAccuracy</span><span class="sxs-lookup"><span data-stu-id="5cf63-126">verticalAccuracy</span></span>|<span data-ttu-id="5cf63-127">Duplo</span><span class="sxs-lookup"><span data-stu-id="5cf63-127">Double</span></span>|<span data-ttu-id="5cf63-128">Precisão da altitude em metros</span><span class="sxs-lookup"><span data-stu-id="5cf63-128">Accuracy of altitude in meters</span></span>|
|<span data-ttu-id="5cf63-129">heading</span><span class="sxs-lookup"><span data-stu-id="5cf63-129">heading</span></span>|<span data-ttu-id="5cf63-130">Duplo</span><span class="sxs-lookup"><span data-stu-id="5cf63-130">Double</span></span>|<span data-ttu-id="5cf63-131">Direção em graus do norte verdadeiro</span><span class="sxs-lookup"><span data-stu-id="5cf63-131">Heading in degrees from true north</span></span>|
|<span data-ttu-id="5cf63-132">speed</span><span class="sxs-lookup"><span data-stu-id="5cf63-132">speed</span></span>|<span data-ttu-id="5cf63-133">Double</span><span class="sxs-lookup"><span data-stu-id="5cf63-133">Double</span></span>|<span data-ttu-id="5cf63-134">Velocidade na qual o dispositivo está viajando, em metros por segundo</span><span class="sxs-lookup"><span data-stu-id="5cf63-134">Speed the device is traveling in meters per second</span></span>|

## <a name="relationships"></a><span data-ttu-id="5cf63-135">Relações</span><span class="sxs-lookup"><span data-stu-id="5cf63-135">Relationships</span></span>
<span data-ttu-id="5cf63-136">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5cf63-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5cf63-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5cf63-137">JSON Representation</span></span>
<span data-ttu-id="5cf63-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5cf63-138">Here is a JSON representation of the resource.</span></span>
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







