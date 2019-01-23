---
title: Tipo de recurso deviceGeoLocation
description: Localização do dispositivo
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3b2105711a9a8f84b705a5a01c658c87cbe48c75
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395052"
---
# <a name="devicegeolocation-resource-type"></a><span data-ttu-id="11a79-103">Tipo de recurso deviceGeoLocation</span><span class="sxs-lookup"><span data-stu-id="11a79-103">deviceGeoLocation resource type</span></span>

> <span data-ttu-id="11a79-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="11a79-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="11a79-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="11a79-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="11a79-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="11a79-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="11a79-107">Localização do dispositivo</span><span class="sxs-lookup"><span data-stu-id="11a79-107">Device location</span></span>

## <a name="properties"></a><span data-ttu-id="11a79-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="11a79-108">Properties</span></span>
|<span data-ttu-id="11a79-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="11a79-109">Property</span></span>|<span data-ttu-id="11a79-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="11a79-110">Type</span></span>|<span data-ttu-id="11a79-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="11a79-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11a79-112">lastCollectedDateTimeUtc</span><span class="sxs-lookup"><span data-stu-id="11a79-112">lastCollectedDateTimeUtc</span></span>|<span data-ttu-id="11a79-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="11a79-113">DateTimeOffset</span></span>|<span data-ttu-id="11a79-114">Hora em que a localização foi registrada, em relação ao UTC</span><span class="sxs-lookup"><span data-stu-id="11a79-114">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="11a79-115">lastCollectedDateTime</span><span class="sxs-lookup"><span data-stu-id="11a79-115">lastCollectedDateTime</span></span>|<span data-ttu-id="11a79-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="11a79-116">DateTimeOffset</span></span>|<span data-ttu-id="11a79-117">Hora em que a localização foi registrada, em relação ao UTC</span><span class="sxs-lookup"><span data-stu-id="11a79-117">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="11a79-118">longitude</span><span class="sxs-lookup"><span data-stu-id="11a79-118">longitude</span></span>|<span data-ttu-id="11a79-119">Double</span><span class="sxs-lookup"><span data-stu-id="11a79-119">Double</span></span>|<span data-ttu-id="11a79-120">Coordenada de longitude da localização do dispositivo</span><span class="sxs-lookup"><span data-stu-id="11a79-120">Longitude coordinate of the device's location</span></span>|
|<span data-ttu-id="11a79-121">latitude</span><span class="sxs-lookup"><span data-stu-id="11a79-121">latitude</span></span>|<span data-ttu-id="11a79-122">Double</span><span class="sxs-lookup"><span data-stu-id="11a79-122">Double</span></span>|<span data-ttu-id="11a79-123">Coordenada de latitude da localização do dispositivo</span><span class="sxs-lookup"><span data-stu-id="11a79-123">Latitude coordinate of the device's location</span></span>|
|<span data-ttu-id="11a79-124">altitude</span><span class="sxs-lookup"><span data-stu-id="11a79-124">altitude</span></span>|<span data-ttu-id="11a79-125">Double</span><span class="sxs-lookup"><span data-stu-id="11a79-125">Double</span></span>|<span data-ttu-id="11a79-126">Altitude, especificada em metros acima do nível do mar</span><span class="sxs-lookup"><span data-stu-id="11a79-126">Altitude, given in meters above sea level</span></span>|
|<span data-ttu-id="11a79-127">horizontalAccuracy</span><span class="sxs-lookup"><span data-stu-id="11a79-127">horizontalAccuracy</span></span>|<span data-ttu-id="11a79-128">Double</span><span class="sxs-lookup"><span data-stu-id="11a79-128">Double</span></span>|<span data-ttu-id="11a79-129">Precisão da latitude e da longitude em metros</span><span class="sxs-lookup"><span data-stu-id="11a79-129">Accuracy of longitude and latitude in meters</span></span>|
|<span data-ttu-id="11a79-130">verticalAccuracy</span><span class="sxs-lookup"><span data-stu-id="11a79-130">verticalAccuracy</span></span>|<span data-ttu-id="11a79-131">Double</span><span class="sxs-lookup"><span data-stu-id="11a79-131">Double</span></span>|<span data-ttu-id="11a79-132">Precisão da altitude em metros</span><span class="sxs-lookup"><span data-stu-id="11a79-132">Accuracy of altitude in meters</span></span>|
|<span data-ttu-id="11a79-133">heading</span><span class="sxs-lookup"><span data-stu-id="11a79-133">heading</span></span>|<span data-ttu-id="11a79-134">Double</span><span class="sxs-lookup"><span data-stu-id="11a79-134">Double</span></span>|<span data-ttu-id="11a79-135">Direção em graus do norte verdadeiro</span><span class="sxs-lookup"><span data-stu-id="11a79-135">Heading in degrees from true north</span></span>|
|<span data-ttu-id="11a79-136">speed</span><span class="sxs-lookup"><span data-stu-id="11a79-136">speed</span></span>|<span data-ttu-id="11a79-137">Double</span><span class="sxs-lookup"><span data-stu-id="11a79-137">Double</span></span>|<span data-ttu-id="11a79-138">Velocidade na qual o dispositivo está viajando, em metros por segundo</span><span class="sxs-lookup"><span data-stu-id="11a79-138">Speed the device is traveling in meters per second</span></span>|

## <a name="relationships"></a><span data-ttu-id="11a79-139">Relações</span><span class="sxs-lookup"><span data-stu-id="11a79-139">Relationships</span></span>
<span data-ttu-id="11a79-140">Nenhum</span><span class="sxs-lookup"><span data-stu-id="11a79-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="11a79-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="11a79-141">JSON Representation</span></span>
<span data-ttu-id="11a79-142">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="11a79-142">Here is a JSON representation of the resource.</span></span>
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




