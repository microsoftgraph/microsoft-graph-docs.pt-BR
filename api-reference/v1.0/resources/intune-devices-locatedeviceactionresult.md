---
title: Tipo de recurso locateDeviceActionResult
description: Resultado de ação de localizar dispositivo
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c335ac49bcf053e58381f7c1111caf5ae70cb0fd
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32570359"
---
# <a name="locatedeviceactionresult-resource-type"></a><span data-ttu-id="5bb08-103">Tipo de recurso locateDeviceActionResult</span><span class="sxs-lookup"><span data-stu-id="5bb08-103">locateDeviceActionResult resource type</span></span>

> <span data-ttu-id="5bb08-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5bb08-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5bb08-105">Resultado da ação de localização do dispositivo</span><span class="sxs-lookup"><span data-stu-id="5bb08-105">Locate device action result</span></span>


<span data-ttu-id="5bb08-106">Herda de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="5bb08-106">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="5bb08-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5bb08-107">Properties</span></span>
|<span data-ttu-id="5bb08-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5bb08-108">Property</span></span>|<span data-ttu-id="5bb08-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="5bb08-109">Type</span></span>|<span data-ttu-id="5bb08-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="5bb08-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5bb08-111">actionName</span><span class="sxs-lookup"><span data-stu-id="5bb08-111">actionName</span></span>|<span data-ttu-id="5bb08-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5bb08-112">String</span></span>|<span data-ttu-id="5bb08-113">Nome da ação Herdado de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="5bb08-113">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="5bb08-114">actionState</span><span class="sxs-lookup"><span data-stu-id="5bb08-114">actionState</span></span>|[<span data-ttu-id="5bb08-115">actionState</span><span class="sxs-lookup"><span data-stu-id="5bb08-115">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="5bb08-116">Estado da ação herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="5bb08-116">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="5bb08-117">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="5bb08-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="5bb08-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="5bb08-118">startDateTime</span></span>|<span data-ttu-id="5bb08-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5bb08-119">DateTimeOffset</span></span>|<span data-ttu-id="5bb08-120">Hora de início da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="5bb08-120">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="5bb08-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="5bb08-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="5bb08-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5bb08-122">DateTimeOffset</span></span>|<span data-ttu-id="5bb08-123">Hora da última atualização do estado da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="5bb08-123">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="5bb08-124">deviceLocation</span><span class="sxs-lookup"><span data-stu-id="5bb08-124">deviceLocation</span></span>|[<span data-ttu-id="5bb08-125">deviceGeoLocation</span><span class="sxs-lookup"><span data-stu-id="5bb08-125">deviceGeoLocation</span></span>](../resources/intune-devices-devicegeolocation.md)|<span data-ttu-id="5bb08-126">local do dispositivo</span><span class="sxs-lookup"><span data-stu-id="5bb08-126">device location</span></span>|

## <a name="relationships"></a><span data-ttu-id="5bb08-127">Relações</span><span class="sxs-lookup"><span data-stu-id="5bb08-127">Relationships</span></span>
<span data-ttu-id="5bb08-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5bb08-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5bb08-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5bb08-129">JSON Representation</span></span>
<span data-ttu-id="5bb08-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5bb08-130">Here is a JSON representation of the resource.</span></span>
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



