---
title: Tipo de recurso deviceGeoLocation
description: Localização do dispositivo
author: tfitzmac
ms.openlocfilehash: b3e790809f79d8d943cc12cc0e5065972c9864ff
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27328627"
---
# <a name="devicegeolocation-resource-type"></a><span data-ttu-id="11798-103">Tipo de recurso deviceGeoLocation</span><span class="sxs-lookup"><span data-stu-id="11798-103">deviceGeoLocation resource type</span></span>

> <span data-ttu-id="11798-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="11798-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="11798-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="11798-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="11798-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="11798-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="11798-107">Localização do dispositivo</span><span class="sxs-lookup"><span data-stu-id="11798-107">Device location</span></span>
## <a name="properties"></a><span data-ttu-id="11798-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="11798-108">Properties</span></span>
|<span data-ttu-id="11798-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="11798-109">Property</span></span>|<span data-ttu-id="11798-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="11798-110">Type</span></span>|<span data-ttu-id="11798-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="11798-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11798-112">lastCollectedDateTimeUtc</span><span class="sxs-lookup"><span data-stu-id="11798-112">lastCollectedDateTimeUtc</span></span>|<span data-ttu-id="11798-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="11798-113">DateTimeOffset</span></span>|<span data-ttu-id="11798-114">Hora em que a localização foi registrada, em relação ao UTC</span><span class="sxs-lookup"><span data-stu-id="11798-114">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="11798-115">lastCollectedDateTime</span><span class="sxs-lookup"><span data-stu-id="11798-115">lastCollectedDateTime</span></span>|<span data-ttu-id="11798-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="11798-116">DateTimeOffset</span></span>|<span data-ttu-id="11798-117">Hora em que a localização foi registrada, em relação ao UTC</span><span class="sxs-lookup"><span data-stu-id="11798-117">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="11798-118">longitude</span><span class="sxs-lookup"><span data-stu-id="11798-118">longitude</span></span>|<span data-ttu-id="11798-119">Double</span><span class="sxs-lookup"><span data-stu-id="11798-119">Double</span></span>|<span data-ttu-id="11798-120">Coordenada de longitude da localização do dispositivo</span><span class="sxs-lookup"><span data-stu-id="11798-120">Longitude coordinate of the device's location</span></span>|
|<span data-ttu-id="11798-121">latitude</span><span class="sxs-lookup"><span data-stu-id="11798-121">latitude</span></span>|<span data-ttu-id="11798-122">Double</span><span class="sxs-lookup"><span data-stu-id="11798-122">Double</span></span>|<span data-ttu-id="11798-123">Coordenada de latitude da localização do dispositivo</span><span class="sxs-lookup"><span data-stu-id="11798-123">Latitude coordinate of the device's location</span></span>|
|<span data-ttu-id="11798-124">altitude</span><span class="sxs-lookup"><span data-stu-id="11798-124">altitude</span></span>|<span data-ttu-id="11798-125">Double</span><span class="sxs-lookup"><span data-stu-id="11798-125">Double</span></span>|<span data-ttu-id="11798-126">Altitude, especificada em metros acima do nível do mar</span><span class="sxs-lookup"><span data-stu-id="11798-126">Altitude, given in meters above sea level</span></span>|
|<span data-ttu-id="11798-127">horizontalAccuracy</span><span class="sxs-lookup"><span data-stu-id="11798-127">horizontalAccuracy</span></span>|<span data-ttu-id="11798-128">Double</span><span class="sxs-lookup"><span data-stu-id="11798-128">Double</span></span>|<span data-ttu-id="11798-129">Precisão da latitude e da longitude em metros</span><span class="sxs-lookup"><span data-stu-id="11798-129">Accuracy of longitude and latitude in meters</span></span>|
|<span data-ttu-id="11798-130">verticalAccuracy</span><span class="sxs-lookup"><span data-stu-id="11798-130">verticalAccuracy</span></span>|<span data-ttu-id="11798-131">Double</span><span class="sxs-lookup"><span data-stu-id="11798-131">Double</span></span>|<span data-ttu-id="11798-132">Precisão da altitude em metros</span><span class="sxs-lookup"><span data-stu-id="11798-132">Accuracy of altitude in meters</span></span>|
|<span data-ttu-id="11798-133">heading</span><span class="sxs-lookup"><span data-stu-id="11798-133">heading</span></span>|<span data-ttu-id="11798-134">Double</span><span class="sxs-lookup"><span data-stu-id="11798-134">Double</span></span>|<span data-ttu-id="11798-135">Direção em graus do norte verdadeiro</span><span class="sxs-lookup"><span data-stu-id="11798-135">Heading in degrees from true north</span></span>|
|<span data-ttu-id="11798-136">speed</span><span class="sxs-lookup"><span data-stu-id="11798-136">speed</span></span>|<span data-ttu-id="11798-137">Double</span><span class="sxs-lookup"><span data-stu-id="11798-137">Double</span></span>|<span data-ttu-id="11798-138">Velocidade na qual o dispositivo está viajando, em metros por segundo</span><span class="sxs-lookup"><span data-stu-id="11798-138">Speed the device is traveling in meters per second</span></span>|

## <a name="relationships"></a><span data-ttu-id="11798-139">Relações</span><span class="sxs-lookup"><span data-stu-id="11798-139">Relationships</span></span>
<span data-ttu-id="11798-140">Nenhum</span><span class="sxs-lookup"><span data-stu-id="11798-140">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="11798-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="11798-141">JSON Representation</span></span>
<span data-ttu-id="11798-142">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="11798-142">Here is a JSON representation of the resource.</span></span>
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





