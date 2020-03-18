---
title: Tipo de recurso deviceGeoLocation
description: Localização do dispositivo
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3c3c8251987dee0aadafdb88eebd9e29afbb5f76
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42784997"
---
# <a name="devicegeolocation-resource-type"></a><span data-ttu-id="ba9d6-103">Tipo de recurso deviceGeoLocation</span><span class="sxs-lookup"><span data-stu-id="ba9d6-103">deviceGeoLocation resource type</span></span>

> <span data-ttu-id="ba9d6-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ba9d6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ba9d6-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ba9d6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ba9d6-106">Localização do dispositivo</span><span class="sxs-lookup"><span data-stu-id="ba9d6-106">Device location</span></span>

## <a name="properties"></a><span data-ttu-id="ba9d6-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ba9d6-107">Properties</span></span>
|<span data-ttu-id="ba9d6-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ba9d6-108">Property</span></span>|<span data-ttu-id="ba9d6-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="ba9d6-109">Type</span></span>|<span data-ttu-id="ba9d6-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="ba9d6-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ba9d6-111">lastCollectedDateTimeUtc</span><span class="sxs-lookup"><span data-stu-id="ba9d6-111">lastCollectedDateTimeUtc</span></span>|<span data-ttu-id="ba9d6-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ba9d6-112">DateTimeOffset</span></span>|<span data-ttu-id="ba9d6-113">Hora em que a localização foi registrada, em relação ao UTC</span><span class="sxs-lookup"><span data-stu-id="ba9d6-113">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="ba9d6-114">lastCollectedDateTime</span><span class="sxs-lookup"><span data-stu-id="ba9d6-114">lastCollectedDateTime</span></span>|<span data-ttu-id="ba9d6-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ba9d6-115">DateTimeOffset</span></span>|<span data-ttu-id="ba9d6-116">Hora em que a localização foi registrada, em relação ao UTC</span><span class="sxs-lookup"><span data-stu-id="ba9d6-116">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="ba9d6-117">longitude</span><span class="sxs-lookup"><span data-stu-id="ba9d6-117">longitude</span></span>|<span data-ttu-id="ba9d6-118">Duplo</span><span class="sxs-lookup"><span data-stu-id="ba9d6-118">Double</span></span>|<span data-ttu-id="ba9d6-119">Coordenada de longitude da localização do dispositivo</span><span class="sxs-lookup"><span data-stu-id="ba9d6-119">Longitude coordinate of the device's location</span></span>|
|<span data-ttu-id="ba9d6-120">latitude</span><span class="sxs-lookup"><span data-stu-id="ba9d6-120">latitude</span></span>|<span data-ttu-id="ba9d6-121">Duplo</span><span class="sxs-lookup"><span data-stu-id="ba9d6-121">Double</span></span>|<span data-ttu-id="ba9d6-122">Coordenada de latitude da localização do dispositivo</span><span class="sxs-lookup"><span data-stu-id="ba9d6-122">Latitude coordinate of the device's location</span></span>|
|<span data-ttu-id="ba9d6-123">altitude</span><span class="sxs-lookup"><span data-stu-id="ba9d6-123">altitude</span></span>|<span data-ttu-id="ba9d6-124">Duplo</span><span class="sxs-lookup"><span data-stu-id="ba9d6-124">Double</span></span>|<span data-ttu-id="ba9d6-125">Altitude, especificada em metros acima do nível do mar</span><span class="sxs-lookup"><span data-stu-id="ba9d6-125">Altitude, given in meters above sea level</span></span>|
|<span data-ttu-id="ba9d6-126">horizontalAccuracy</span><span class="sxs-lookup"><span data-stu-id="ba9d6-126">horizontalAccuracy</span></span>|<span data-ttu-id="ba9d6-127">Duplo</span><span class="sxs-lookup"><span data-stu-id="ba9d6-127">Double</span></span>|<span data-ttu-id="ba9d6-128">Precisão da latitude e da longitude em metros</span><span class="sxs-lookup"><span data-stu-id="ba9d6-128">Accuracy of longitude and latitude in meters</span></span>|
|<span data-ttu-id="ba9d6-129">verticalAccuracy</span><span class="sxs-lookup"><span data-stu-id="ba9d6-129">verticalAccuracy</span></span>|<span data-ttu-id="ba9d6-130">Duplo</span><span class="sxs-lookup"><span data-stu-id="ba9d6-130">Double</span></span>|<span data-ttu-id="ba9d6-131">Precisão da altitude em metros</span><span class="sxs-lookup"><span data-stu-id="ba9d6-131">Accuracy of altitude in meters</span></span>|
|<span data-ttu-id="ba9d6-132">heading</span><span class="sxs-lookup"><span data-stu-id="ba9d6-132">heading</span></span>|<span data-ttu-id="ba9d6-133">Duplo</span><span class="sxs-lookup"><span data-stu-id="ba9d6-133">Double</span></span>|<span data-ttu-id="ba9d6-134">Direção em graus do norte verdadeiro</span><span class="sxs-lookup"><span data-stu-id="ba9d6-134">Heading in degrees from true north</span></span>|
|<span data-ttu-id="ba9d6-135">speed</span><span class="sxs-lookup"><span data-stu-id="ba9d6-135">speed</span></span>|<span data-ttu-id="ba9d6-136">Double</span><span class="sxs-lookup"><span data-stu-id="ba9d6-136">Double</span></span>|<span data-ttu-id="ba9d6-137">Velocidade na qual o dispositivo está viajando, em metros por segundo</span><span class="sxs-lookup"><span data-stu-id="ba9d6-137">Speed the device is traveling in meters per second</span></span>|

## <a name="relationships"></a><span data-ttu-id="ba9d6-138">Relações</span><span class="sxs-lookup"><span data-stu-id="ba9d6-138">Relationships</span></span>
<span data-ttu-id="ba9d6-139">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ba9d6-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ba9d6-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ba9d6-140">JSON Representation</span></span>
<span data-ttu-id="ba9d6-141">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ba9d6-141">Here is a JSON representation of the resource.</span></span>
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



