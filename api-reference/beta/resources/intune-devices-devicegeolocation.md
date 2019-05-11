---
title: Tipo de recurso deviceGeoLocation
description: Localização do dispositivo
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 46a92f1faad55d82e2ed8184c5f4a4d360b7d588
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33942133"
---
# <a name="devicegeolocation-resource-type"></a><span data-ttu-id="826c7-103">Tipo de recurso deviceGeoLocation</span><span class="sxs-lookup"><span data-stu-id="826c7-103">deviceGeoLocation resource type</span></span>

> <span data-ttu-id="826c7-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="826c7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="826c7-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="826c7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="826c7-106">Localização do dispositivo</span><span class="sxs-lookup"><span data-stu-id="826c7-106">Device location</span></span>

## <a name="properties"></a><span data-ttu-id="826c7-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="826c7-107">Properties</span></span>
|<span data-ttu-id="826c7-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="826c7-108">Property</span></span>|<span data-ttu-id="826c7-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="826c7-109">Type</span></span>|<span data-ttu-id="826c7-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="826c7-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="826c7-111">lastCollectedDateTimeUtc</span><span class="sxs-lookup"><span data-stu-id="826c7-111">lastCollectedDateTimeUtc</span></span>|<span data-ttu-id="826c7-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="826c7-112">DateTimeOffset</span></span>|<span data-ttu-id="826c7-113">Hora em que a localização foi registrada, em relação ao UTC</span><span class="sxs-lookup"><span data-stu-id="826c7-113">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="826c7-114">lastCollectedDateTime</span><span class="sxs-lookup"><span data-stu-id="826c7-114">lastCollectedDateTime</span></span>|<span data-ttu-id="826c7-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="826c7-115">DateTimeOffset</span></span>|<span data-ttu-id="826c7-116">Hora em que a localização foi registrada, em relação ao UTC</span><span class="sxs-lookup"><span data-stu-id="826c7-116">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="826c7-117">longitude</span><span class="sxs-lookup"><span data-stu-id="826c7-117">longitude</span></span>|<span data-ttu-id="826c7-118">Duplo</span><span class="sxs-lookup"><span data-stu-id="826c7-118">Double</span></span>|<span data-ttu-id="826c7-119">Coordenada de longitude da localização do dispositivo</span><span class="sxs-lookup"><span data-stu-id="826c7-119">Longitude coordinate of the device's location</span></span>|
|<span data-ttu-id="826c7-120">latitude</span><span class="sxs-lookup"><span data-stu-id="826c7-120">latitude</span></span>|<span data-ttu-id="826c7-121">Duplo</span><span class="sxs-lookup"><span data-stu-id="826c7-121">Double</span></span>|<span data-ttu-id="826c7-122">Coordenada de latitude da localização do dispositivo</span><span class="sxs-lookup"><span data-stu-id="826c7-122">Latitude coordinate of the device's location</span></span>|
|<span data-ttu-id="826c7-123">altitude</span><span class="sxs-lookup"><span data-stu-id="826c7-123">altitude</span></span>|<span data-ttu-id="826c7-124">Duplo</span><span class="sxs-lookup"><span data-stu-id="826c7-124">Double</span></span>|<span data-ttu-id="826c7-125">Altitude, especificada em metros acima do nível do mar</span><span class="sxs-lookup"><span data-stu-id="826c7-125">Altitude, given in meters above sea level</span></span>|
|<span data-ttu-id="826c7-126">horizontalAccuracy</span><span class="sxs-lookup"><span data-stu-id="826c7-126">horizontalAccuracy</span></span>|<span data-ttu-id="826c7-127">Duplo</span><span class="sxs-lookup"><span data-stu-id="826c7-127">Double</span></span>|<span data-ttu-id="826c7-128">Precisão da latitude e da longitude em metros</span><span class="sxs-lookup"><span data-stu-id="826c7-128">Accuracy of longitude and latitude in meters</span></span>|
|<span data-ttu-id="826c7-129">verticalAccuracy</span><span class="sxs-lookup"><span data-stu-id="826c7-129">verticalAccuracy</span></span>|<span data-ttu-id="826c7-130">Duplo</span><span class="sxs-lookup"><span data-stu-id="826c7-130">Double</span></span>|<span data-ttu-id="826c7-131">Precisão da altitude em metros</span><span class="sxs-lookup"><span data-stu-id="826c7-131">Accuracy of altitude in meters</span></span>|
|<span data-ttu-id="826c7-132">heading</span><span class="sxs-lookup"><span data-stu-id="826c7-132">heading</span></span>|<span data-ttu-id="826c7-133">Duplo</span><span class="sxs-lookup"><span data-stu-id="826c7-133">Double</span></span>|<span data-ttu-id="826c7-134">Direção em graus do norte verdadeiro</span><span class="sxs-lookup"><span data-stu-id="826c7-134">Heading in degrees from true north</span></span>|
|<span data-ttu-id="826c7-135">speed</span><span class="sxs-lookup"><span data-stu-id="826c7-135">speed</span></span>|<span data-ttu-id="826c7-136">Double</span><span class="sxs-lookup"><span data-stu-id="826c7-136">Double</span></span>|<span data-ttu-id="826c7-137">Velocidade na qual o dispositivo está viajando, em metros por segundo</span><span class="sxs-lookup"><span data-stu-id="826c7-137">Speed the device is traveling in meters per second</span></span>|

## <a name="relationships"></a><span data-ttu-id="826c7-138">Relações</span><span class="sxs-lookup"><span data-stu-id="826c7-138">Relationships</span></span>
<span data-ttu-id="826c7-139">Nenhum</span><span class="sxs-lookup"><span data-stu-id="826c7-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="826c7-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="826c7-140">JSON Representation</span></span>
<span data-ttu-id="826c7-141">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="826c7-141">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceGeoLocation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceGeoLocation",
  "lastCollectedDateTimeUtc": "String (timestamp)",
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




