---
title: Tipo de recurso deviceGeoLocation
description: Localização do dispositivo
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5aa5c419acea39c48ab14ac503b34dcdf0110aec
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49293035"
---
# <a name="devicegeolocation-resource-type"></a><span data-ttu-id="51287-103">Tipo de recurso deviceGeoLocation</span><span class="sxs-lookup"><span data-stu-id="51287-103">deviceGeoLocation resource type</span></span>

<span data-ttu-id="51287-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="51287-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="51287-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="51287-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="51287-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="51287-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="51287-107">Localização do dispositivo</span><span class="sxs-lookup"><span data-stu-id="51287-107">Device location</span></span>

## <a name="properties"></a><span data-ttu-id="51287-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="51287-108">Properties</span></span>
|<span data-ttu-id="51287-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="51287-109">Property</span></span>|<span data-ttu-id="51287-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="51287-110">Type</span></span>|<span data-ttu-id="51287-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="51287-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="51287-112">lastCollectedDateTimeUtc</span><span class="sxs-lookup"><span data-stu-id="51287-112">lastCollectedDateTimeUtc</span></span>|<span data-ttu-id="51287-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="51287-113">DateTimeOffset</span></span>|<span data-ttu-id="51287-114">Hora em que a localização foi registrada, em relação ao UTC</span><span class="sxs-lookup"><span data-stu-id="51287-114">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="51287-115">lastCollectedDateTime</span><span class="sxs-lookup"><span data-stu-id="51287-115">lastCollectedDateTime</span></span>|<span data-ttu-id="51287-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="51287-116">DateTimeOffset</span></span>|<span data-ttu-id="51287-117">Hora em que a localização foi registrada, em relação ao UTC</span><span class="sxs-lookup"><span data-stu-id="51287-117">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="51287-118">longitude</span><span class="sxs-lookup"><span data-stu-id="51287-118">longitude</span></span>|<span data-ttu-id="51287-119">Double</span><span class="sxs-lookup"><span data-stu-id="51287-119">Double</span></span>|<span data-ttu-id="51287-120">Coordenada de longitude da localização do dispositivo</span><span class="sxs-lookup"><span data-stu-id="51287-120">Longitude coordinate of the device's location</span></span>|
|<span data-ttu-id="51287-121">latitude</span><span class="sxs-lookup"><span data-stu-id="51287-121">latitude</span></span>|<span data-ttu-id="51287-122">Double</span><span class="sxs-lookup"><span data-stu-id="51287-122">Double</span></span>|<span data-ttu-id="51287-123">Coordenada de latitude da localização do dispositivo</span><span class="sxs-lookup"><span data-stu-id="51287-123">Latitude coordinate of the device's location</span></span>|
|<span data-ttu-id="51287-124">altitude</span><span class="sxs-lookup"><span data-stu-id="51287-124">altitude</span></span>|<span data-ttu-id="51287-125">Double</span><span class="sxs-lookup"><span data-stu-id="51287-125">Double</span></span>|<span data-ttu-id="51287-126">Altitude, especificada em metros acima do nível do mar</span><span class="sxs-lookup"><span data-stu-id="51287-126">Altitude, given in meters above sea level</span></span>|
|<span data-ttu-id="51287-127">horizontalAccuracy</span><span class="sxs-lookup"><span data-stu-id="51287-127">horizontalAccuracy</span></span>|<span data-ttu-id="51287-128">Double</span><span class="sxs-lookup"><span data-stu-id="51287-128">Double</span></span>|<span data-ttu-id="51287-129">Precisão da latitude e da longitude em metros</span><span class="sxs-lookup"><span data-stu-id="51287-129">Accuracy of longitude and latitude in meters</span></span>|
|<span data-ttu-id="51287-130">verticalAccuracy</span><span class="sxs-lookup"><span data-stu-id="51287-130">verticalAccuracy</span></span>|<span data-ttu-id="51287-131">Double</span><span class="sxs-lookup"><span data-stu-id="51287-131">Double</span></span>|<span data-ttu-id="51287-132">Precisão da altitude em metros</span><span class="sxs-lookup"><span data-stu-id="51287-132">Accuracy of altitude in meters</span></span>|
|<span data-ttu-id="51287-133">heading</span><span class="sxs-lookup"><span data-stu-id="51287-133">heading</span></span>|<span data-ttu-id="51287-134">Double</span><span class="sxs-lookup"><span data-stu-id="51287-134">Double</span></span>|<span data-ttu-id="51287-135">Direção em graus do norte verdadeiro</span><span class="sxs-lookup"><span data-stu-id="51287-135">Heading in degrees from true north</span></span>|
|<span data-ttu-id="51287-136">speed</span><span class="sxs-lookup"><span data-stu-id="51287-136">speed</span></span>|<span data-ttu-id="51287-137">Double</span><span class="sxs-lookup"><span data-stu-id="51287-137">Double</span></span>|<span data-ttu-id="51287-138">Velocidade na qual o dispositivo está viajando, em metros por segundo</span><span class="sxs-lookup"><span data-stu-id="51287-138">Speed the device is traveling in meters per second</span></span>|

## <a name="relationships"></a><span data-ttu-id="51287-139">Relações</span><span class="sxs-lookup"><span data-stu-id="51287-139">Relationships</span></span>
<span data-ttu-id="51287-140">Nenhum</span><span class="sxs-lookup"><span data-stu-id="51287-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="51287-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="51287-141">JSON Representation</span></span>
<span data-ttu-id="51287-142">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="51287-142">Here is a JSON representation of the resource.</span></span>
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




