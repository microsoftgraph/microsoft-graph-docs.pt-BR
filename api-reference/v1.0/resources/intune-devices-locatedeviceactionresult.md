---
title: Tipo de recurso locateDeviceActionResult
description: Resultado de ação de localizar dispositivo
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c335ac49bcf053e58381f7c1111caf5ae70cb0fd
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30255350"
---
# <a name="locatedeviceactionresult-resource-type"></a><span data-ttu-id="ce60b-103">Tipo de recurso locateDeviceActionResult</span><span class="sxs-lookup"><span data-stu-id="ce60b-103">locateDeviceActionResult resource type</span></span>

> <span data-ttu-id="ce60b-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ce60b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ce60b-105">Resultado da ação de localização do dispositivo</span><span class="sxs-lookup"><span data-stu-id="ce60b-105">Locate device action result</span></span>


<span data-ttu-id="ce60b-106">Herda de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="ce60b-106">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ce60b-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ce60b-107">Properties</span></span>
|<span data-ttu-id="ce60b-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ce60b-108">Property</span></span>|<span data-ttu-id="ce60b-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="ce60b-109">Type</span></span>|<span data-ttu-id="ce60b-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="ce60b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ce60b-111">actionName</span><span class="sxs-lookup"><span data-stu-id="ce60b-111">actionName</span></span>|<span data-ttu-id="ce60b-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ce60b-112">String</span></span>|<span data-ttu-id="ce60b-113">Nome da ação herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="ce60b-113">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="ce60b-114">actionState</span><span class="sxs-lookup"><span data-stu-id="ce60b-114">actionState</span></span>|[<span data-ttu-id="ce60b-115">actionState</span><span class="sxs-lookup"><span data-stu-id="ce60b-115">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="ce60b-116">Estado da ação herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="ce60b-116">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="ce60b-117">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="ce60b-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="ce60b-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="ce60b-118">startDateTime</span></span>|<span data-ttu-id="ce60b-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ce60b-119">DateTimeOffset</span></span>|<span data-ttu-id="ce60b-120">Hora em que ação foi iniciada, herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="ce60b-120">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="ce60b-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="ce60b-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="ce60b-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ce60b-122">DateTimeOffset</span></span>|<span data-ttu-id="ce60b-123">Hora da última atualização do estado da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="ce60b-123">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="ce60b-124">deviceLocation</span><span class="sxs-lookup"><span data-stu-id="ce60b-124">deviceLocation</span></span>|[<span data-ttu-id="ce60b-125">deviceGeoLocation</span><span class="sxs-lookup"><span data-stu-id="ce60b-125">deviceGeoLocation</span></span>](../resources/intune-devices-devicegeolocation.md)|<span data-ttu-id="ce60b-126">local do dispositivo</span><span class="sxs-lookup"><span data-stu-id="ce60b-126">device location</span></span>|

## <a name="relationships"></a><span data-ttu-id="ce60b-127">Relações</span><span class="sxs-lookup"><span data-stu-id="ce60b-127">Relationships</span></span>
<span data-ttu-id="ce60b-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ce60b-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ce60b-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ce60b-129">JSON Representation</span></span>
<span data-ttu-id="ce60b-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ce60b-130">Here is a JSON representation of the resource.</span></span>
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



