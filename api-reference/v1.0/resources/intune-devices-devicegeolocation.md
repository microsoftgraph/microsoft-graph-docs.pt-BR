---
title: Tipo de recurso deviceGeoLocation
description: Localização do dispositivo
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 69e097d433d774c3dd445c94cd29eb059292806f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48091226"
---
# <a name="devicegeolocation-resource-type"></a><span data-ttu-id="2e93b-103">Tipo de recurso deviceGeoLocation</span><span class="sxs-lookup"><span data-stu-id="2e93b-103">deviceGeoLocation resource type</span></span>

<span data-ttu-id="2e93b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2e93b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2e93b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2e93b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2e93b-106">Localização do dispositivo</span><span class="sxs-lookup"><span data-stu-id="2e93b-106">Device location</span></span>

## <a name="properties"></a><span data-ttu-id="2e93b-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2e93b-107">Properties</span></span>
|<span data-ttu-id="2e93b-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2e93b-108">Property</span></span>|<span data-ttu-id="2e93b-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="2e93b-109">Type</span></span>|<span data-ttu-id="2e93b-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="2e93b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2e93b-111">lastCollectedDateTime</span><span class="sxs-lookup"><span data-stu-id="2e93b-111">lastCollectedDateTime</span></span>|<span data-ttu-id="2e93b-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2e93b-112">DateTimeOffset</span></span>|<span data-ttu-id="2e93b-113">Hora em que a localização foi registrada, em relação ao UTC</span><span class="sxs-lookup"><span data-stu-id="2e93b-113">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="2e93b-114">longitude</span><span class="sxs-lookup"><span data-stu-id="2e93b-114">longitude</span></span>|<span data-ttu-id="2e93b-115">Double</span><span class="sxs-lookup"><span data-stu-id="2e93b-115">Double</span></span>|<span data-ttu-id="2e93b-116">Coordenada de longitude da localização do dispositivo</span><span class="sxs-lookup"><span data-stu-id="2e93b-116">Longitude coordinate of the device's location</span></span>|
|<span data-ttu-id="2e93b-117">latitude</span><span class="sxs-lookup"><span data-stu-id="2e93b-117">latitude</span></span>|<span data-ttu-id="2e93b-118">Double</span><span class="sxs-lookup"><span data-stu-id="2e93b-118">Double</span></span>|<span data-ttu-id="2e93b-119">Coordenada de latitude da localização do dispositivo</span><span class="sxs-lookup"><span data-stu-id="2e93b-119">Latitude coordinate of the device's location</span></span>|
|<span data-ttu-id="2e93b-120">altitude</span><span class="sxs-lookup"><span data-stu-id="2e93b-120">altitude</span></span>|<span data-ttu-id="2e93b-121">Double</span><span class="sxs-lookup"><span data-stu-id="2e93b-121">Double</span></span>|<span data-ttu-id="2e93b-122">Altitude, especificada em metros acima do nível do mar</span><span class="sxs-lookup"><span data-stu-id="2e93b-122">Altitude, given in meters above sea level</span></span>|
|<span data-ttu-id="2e93b-123">horizontalAccuracy</span><span class="sxs-lookup"><span data-stu-id="2e93b-123">horizontalAccuracy</span></span>|<span data-ttu-id="2e93b-124">Double</span><span class="sxs-lookup"><span data-stu-id="2e93b-124">Double</span></span>|<span data-ttu-id="2e93b-125">Precisão da latitude e da longitude em metros</span><span class="sxs-lookup"><span data-stu-id="2e93b-125">Accuracy of longitude and latitude in meters</span></span>|
|<span data-ttu-id="2e93b-126">verticalAccuracy</span><span class="sxs-lookup"><span data-stu-id="2e93b-126">verticalAccuracy</span></span>|<span data-ttu-id="2e93b-127">Double</span><span class="sxs-lookup"><span data-stu-id="2e93b-127">Double</span></span>|<span data-ttu-id="2e93b-128">Precisão da altitude em metros</span><span class="sxs-lookup"><span data-stu-id="2e93b-128">Accuracy of altitude in meters</span></span>|
|<span data-ttu-id="2e93b-129">heading</span><span class="sxs-lookup"><span data-stu-id="2e93b-129">heading</span></span>|<span data-ttu-id="2e93b-130">Double</span><span class="sxs-lookup"><span data-stu-id="2e93b-130">Double</span></span>|<span data-ttu-id="2e93b-131">Direção em graus do norte verdadeiro</span><span class="sxs-lookup"><span data-stu-id="2e93b-131">Heading in degrees from true north</span></span>|
|<span data-ttu-id="2e93b-132">speed</span><span class="sxs-lookup"><span data-stu-id="2e93b-132">speed</span></span>|<span data-ttu-id="2e93b-133">Double</span><span class="sxs-lookup"><span data-stu-id="2e93b-133">Double</span></span>|<span data-ttu-id="2e93b-134">Velocidade na qual o dispositivo está viajando, em metros por segundo</span><span class="sxs-lookup"><span data-stu-id="2e93b-134">Speed the device is traveling in meters per second</span></span>|

## <a name="relationships"></a><span data-ttu-id="2e93b-135">Relações</span><span class="sxs-lookup"><span data-stu-id="2e93b-135">Relationships</span></span>
<span data-ttu-id="2e93b-136">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2e93b-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2e93b-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2e93b-137">JSON Representation</span></span>
<span data-ttu-id="2e93b-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2e93b-138">Here is a JSON representation of the resource.</span></span>
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









