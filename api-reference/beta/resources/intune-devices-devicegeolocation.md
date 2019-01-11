---
title: Tipo de recurso deviceGeoLocation
description: Localização do dispositivo
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: dd81a0665d3d85a10488f78245449d265c85a8cc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845259"
---
# <a name="devicegeolocation-resource-type"></a><span data-ttu-id="0d11c-103">Tipo de recurso deviceGeoLocation</span><span class="sxs-lookup"><span data-stu-id="0d11c-103">deviceGeoLocation resource type</span></span>

> <span data-ttu-id="0d11c-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="0d11c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0d11c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="0d11c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0d11c-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="0d11c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0d11c-107">Localização do dispositivo</span><span class="sxs-lookup"><span data-stu-id="0d11c-107">Device location</span></span>
## <a name="properties"></a><span data-ttu-id="0d11c-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0d11c-108">Properties</span></span>
|<span data-ttu-id="0d11c-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0d11c-109">Property</span></span>|<span data-ttu-id="0d11c-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="0d11c-110">Type</span></span>|<span data-ttu-id="0d11c-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="0d11c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0d11c-112">lastCollectedDateTimeUtc</span><span class="sxs-lookup"><span data-stu-id="0d11c-112">lastCollectedDateTimeUtc</span></span>|<span data-ttu-id="0d11c-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0d11c-113">DateTimeOffset</span></span>|<span data-ttu-id="0d11c-114">Hora em que a localização foi registrada, em relação ao UTC</span><span class="sxs-lookup"><span data-stu-id="0d11c-114">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="0d11c-115">lastCollectedDateTime</span><span class="sxs-lookup"><span data-stu-id="0d11c-115">lastCollectedDateTime</span></span>|<span data-ttu-id="0d11c-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0d11c-116">DateTimeOffset</span></span>|<span data-ttu-id="0d11c-117">Hora em que a localização foi registrada, em relação ao UTC</span><span class="sxs-lookup"><span data-stu-id="0d11c-117">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="0d11c-118">longitude</span><span class="sxs-lookup"><span data-stu-id="0d11c-118">longitude</span></span>|<span data-ttu-id="0d11c-119">Double</span><span class="sxs-lookup"><span data-stu-id="0d11c-119">Double</span></span>|<span data-ttu-id="0d11c-120">Coordenada de longitude da localização do dispositivo</span><span class="sxs-lookup"><span data-stu-id="0d11c-120">Longitude coordinate of the device's location</span></span>|
|<span data-ttu-id="0d11c-121">latitude</span><span class="sxs-lookup"><span data-stu-id="0d11c-121">latitude</span></span>|<span data-ttu-id="0d11c-122">Double</span><span class="sxs-lookup"><span data-stu-id="0d11c-122">Double</span></span>|<span data-ttu-id="0d11c-123">Coordenada de latitude da localização do dispositivo</span><span class="sxs-lookup"><span data-stu-id="0d11c-123">Latitude coordinate of the device's location</span></span>|
|<span data-ttu-id="0d11c-124">altitude</span><span class="sxs-lookup"><span data-stu-id="0d11c-124">altitude</span></span>|<span data-ttu-id="0d11c-125">Double</span><span class="sxs-lookup"><span data-stu-id="0d11c-125">Double</span></span>|<span data-ttu-id="0d11c-126">Altitude, especificada em metros acima do nível do mar</span><span class="sxs-lookup"><span data-stu-id="0d11c-126">Altitude, given in meters above sea level</span></span>|
|<span data-ttu-id="0d11c-127">horizontalAccuracy</span><span class="sxs-lookup"><span data-stu-id="0d11c-127">horizontalAccuracy</span></span>|<span data-ttu-id="0d11c-128">Double</span><span class="sxs-lookup"><span data-stu-id="0d11c-128">Double</span></span>|<span data-ttu-id="0d11c-129">Precisão da latitude e da longitude em metros</span><span class="sxs-lookup"><span data-stu-id="0d11c-129">Accuracy of longitude and latitude in meters</span></span>|
|<span data-ttu-id="0d11c-130">verticalAccuracy</span><span class="sxs-lookup"><span data-stu-id="0d11c-130">verticalAccuracy</span></span>|<span data-ttu-id="0d11c-131">Double</span><span class="sxs-lookup"><span data-stu-id="0d11c-131">Double</span></span>|<span data-ttu-id="0d11c-132">Precisão da altitude em metros</span><span class="sxs-lookup"><span data-stu-id="0d11c-132">Accuracy of altitude in meters</span></span>|
|<span data-ttu-id="0d11c-133">heading</span><span class="sxs-lookup"><span data-stu-id="0d11c-133">heading</span></span>|<span data-ttu-id="0d11c-134">Double</span><span class="sxs-lookup"><span data-stu-id="0d11c-134">Double</span></span>|<span data-ttu-id="0d11c-135">Direção em graus do norte verdadeiro</span><span class="sxs-lookup"><span data-stu-id="0d11c-135">Heading in degrees from true north</span></span>|
|<span data-ttu-id="0d11c-136">speed</span><span class="sxs-lookup"><span data-stu-id="0d11c-136">speed</span></span>|<span data-ttu-id="0d11c-137">Double</span><span class="sxs-lookup"><span data-stu-id="0d11c-137">Double</span></span>|<span data-ttu-id="0d11c-138">Velocidade na qual o dispositivo está viajando, em metros por segundo</span><span class="sxs-lookup"><span data-stu-id="0d11c-138">Speed the device is traveling in meters per second</span></span>|

## <a name="relationships"></a><span data-ttu-id="0d11c-139">Relações</span><span class="sxs-lookup"><span data-stu-id="0d11c-139">Relationships</span></span>
<span data-ttu-id="0d11c-140">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0d11c-140">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0d11c-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0d11c-141">JSON Representation</span></span>
<span data-ttu-id="0d11c-142">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0d11c-142">Here is a JSON representation of the resource.</span></span>
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





