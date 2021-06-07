---
title: Tipo de recurso deviceGeoLocation
description: Localização do dispositivo
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a406ede926ad637a338437559840cdefdadc64ce
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754578"
---
# <a name="devicegeolocation-resource-type"></a><span data-ttu-id="74f61-103">Tipo de recurso deviceGeoLocation</span><span class="sxs-lookup"><span data-stu-id="74f61-103">deviceGeoLocation resource type</span></span>

<span data-ttu-id="74f61-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="74f61-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="74f61-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="74f61-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="74f61-106">Localização do dispositivo</span><span class="sxs-lookup"><span data-stu-id="74f61-106">Device location</span></span>

## <a name="properties"></a><span data-ttu-id="74f61-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="74f61-107">Properties</span></span>
|<span data-ttu-id="74f61-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="74f61-108">Property</span></span>|<span data-ttu-id="74f61-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="74f61-109">Type</span></span>|<span data-ttu-id="74f61-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="74f61-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="74f61-111">lastCollectedDateTime</span><span class="sxs-lookup"><span data-stu-id="74f61-111">lastCollectedDateTime</span></span>|<span data-ttu-id="74f61-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="74f61-112">DateTimeOffset</span></span>|<span data-ttu-id="74f61-113">Hora em que a localização foi registrada, em relação ao UTC</span><span class="sxs-lookup"><span data-stu-id="74f61-113">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="74f61-114">longitude</span><span class="sxs-lookup"><span data-stu-id="74f61-114">longitude</span></span>|<span data-ttu-id="74f61-115">Double</span><span class="sxs-lookup"><span data-stu-id="74f61-115">Double</span></span>|<span data-ttu-id="74f61-116">Coordenada de longitude da localização do dispositivo</span><span class="sxs-lookup"><span data-stu-id="74f61-116">Longitude coordinate of the device's location</span></span>|
|<span data-ttu-id="74f61-117">latitude</span><span class="sxs-lookup"><span data-stu-id="74f61-117">latitude</span></span>|<span data-ttu-id="74f61-118">Double</span><span class="sxs-lookup"><span data-stu-id="74f61-118">Double</span></span>|<span data-ttu-id="74f61-119">Coordenada de latitude da localização do dispositivo</span><span class="sxs-lookup"><span data-stu-id="74f61-119">Latitude coordinate of the device's location</span></span>|
|<span data-ttu-id="74f61-120">altitude</span><span class="sxs-lookup"><span data-stu-id="74f61-120">altitude</span></span>|<span data-ttu-id="74f61-121">Double</span><span class="sxs-lookup"><span data-stu-id="74f61-121">Double</span></span>|<span data-ttu-id="74f61-122">Altitude, especificada em metros acima do nível do mar</span><span class="sxs-lookup"><span data-stu-id="74f61-122">Altitude, given in meters above sea level</span></span>|
|<span data-ttu-id="74f61-123">horizontalAccuracy</span><span class="sxs-lookup"><span data-stu-id="74f61-123">horizontalAccuracy</span></span>|<span data-ttu-id="74f61-124">Double</span><span class="sxs-lookup"><span data-stu-id="74f61-124">Double</span></span>|<span data-ttu-id="74f61-125">Precisão da latitude e da longitude em metros</span><span class="sxs-lookup"><span data-stu-id="74f61-125">Accuracy of longitude and latitude in meters</span></span>|
|<span data-ttu-id="74f61-126">verticalAccuracy</span><span class="sxs-lookup"><span data-stu-id="74f61-126">verticalAccuracy</span></span>|<span data-ttu-id="74f61-127">Double</span><span class="sxs-lookup"><span data-stu-id="74f61-127">Double</span></span>|<span data-ttu-id="74f61-128">Precisão da altitude em metros</span><span class="sxs-lookup"><span data-stu-id="74f61-128">Accuracy of altitude in meters</span></span>|
|<span data-ttu-id="74f61-129">heading</span><span class="sxs-lookup"><span data-stu-id="74f61-129">heading</span></span>|<span data-ttu-id="74f61-130">Double</span><span class="sxs-lookup"><span data-stu-id="74f61-130">Double</span></span>|<span data-ttu-id="74f61-131">Direção em graus do norte verdadeiro</span><span class="sxs-lookup"><span data-stu-id="74f61-131">Heading in degrees from true north</span></span>|
|<span data-ttu-id="74f61-132">speed</span><span class="sxs-lookup"><span data-stu-id="74f61-132">speed</span></span>|<span data-ttu-id="74f61-133">Double</span><span class="sxs-lookup"><span data-stu-id="74f61-133">Double</span></span>|<span data-ttu-id="74f61-134">Velocidade na qual o dispositivo está viajando, em metros por segundo</span><span class="sxs-lookup"><span data-stu-id="74f61-134">Speed the device is traveling in meters per second</span></span>|

## <a name="relationships"></a><span data-ttu-id="74f61-135">Relações</span><span class="sxs-lookup"><span data-stu-id="74f61-135">Relationships</span></span>
<span data-ttu-id="74f61-136">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="74f61-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="74f61-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="74f61-137">JSON Representation</span></span>
<span data-ttu-id="74f61-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="74f61-138">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceGeoLocation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceGeoLocation",
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




