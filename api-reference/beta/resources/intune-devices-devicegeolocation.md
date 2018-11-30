---
title: Tipo de recurso deviceGeoLocation
description: Localização do dispositivo
ms.openlocfilehash: 2ab7f777d00b891ceb7aae127ac87868aec582cc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034722"
---
# <a name="devicegeolocation-resource-type"></a><span data-ttu-id="6d53b-103">Tipo de recurso deviceGeoLocation</span><span class="sxs-lookup"><span data-stu-id="6d53b-103">deviceGeoLocation resource type</span></span>

> <span data-ttu-id="6d53b-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="6d53b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6d53b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="6d53b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6d53b-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="6d53b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6d53b-107">Localização do dispositivo</span><span class="sxs-lookup"><span data-stu-id="6d53b-107">Device location</span></span>
## <a name="properties"></a><span data-ttu-id="6d53b-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6d53b-108">Properties</span></span>
|<span data-ttu-id="6d53b-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6d53b-109">Property</span></span>|<span data-ttu-id="6d53b-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="6d53b-110">Type</span></span>|<span data-ttu-id="6d53b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="6d53b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6d53b-112">lastCollectedDateTimeUtc</span><span class="sxs-lookup"><span data-stu-id="6d53b-112">lastCollectedDateTimeUtc</span></span>|<span data-ttu-id="6d53b-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6d53b-113">DateTimeOffset</span></span>|<span data-ttu-id="6d53b-114">Hora em que a localização foi registrada, em relação ao UTC</span><span class="sxs-lookup"><span data-stu-id="6d53b-114">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="6d53b-115">lastCollectedDateTime</span><span class="sxs-lookup"><span data-stu-id="6d53b-115">lastCollectedDateTime</span></span>|<span data-ttu-id="6d53b-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6d53b-116">DateTimeOffset</span></span>|<span data-ttu-id="6d53b-117">Hora em que a localização foi registrada, em relação ao UTC</span><span class="sxs-lookup"><span data-stu-id="6d53b-117">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="6d53b-118">longitude</span><span class="sxs-lookup"><span data-stu-id="6d53b-118">longitude</span></span>|<span data-ttu-id="6d53b-119">Double</span><span class="sxs-lookup"><span data-stu-id="6d53b-119">Double</span></span>|<span data-ttu-id="6d53b-120">Coordenada de longitude da localização do dispositivo</span><span class="sxs-lookup"><span data-stu-id="6d53b-120">Longitude coordinate of the device's location</span></span>|
|<span data-ttu-id="6d53b-121">latitude</span><span class="sxs-lookup"><span data-stu-id="6d53b-121">latitude</span></span>|<span data-ttu-id="6d53b-122">Double</span><span class="sxs-lookup"><span data-stu-id="6d53b-122">Double</span></span>|<span data-ttu-id="6d53b-123">Coordenada de latitude da localização do dispositivo</span><span class="sxs-lookup"><span data-stu-id="6d53b-123">Latitude coordinate of the device's location</span></span>|
|<span data-ttu-id="6d53b-124">altitude</span><span class="sxs-lookup"><span data-stu-id="6d53b-124">altitude</span></span>|<span data-ttu-id="6d53b-125">Double</span><span class="sxs-lookup"><span data-stu-id="6d53b-125">Double</span></span>|<span data-ttu-id="6d53b-126">Altitude, especificada em metros acima do nível do mar</span><span class="sxs-lookup"><span data-stu-id="6d53b-126">Altitude, given in meters above sea level</span></span>|
|<span data-ttu-id="6d53b-127">horizontalAccuracy</span><span class="sxs-lookup"><span data-stu-id="6d53b-127">horizontalAccuracy</span></span>|<span data-ttu-id="6d53b-128">Double</span><span class="sxs-lookup"><span data-stu-id="6d53b-128">Double</span></span>|<span data-ttu-id="6d53b-129">Precisão da latitude e da longitude em metros</span><span class="sxs-lookup"><span data-stu-id="6d53b-129">Accuracy of longitude and latitude in meters</span></span>|
|<span data-ttu-id="6d53b-130">verticalAccuracy</span><span class="sxs-lookup"><span data-stu-id="6d53b-130">verticalAccuracy</span></span>|<span data-ttu-id="6d53b-131">Double</span><span class="sxs-lookup"><span data-stu-id="6d53b-131">Double</span></span>|<span data-ttu-id="6d53b-132">Precisão da altitude em metros</span><span class="sxs-lookup"><span data-stu-id="6d53b-132">Accuracy of altitude in meters</span></span>|
|<span data-ttu-id="6d53b-133">heading</span><span class="sxs-lookup"><span data-stu-id="6d53b-133">heading</span></span>|<span data-ttu-id="6d53b-134">Double</span><span class="sxs-lookup"><span data-stu-id="6d53b-134">Double</span></span>|<span data-ttu-id="6d53b-135">Direção em graus do norte verdadeiro</span><span class="sxs-lookup"><span data-stu-id="6d53b-135">Heading in degrees from true north</span></span>|
|<span data-ttu-id="6d53b-136">speed</span><span class="sxs-lookup"><span data-stu-id="6d53b-136">speed</span></span>|<span data-ttu-id="6d53b-137">Double</span><span class="sxs-lookup"><span data-stu-id="6d53b-137">Double</span></span>|<span data-ttu-id="6d53b-138">Velocidade na qual o dispositivo está viajando, em metros por segundo</span><span class="sxs-lookup"><span data-stu-id="6d53b-138">Speed the device is traveling in meters per second</span></span>|

## <a name="relationships"></a><span data-ttu-id="6d53b-139">Relações</span><span class="sxs-lookup"><span data-stu-id="6d53b-139">Relationships</span></span>
<span data-ttu-id="6d53b-140">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6d53b-140">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6d53b-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6d53b-141">JSON Representation</span></span>
<span data-ttu-id="6d53b-142">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6d53b-142">Here is a JSON representation of the resource.</span></span>
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





