---
title: Tipo de recurso deviceGeoLocation
description: Localização do dispositivo
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 88802f3d4909f07ab96395efdf61ad7e817f4be8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36030811"
---
# <a name="devicegeolocation-resource-type"></a><span data-ttu-id="f27e3-103">Tipo de recurso deviceGeoLocation</span><span class="sxs-lookup"><span data-stu-id="f27e3-103">deviceGeoLocation resource type</span></span>

> <span data-ttu-id="f27e3-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f27e3-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f27e3-105">Localização do dispositivo</span><span class="sxs-lookup"><span data-stu-id="f27e3-105">Device location</span></span>

## <a name="properties"></a><span data-ttu-id="f27e3-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f27e3-106">Properties</span></span>
|<span data-ttu-id="f27e3-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f27e3-107">Property</span></span>|<span data-ttu-id="f27e3-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="f27e3-108">Type</span></span>|<span data-ttu-id="f27e3-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="f27e3-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f27e3-110">lastCollectedDateTime</span><span class="sxs-lookup"><span data-stu-id="f27e3-110">lastCollectedDateTime</span></span>|<span data-ttu-id="f27e3-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f27e3-111">DateTimeOffset</span></span>|<span data-ttu-id="f27e3-112">Hora em que a localização foi registrada, em relação ao UTC</span><span class="sxs-lookup"><span data-stu-id="f27e3-112">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="f27e3-113">longitude</span><span class="sxs-lookup"><span data-stu-id="f27e3-113">longitude</span></span>|<span data-ttu-id="f27e3-114">Duplo</span><span class="sxs-lookup"><span data-stu-id="f27e3-114">Double</span></span>|<span data-ttu-id="f27e3-115">Coordenada de longitude da localização do dispositivo</span><span class="sxs-lookup"><span data-stu-id="f27e3-115">Longitude coordinate of the device's location</span></span>|
|<span data-ttu-id="f27e3-116">latitude</span><span class="sxs-lookup"><span data-stu-id="f27e3-116">latitude</span></span>|<span data-ttu-id="f27e3-117">Duplo</span><span class="sxs-lookup"><span data-stu-id="f27e3-117">Double</span></span>|<span data-ttu-id="f27e3-118">Coordenada de latitude da localização do dispositivo</span><span class="sxs-lookup"><span data-stu-id="f27e3-118">Latitude coordinate of the device's location</span></span>|
|<span data-ttu-id="f27e3-119">altitude</span><span class="sxs-lookup"><span data-stu-id="f27e3-119">altitude</span></span>|<span data-ttu-id="f27e3-120">Duplo</span><span class="sxs-lookup"><span data-stu-id="f27e3-120">Double</span></span>|<span data-ttu-id="f27e3-121">Altitude, especificada em metros acima do nível do mar</span><span class="sxs-lookup"><span data-stu-id="f27e3-121">Altitude, given in meters above sea level</span></span>|
|<span data-ttu-id="f27e3-122">horizontalAccuracy</span><span class="sxs-lookup"><span data-stu-id="f27e3-122">horizontalAccuracy</span></span>|<span data-ttu-id="f27e3-123">Duplo</span><span class="sxs-lookup"><span data-stu-id="f27e3-123">Double</span></span>|<span data-ttu-id="f27e3-124">Precisão da latitude e da longitude em metros</span><span class="sxs-lookup"><span data-stu-id="f27e3-124">Accuracy of longitude and latitude in meters</span></span>|
|<span data-ttu-id="f27e3-125">verticalAccuracy</span><span class="sxs-lookup"><span data-stu-id="f27e3-125">verticalAccuracy</span></span>|<span data-ttu-id="f27e3-126">Duplo</span><span class="sxs-lookup"><span data-stu-id="f27e3-126">Double</span></span>|<span data-ttu-id="f27e3-127">Precisão da altitude em metros</span><span class="sxs-lookup"><span data-stu-id="f27e3-127">Accuracy of altitude in meters</span></span>|
|<span data-ttu-id="f27e3-128">heading</span><span class="sxs-lookup"><span data-stu-id="f27e3-128">heading</span></span>|<span data-ttu-id="f27e3-129">Duplo</span><span class="sxs-lookup"><span data-stu-id="f27e3-129">Double</span></span>|<span data-ttu-id="f27e3-130">Direção em graus do norte verdadeiro</span><span class="sxs-lookup"><span data-stu-id="f27e3-130">Heading in degrees from true north</span></span>|
|<span data-ttu-id="f27e3-131">speed</span><span class="sxs-lookup"><span data-stu-id="f27e3-131">speed</span></span>|<span data-ttu-id="f27e3-132">Double</span><span class="sxs-lookup"><span data-stu-id="f27e3-132">Double</span></span>|<span data-ttu-id="f27e3-133">Velocidade na qual o dispositivo está viajando, em metros por segundo</span><span class="sxs-lookup"><span data-stu-id="f27e3-133">Speed the device is traveling in meters per second</span></span>|

## <a name="relationships"></a><span data-ttu-id="f27e3-134">Relações</span><span class="sxs-lookup"><span data-stu-id="f27e3-134">Relationships</span></span>
<span data-ttu-id="f27e3-135">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f27e3-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f27e3-136">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f27e3-136">JSON Representation</span></span>
<span data-ttu-id="f27e3-137">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f27e3-137">Here is a JSON representation of the resource.</span></span>
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



