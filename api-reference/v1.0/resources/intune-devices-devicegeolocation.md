---
title: Tipo de recurso deviceGeoLocation
description: Localização do dispositivo
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 48c0b4224225c70a9f5c4a636e1e15e4ddea3364
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533292"
---
# <a name="devicegeolocation-resource-type"></a><span data-ttu-id="66bc8-103">Tipo de recurso deviceGeoLocation</span><span class="sxs-lookup"><span data-stu-id="66bc8-103">deviceGeoLocation resource type</span></span>

<span data-ttu-id="66bc8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="66bc8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="66bc8-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="66bc8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="66bc8-106">Localização do dispositivo</span><span class="sxs-lookup"><span data-stu-id="66bc8-106">Device location</span></span>

## <a name="properties"></a><span data-ttu-id="66bc8-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="66bc8-107">Properties</span></span>
|<span data-ttu-id="66bc8-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="66bc8-108">Property</span></span>|<span data-ttu-id="66bc8-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="66bc8-109">Type</span></span>|<span data-ttu-id="66bc8-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="66bc8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66bc8-111">lastCollectedDateTime</span><span class="sxs-lookup"><span data-stu-id="66bc8-111">lastCollectedDateTime</span></span>|<span data-ttu-id="66bc8-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="66bc8-112">DateTimeOffset</span></span>|<span data-ttu-id="66bc8-113">Hora em que a localização foi registrada, em relação ao UTC</span><span class="sxs-lookup"><span data-stu-id="66bc8-113">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="66bc8-114">longitude</span><span class="sxs-lookup"><span data-stu-id="66bc8-114">longitude</span></span>|<span data-ttu-id="66bc8-115">Duplo</span><span class="sxs-lookup"><span data-stu-id="66bc8-115">Double</span></span>|<span data-ttu-id="66bc8-116">Coordenada de longitude da localização do dispositivo</span><span class="sxs-lookup"><span data-stu-id="66bc8-116">Longitude coordinate of the device's location</span></span>|
|<span data-ttu-id="66bc8-117">latitude</span><span class="sxs-lookup"><span data-stu-id="66bc8-117">latitude</span></span>|<span data-ttu-id="66bc8-118">Duplo</span><span class="sxs-lookup"><span data-stu-id="66bc8-118">Double</span></span>|<span data-ttu-id="66bc8-119">Coordenada de latitude da localização do dispositivo</span><span class="sxs-lookup"><span data-stu-id="66bc8-119">Latitude coordinate of the device's location</span></span>|
|<span data-ttu-id="66bc8-120">altitude</span><span class="sxs-lookup"><span data-stu-id="66bc8-120">altitude</span></span>|<span data-ttu-id="66bc8-121">Duplo</span><span class="sxs-lookup"><span data-stu-id="66bc8-121">Double</span></span>|<span data-ttu-id="66bc8-122">Altitude, especificada em metros acima do nível do mar</span><span class="sxs-lookup"><span data-stu-id="66bc8-122">Altitude, given in meters above sea level</span></span>|
|<span data-ttu-id="66bc8-123">horizontalAccuracy</span><span class="sxs-lookup"><span data-stu-id="66bc8-123">horizontalAccuracy</span></span>|<span data-ttu-id="66bc8-124">Duplo</span><span class="sxs-lookup"><span data-stu-id="66bc8-124">Double</span></span>|<span data-ttu-id="66bc8-125">Precisão da latitude e da longitude em metros</span><span class="sxs-lookup"><span data-stu-id="66bc8-125">Accuracy of longitude and latitude in meters</span></span>|
|<span data-ttu-id="66bc8-126">verticalAccuracy</span><span class="sxs-lookup"><span data-stu-id="66bc8-126">verticalAccuracy</span></span>|<span data-ttu-id="66bc8-127">Duplo</span><span class="sxs-lookup"><span data-stu-id="66bc8-127">Double</span></span>|<span data-ttu-id="66bc8-128">Precisão da altitude em metros</span><span class="sxs-lookup"><span data-stu-id="66bc8-128">Accuracy of altitude in meters</span></span>|
|<span data-ttu-id="66bc8-129">heading</span><span class="sxs-lookup"><span data-stu-id="66bc8-129">heading</span></span>|<span data-ttu-id="66bc8-130">Duplo</span><span class="sxs-lookup"><span data-stu-id="66bc8-130">Double</span></span>|<span data-ttu-id="66bc8-131">Direção em graus do norte verdadeiro</span><span class="sxs-lookup"><span data-stu-id="66bc8-131">Heading in degrees from true north</span></span>|
|<span data-ttu-id="66bc8-132">speed</span><span class="sxs-lookup"><span data-stu-id="66bc8-132">speed</span></span>|<span data-ttu-id="66bc8-133">Double</span><span class="sxs-lookup"><span data-stu-id="66bc8-133">Double</span></span>|<span data-ttu-id="66bc8-134">Velocidade na qual o dispositivo está viajando, em metros por segundo</span><span class="sxs-lookup"><span data-stu-id="66bc8-134">Speed the device is traveling in meters per second</span></span>|

## <a name="relationships"></a><span data-ttu-id="66bc8-135">Relações</span><span class="sxs-lookup"><span data-stu-id="66bc8-135">Relationships</span></span>
<span data-ttu-id="66bc8-136">Nenhum</span><span class="sxs-lookup"><span data-stu-id="66bc8-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="66bc8-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="66bc8-137">JSON Representation</span></span>
<span data-ttu-id="66bc8-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="66bc8-138">Here is a JSON representation of the resource.</span></span>
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




