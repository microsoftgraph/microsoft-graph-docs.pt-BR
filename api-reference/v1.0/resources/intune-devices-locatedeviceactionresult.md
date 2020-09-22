---
title: Tipo de recurso locateDeviceActionResult
description: Resultado de ação de localizar dispositivo
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 98f61377675154034a4a839bdb990717f03d4c2c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48091135"
---
# <a name="locatedeviceactionresult-resource-type"></a><span data-ttu-id="bce60-103">Tipo de recurso locateDeviceActionResult</span><span class="sxs-lookup"><span data-stu-id="bce60-103">locateDeviceActionResult resource type</span></span>

<span data-ttu-id="bce60-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bce60-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bce60-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bce60-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bce60-106">Resultado da ação de localização do dispositivo</span><span class="sxs-lookup"><span data-stu-id="bce60-106">Locate device action result</span></span>


<span data-ttu-id="bce60-107">Herda de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="bce60-107">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="bce60-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bce60-108">Properties</span></span>
|<span data-ttu-id="bce60-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bce60-109">Property</span></span>|<span data-ttu-id="bce60-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="bce60-110">Type</span></span>|<span data-ttu-id="bce60-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="bce60-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bce60-112">actionName</span><span class="sxs-lookup"><span data-stu-id="bce60-112">actionName</span></span>|<span data-ttu-id="bce60-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bce60-113">String</span></span>|<span data-ttu-id="bce60-114">Nome da ação Herdado de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="bce60-114">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="bce60-115">actionState</span><span class="sxs-lookup"><span data-stu-id="bce60-115">actionState</span></span>|[<span data-ttu-id="bce60-116">actionState</span><span class="sxs-lookup"><span data-stu-id="bce60-116">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="bce60-117">Estado da ação herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="bce60-117">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="bce60-118">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="bce60-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="bce60-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="bce60-119">startDateTime</span></span>|<span data-ttu-id="bce60-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bce60-120">DateTimeOffset</span></span>|<span data-ttu-id="bce60-121">Hora de início da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="bce60-121">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="bce60-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="bce60-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="bce60-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bce60-123">DateTimeOffset</span></span>|<span data-ttu-id="bce60-124">Hora da última atualização do estado da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="bce60-124">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="bce60-125">deviceLocation</span><span class="sxs-lookup"><span data-stu-id="bce60-125">deviceLocation</span></span>|[<span data-ttu-id="bce60-126">deviceGeoLocation</span><span class="sxs-lookup"><span data-stu-id="bce60-126">deviceGeoLocation</span></span>](../resources/intune-devices-devicegeolocation.md)|<span data-ttu-id="bce60-127">local do dispositivo</span><span class="sxs-lookup"><span data-stu-id="bce60-127">device location</span></span>|

## <a name="relationships"></a><span data-ttu-id="bce60-128">Relações</span><span class="sxs-lookup"><span data-stu-id="bce60-128">Relationships</span></span>
<span data-ttu-id="bce60-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bce60-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bce60-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bce60-130">JSON Representation</span></span>
<span data-ttu-id="bce60-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bce60-131">Here is a JSON representation of the resource.</span></span>
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









