---
title: Tipo de recurso deviceGeoLocation
description: Localização do dispositivo
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7417f5020fd7496a2daecde3ffbeb6e7391eaf08
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528646"
---
# <a name="devicegeolocation-resource-type"></a><span data-ttu-id="dbd0f-103">Tipo de recurso deviceGeoLocation</span><span class="sxs-lookup"><span data-stu-id="dbd0f-103">deviceGeoLocation resource type</span></span>

<span data-ttu-id="dbd0f-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="dbd0f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dbd0f-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="dbd0f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dbd0f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="dbd0f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dbd0f-107">Localização do dispositivo</span><span class="sxs-lookup"><span data-stu-id="dbd0f-107">Device location</span></span>

## <a name="properties"></a><span data-ttu-id="dbd0f-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="dbd0f-108">Properties</span></span>
|<span data-ttu-id="dbd0f-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dbd0f-109">Property</span></span>|<span data-ttu-id="dbd0f-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="dbd0f-110">Type</span></span>|<span data-ttu-id="dbd0f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="dbd0f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dbd0f-112">lastCollectedDateTimeUtc</span><span class="sxs-lookup"><span data-stu-id="dbd0f-112">lastCollectedDateTimeUtc</span></span>|<span data-ttu-id="dbd0f-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dbd0f-113">DateTimeOffset</span></span>|<span data-ttu-id="dbd0f-114">Hora em que a localização foi registrada, em relação ao UTC</span><span class="sxs-lookup"><span data-stu-id="dbd0f-114">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="dbd0f-115">lastCollectedDateTime</span><span class="sxs-lookup"><span data-stu-id="dbd0f-115">lastCollectedDateTime</span></span>|<span data-ttu-id="dbd0f-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dbd0f-116">DateTimeOffset</span></span>|<span data-ttu-id="dbd0f-117">Hora em que a localização foi registrada, em relação ao UTC</span><span class="sxs-lookup"><span data-stu-id="dbd0f-117">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="dbd0f-118">longitude</span><span class="sxs-lookup"><span data-stu-id="dbd0f-118">longitude</span></span>|<span data-ttu-id="dbd0f-119">Duplo</span><span class="sxs-lookup"><span data-stu-id="dbd0f-119">Double</span></span>|<span data-ttu-id="dbd0f-120">Coordenada de longitude da localização do dispositivo</span><span class="sxs-lookup"><span data-stu-id="dbd0f-120">Longitude coordinate of the device's location</span></span>|
|<span data-ttu-id="dbd0f-121">latitude</span><span class="sxs-lookup"><span data-stu-id="dbd0f-121">latitude</span></span>|<span data-ttu-id="dbd0f-122">Duplo</span><span class="sxs-lookup"><span data-stu-id="dbd0f-122">Double</span></span>|<span data-ttu-id="dbd0f-123">Coordenada de latitude da localização do dispositivo</span><span class="sxs-lookup"><span data-stu-id="dbd0f-123">Latitude coordinate of the device's location</span></span>|
|<span data-ttu-id="dbd0f-124">altitude</span><span class="sxs-lookup"><span data-stu-id="dbd0f-124">altitude</span></span>|<span data-ttu-id="dbd0f-125">Duplo</span><span class="sxs-lookup"><span data-stu-id="dbd0f-125">Double</span></span>|<span data-ttu-id="dbd0f-126">Altitude, especificada em metros acima do nível do mar</span><span class="sxs-lookup"><span data-stu-id="dbd0f-126">Altitude, given in meters above sea level</span></span>|
|<span data-ttu-id="dbd0f-127">horizontalAccuracy</span><span class="sxs-lookup"><span data-stu-id="dbd0f-127">horizontalAccuracy</span></span>|<span data-ttu-id="dbd0f-128">Duplo</span><span class="sxs-lookup"><span data-stu-id="dbd0f-128">Double</span></span>|<span data-ttu-id="dbd0f-129">Precisão da latitude e da longitude em metros</span><span class="sxs-lookup"><span data-stu-id="dbd0f-129">Accuracy of longitude and latitude in meters</span></span>|
|<span data-ttu-id="dbd0f-130">verticalAccuracy</span><span class="sxs-lookup"><span data-stu-id="dbd0f-130">verticalAccuracy</span></span>|<span data-ttu-id="dbd0f-131">Duplo</span><span class="sxs-lookup"><span data-stu-id="dbd0f-131">Double</span></span>|<span data-ttu-id="dbd0f-132">Precisão da altitude em metros</span><span class="sxs-lookup"><span data-stu-id="dbd0f-132">Accuracy of altitude in meters</span></span>|
|<span data-ttu-id="dbd0f-133">heading</span><span class="sxs-lookup"><span data-stu-id="dbd0f-133">heading</span></span>|<span data-ttu-id="dbd0f-134">Duplo</span><span class="sxs-lookup"><span data-stu-id="dbd0f-134">Double</span></span>|<span data-ttu-id="dbd0f-135">Direção em graus do norte verdadeiro</span><span class="sxs-lookup"><span data-stu-id="dbd0f-135">Heading in degrees from true north</span></span>|
|<span data-ttu-id="dbd0f-136">speed</span><span class="sxs-lookup"><span data-stu-id="dbd0f-136">speed</span></span>|<span data-ttu-id="dbd0f-137">Double</span><span class="sxs-lookup"><span data-stu-id="dbd0f-137">Double</span></span>|<span data-ttu-id="dbd0f-138">Velocidade na qual o dispositivo está viajando, em metros por segundo</span><span class="sxs-lookup"><span data-stu-id="dbd0f-138">Speed the device is traveling in meters per second</span></span>|

## <a name="relationships"></a><span data-ttu-id="dbd0f-139">Relações</span><span class="sxs-lookup"><span data-stu-id="dbd0f-139">Relationships</span></span>
<span data-ttu-id="dbd0f-140">Nenhum</span><span class="sxs-lookup"><span data-stu-id="dbd0f-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dbd0f-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="dbd0f-141">JSON Representation</span></span>
<span data-ttu-id="dbd0f-142">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="dbd0f-142">Here is a JSON representation of the resource.</span></span>
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



