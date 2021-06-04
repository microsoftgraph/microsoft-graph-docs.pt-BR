---
title: Tipo de recurso locateDeviceActionResult
description: Resultado de ação de localizar dispositivo
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0fc2fa997d56fffd673964a1d387b175bfef2ba1
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754557"
---
# <a name="locatedeviceactionresult-resource-type"></a><span data-ttu-id="3bc66-103">Tipo de recurso locateDeviceActionResult</span><span class="sxs-lookup"><span data-stu-id="3bc66-103">locateDeviceActionResult resource type</span></span>

<span data-ttu-id="3bc66-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3bc66-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3bc66-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3bc66-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3bc66-106">Resultado da ação de localização do dispositivo</span><span class="sxs-lookup"><span data-stu-id="3bc66-106">Locate device action result</span></span>


<span data-ttu-id="3bc66-107">Herda de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="3bc66-107">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="3bc66-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3bc66-108">Properties</span></span>
|<span data-ttu-id="3bc66-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3bc66-109">Property</span></span>|<span data-ttu-id="3bc66-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="3bc66-110">Type</span></span>|<span data-ttu-id="3bc66-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="3bc66-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3bc66-112">actionName</span><span class="sxs-lookup"><span data-stu-id="3bc66-112">actionName</span></span>|<span data-ttu-id="3bc66-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3bc66-113">String</span></span>|<span data-ttu-id="3bc66-114">Nome da ação Herdado de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="3bc66-114">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="3bc66-115">actionState</span><span class="sxs-lookup"><span data-stu-id="3bc66-115">actionState</span></span>|[<span data-ttu-id="3bc66-116">actionState</span><span class="sxs-lookup"><span data-stu-id="3bc66-116">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="3bc66-117">Estado da ação Herdado de [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="3bc66-117">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="3bc66-118">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="3bc66-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="3bc66-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="3bc66-119">startDateTime</span></span>|<span data-ttu-id="3bc66-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3bc66-120">DateTimeOffset</span></span>|<span data-ttu-id="3bc66-121">Hora de início da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="3bc66-121">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="3bc66-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="3bc66-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="3bc66-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3bc66-123">DateTimeOffset</span></span>|<span data-ttu-id="3bc66-124">Hora da última atualização do estado da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="3bc66-124">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="3bc66-125">deviceLocation</span><span class="sxs-lookup"><span data-stu-id="3bc66-125">deviceLocation</span></span>|[<span data-ttu-id="3bc66-126">deviceGeoLocation</span><span class="sxs-lookup"><span data-stu-id="3bc66-126">deviceGeoLocation</span></span>](../resources/intune-devices-devicegeolocation.md)|<span data-ttu-id="3bc66-127">local do dispositivo</span><span class="sxs-lookup"><span data-stu-id="3bc66-127">device location</span></span>|

## <a name="relationships"></a><span data-ttu-id="3bc66-128">Relações</span><span class="sxs-lookup"><span data-stu-id="3bc66-128">Relationships</span></span>
<span data-ttu-id="3bc66-129">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="3bc66-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3bc66-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3bc66-130">JSON Representation</span></span>
<span data-ttu-id="3bc66-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3bc66-131">Here is a JSON representation of the resource.</span></span>
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
    "longitude": "4.2",
    "latitude": "4.2",
    "altitude": "4.2",
    "horizontalAccuracy": "4.2",
    "verticalAccuracy": "4.2",
    "heading": "4.2",
    "speed": "4.2"
  }
}
```




