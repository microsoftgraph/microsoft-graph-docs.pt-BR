---
title: Tipo de recurso deviceGeoLocation
description: Localização do dispositivo
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 896f463daadef157b9f8c10628dd9101508b88f0
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/09/2020
ms.locfileid: "44175641"
---
# <a name="devicegeolocation-resource-type"></a><span data-ttu-id="26b92-103">Tipo de recurso deviceGeoLocation</span><span class="sxs-lookup"><span data-stu-id="26b92-103">deviceGeoLocation resource type</span></span>

<span data-ttu-id="26b92-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="26b92-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="26b92-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="26b92-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="26b92-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="26b92-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="26b92-107">Localização do dispositivo</span><span class="sxs-lookup"><span data-stu-id="26b92-107">Device location</span></span>

## <a name="properties"></a><span data-ttu-id="26b92-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="26b92-108">Properties</span></span>
|<span data-ttu-id="26b92-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="26b92-109">Property</span></span>|<span data-ttu-id="26b92-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="26b92-110">Type</span></span>|<span data-ttu-id="26b92-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="26b92-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26b92-112">lastCollectedDateTimeUtc</span><span class="sxs-lookup"><span data-stu-id="26b92-112">lastCollectedDateTimeUtc</span></span>|<span data-ttu-id="26b92-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="26b92-113">DateTimeOffset</span></span>|<span data-ttu-id="26b92-114">Hora em que a localização foi registrada, em relação ao UTC</span><span class="sxs-lookup"><span data-stu-id="26b92-114">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="26b92-115">lastCollectedDateTime</span><span class="sxs-lookup"><span data-stu-id="26b92-115">lastCollectedDateTime</span></span>|<span data-ttu-id="26b92-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="26b92-116">DateTimeOffset</span></span>|<span data-ttu-id="26b92-117">Hora em que a localização foi registrada, em relação ao UTC</span><span class="sxs-lookup"><span data-stu-id="26b92-117">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="26b92-118">longitude</span><span class="sxs-lookup"><span data-stu-id="26b92-118">longitude</span></span>|<span data-ttu-id="26b92-119">Duplo</span><span class="sxs-lookup"><span data-stu-id="26b92-119">Double</span></span>|<span data-ttu-id="26b92-120">Coordenada de longitude da localização do dispositivo</span><span class="sxs-lookup"><span data-stu-id="26b92-120">Longitude coordinate of the device's location</span></span>|
|<span data-ttu-id="26b92-121">latitude</span><span class="sxs-lookup"><span data-stu-id="26b92-121">latitude</span></span>|<span data-ttu-id="26b92-122">Duplo</span><span class="sxs-lookup"><span data-stu-id="26b92-122">Double</span></span>|<span data-ttu-id="26b92-123">Coordenada de latitude da localização do dispositivo</span><span class="sxs-lookup"><span data-stu-id="26b92-123">Latitude coordinate of the device's location</span></span>|
|<span data-ttu-id="26b92-124">altitude</span><span class="sxs-lookup"><span data-stu-id="26b92-124">altitude</span></span>|<span data-ttu-id="26b92-125">Duplo</span><span class="sxs-lookup"><span data-stu-id="26b92-125">Double</span></span>|<span data-ttu-id="26b92-126">Altitude, especificada em metros acima do nível do mar</span><span class="sxs-lookup"><span data-stu-id="26b92-126">Altitude, given in meters above sea level</span></span>|
|<span data-ttu-id="26b92-127">horizontalAccuracy</span><span class="sxs-lookup"><span data-stu-id="26b92-127">horizontalAccuracy</span></span>|<span data-ttu-id="26b92-128">Duplo</span><span class="sxs-lookup"><span data-stu-id="26b92-128">Double</span></span>|<span data-ttu-id="26b92-129">Precisão da latitude e da longitude em metros</span><span class="sxs-lookup"><span data-stu-id="26b92-129">Accuracy of longitude and latitude in meters</span></span>|
|<span data-ttu-id="26b92-130">verticalAccuracy</span><span class="sxs-lookup"><span data-stu-id="26b92-130">verticalAccuracy</span></span>|<span data-ttu-id="26b92-131">Duplo</span><span class="sxs-lookup"><span data-stu-id="26b92-131">Double</span></span>|<span data-ttu-id="26b92-132">Precisão da altitude em metros</span><span class="sxs-lookup"><span data-stu-id="26b92-132">Accuracy of altitude in meters</span></span>|
|<span data-ttu-id="26b92-133">heading</span><span class="sxs-lookup"><span data-stu-id="26b92-133">heading</span></span>|<span data-ttu-id="26b92-134">Duplo</span><span class="sxs-lookup"><span data-stu-id="26b92-134">Double</span></span>|<span data-ttu-id="26b92-135">Direção em graus do norte verdadeiro</span><span class="sxs-lookup"><span data-stu-id="26b92-135">Heading in degrees from true north</span></span>|
|<span data-ttu-id="26b92-136">speed</span><span class="sxs-lookup"><span data-stu-id="26b92-136">speed</span></span>|<span data-ttu-id="26b92-137">Double</span><span class="sxs-lookup"><span data-stu-id="26b92-137">Double</span></span>|<span data-ttu-id="26b92-138">Velocidade na qual o dispositivo está viajando, em metros por segundo</span><span class="sxs-lookup"><span data-stu-id="26b92-138">Speed the device is traveling in meters per second</span></span>|

## <a name="relationships"></a><span data-ttu-id="26b92-139">Relações</span><span class="sxs-lookup"><span data-stu-id="26b92-139">Relationships</span></span>
<span data-ttu-id="26b92-140">Nenhum</span><span class="sxs-lookup"><span data-stu-id="26b92-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="26b92-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="26b92-141">JSON Representation</span></span>
<span data-ttu-id="26b92-142">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="26b92-142">Here is a JSON representation of the resource.</span></span>
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
  "longitude": "4.2",
  "latitude": "4.2",
  "altitude": "4.2",
  "horizontalAccuracy": "4.2",
  "verticalAccuracy": "4.2",
  "heading": "4.2",
  "speed": "4.2"
}
```



