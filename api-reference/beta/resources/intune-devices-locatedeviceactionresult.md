---
title: Tipo de recurso locateDeviceActionResult
description: Resultado de ação de localizar dispositivo
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c3dad81d0cb919c421c5dcaaa652a2eeaac788bf
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43470541"
---
# <a name="locatedeviceactionresult-resource-type"></a><span data-ttu-id="73db7-103">Tipo de recurso locateDeviceActionResult</span><span class="sxs-lookup"><span data-stu-id="73db7-103">locateDeviceActionResult resource type</span></span>

<span data-ttu-id="73db7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="73db7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="73db7-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="73db7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="73db7-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="73db7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="73db7-107">Resultado da ação de localização do dispositivo</span><span class="sxs-lookup"><span data-stu-id="73db7-107">Locate device action result</span></span>


<span data-ttu-id="73db7-108">Herda de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="73db7-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="73db7-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="73db7-109">Properties</span></span>
|<span data-ttu-id="73db7-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="73db7-110">Property</span></span>|<span data-ttu-id="73db7-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="73db7-111">Type</span></span>|<span data-ttu-id="73db7-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="73db7-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="73db7-113">actionName</span><span class="sxs-lookup"><span data-stu-id="73db7-113">actionName</span></span>|<span data-ttu-id="73db7-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="73db7-114">String</span></span>|<span data-ttu-id="73db7-115">Nome da ação Herdado de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="73db7-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="73db7-116">actionState</span><span class="sxs-lookup"><span data-stu-id="73db7-116">actionState</span></span>|[<span data-ttu-id="73db7-117">actionState</span><span class="sxs-lookup"><span data-stu-id="73db7-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="73db7-118">Estado da ação herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="73db7-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="73db7-119">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="73db7-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="73db7-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="73db7-120">startDateTime</span></span>|<span data-ttu-id="73db7-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="73db7-121">DateTimeOffset</span></span>|<span data-ttu-id="73db7-122">Hora de início da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="73db7-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="73db7-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="73db7-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="73db7-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="73db7-124">DateTimeOffset</span></span>|<span data-ttu-id="73db7-125">Hora da última atualização do estado da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="73db7-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="73db7-126">deviceLocation</span><span class="sxs-lookup"><span data-stu-id="73db7-126">deviceLocation</span></span>|[<span data-ttu-id="73db7-127">deviceGeoLocation</span><span class="sxs-lookup"><span data-stu-id="73db7-127">deviceGeoLocation</span></span>](../resources/intune-devices-devicegeolocation.md)|<span data-ttu-id="73db7-128">local do dispositivo</span><span class="sxs-lookup"><span data-stu-id="73db7-128">device location</span></span>|

## <a name="relationships"></a><span data-ttu-id="73db7-129">Relações</span><span class="sxs-lookup"><span data-stu-id="73db7-129">Relationships</span></span>
<span data-ttu-id="73db7-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="73db7-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="73db7-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="73db7-131">JSON Representation</span></span>
<span data-ttu-id="73db7-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="73db7-132">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.locateDeviceActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.locateDeviceActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "deviceLocation": {
    "@odata.type": "microsoft.graph.deviceGeoLocation",
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
}
```



