---
title: Tipo de recurso deviceGeoLocation
description: Localização do dispositivo
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b51768aea1338486431ceffadd95f8760a7216ab
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30260211"
---
# <a name="devicegeolocation-resource-type"></a><span data-ttu-id="81998-103">Tipo de recurso deviceGeoLocation</span><span class="sxs-lookup"><span data-stu-id="81998-103">deviceGeoLocation resource type</span></span>

> <span data-ttu-id="81998-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="81998-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="81998-105">Localização do dispositivo</span><span class="sxs-lookup"><span data-stu-id="81998-105">Device location</span></span>

## <a name="properties"></a><span data-ttu-id="81998-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="81998-106">Properties</span></span>
|<span data-ttu-id="81998-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="81998-107">Property</span></span>|<span data-ttu-id="81998-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="81998-108">Type</span></span>|<span data-ttu-id="81998-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="81998-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81998-110">lastCollectedDateTime</span><span class="sxs-lookup"><span data-stu-id="81998-110">lastCollectedDateTime</span></span>|<span data-ttu-id="81998-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="81998-111">DateTimeOffset</span></span>|<span data-ttu-id="81998-112">Hora em que a localização foi registrada, em relação ao UTC</span><span class="sxs-lookup"><span data-stu-id="81998-112">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="81998-113">longitude</span><span class="sxs-lookup"><span data-stu-id="81998-113">longitude</span></span>|<span data-ttu-id="81998-114">Duplo</span><span class="sxs-lookup"><span data-stu-id="81998-114">Double</span></span>|<span data-ttu-id="81998-115">Coordenada de longitude da localização do dispositivo</span><span class="sxs-lookup"><span data-stu-id="81998-115">Longitude coordinate of the device's location</span></span>|
|<span data-ttu-id="81998-116">latitude</span><span class="sxs-lookup"><span data-stu-id="81998-116">latitude</span></span>|<span data-ttu-id="81998-117">Duplo</span><span class="sxs-lookup"><span data-stu-id="81998-117">Double</span></span>|<span data-ttu-id="81998-118">Coordenada de latitude da localização do dispositivo</span><span class="sxs-lookup"><span data-stu-id="81998-118">Latitude coordinate of the device's location</span></span>|
|<span data-ttu-id="81998-119">altitude</span><span class="sxs-lookup"><span data-stu-id="81998-119">altitude</span></span>|<span data-ttu-id="81998-120">Duplo</span><span class="sxs-lookup"><span data-stu-id="81998-120">Double</span></span>|<span data-ttu-id="81998-121">Altitude, especificada em metros acima do nível do mar</span><span class="sxs-lookup"><span data-stu-id="81998-121">Altitude, given in meters above sea level</span></span>|
|<span data-ttu-id="81998-122">horizontalAccuracy</span><span class="sxs-lookup"><span data-stu-id="81998-122">horizontalAccuracy</span></span>|<span data-ttu-id="81998-123">Duplo</span><span class="sxs-lookup"><span data-stu-id="81998-123">Double</span></span>|<span data-ttu-id="81998-124">Precisão da latitude e da longitude em metros</span><span class="sxs-lookup"><span data-stu-id="81998-124">Accuracy of longitude and latitude in meters</span></span>|
|<span data-ttu-id="81998-125">verticalAccuracy</span><span class="sxs-lookup"><span data-stu-id="81998-125">verticalAccuracy</span></span>|<span data-ttu-id="81998-126">Duplo</span><span class="sxs-lookup"><span data-stu-id="81998-126">Double</span></span>|<span data-ttu-id="81998-127">Precisão da altitude em metros</span><span class="sxs-lookup"><span data-stu-id="81998-127">Accuracy of altitude in meters</span></span>|
|<span data-ttu-id="81998-128">heading</span><span class="sxs-lookup"><span data-stu-id="81998-128">heading</span></span>|<span data-ttu-id="81998-129">Duplo</span><span class="sxs-lookup"><span data-stu-id="81998-129">Double</span></span>|<span data-ttu-id="81998-130">Direção em graus do norte verdadeiro</span><span class="sxs-lookup"><span data-stu-id="81998-130">Heading in degrees from true north</span></span>|
|<span data-ttu-id="81998-131">speed</span><span class="sxs-lookup"><span data-stu-id="81998-131">speed</span></span>|<span data-ttu-id="81998-132">Double</span><span class="sxs-lookup"><span data-stu-id="81998-132">Double</span></span>|<span data-ttu-id="81998-133">Velocidade na qual o dispositivo está viajando, em metros por segundo</span><span class="sxs-lookup"><span data-stu-id="81998-133">Speed the device is traveling in meters per second</span></span>|

## <a name="relationships"></a><span data-ttu-id="81998-134">Relações</span><span class="sxs-lookup"><span data-stu-id="81998-134">Relationships</span></span>
<span data-ttu-id="81998-135">Nenhum</span><span class="sxs-lookup"><span data-stu-id="81998-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="81998-136">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="81998-136">JSON Representation</span></span>
<span data-ttu-id="81998-137">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="81998-137">Here is a JSON representation of the resource.</span></span>
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



