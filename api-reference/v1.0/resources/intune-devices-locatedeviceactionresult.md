---
title: Tipo de recurso locateDeviceActionResult
description: Resultado da ação de localização do dispositivo
ms.openlocfilehash: 3cabeca1ac07dd1911cf4c60300d07bdc1266134
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27005146"
---
# <a name="locatedeviceactionresult-resource-type"></a><span data-ttu-id="09526-103">Tipo de recurso locateDeviceActionResult</span><span class="sxs-lookup"><span data-stu-id="09526-103">locateDeviceActionResult resource type</span></span>

> <span data-ttu-id="09526-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="09526-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="09526-105">Resultado da ação de localização do dispositivo</span><span class="sxs-lookup"><span data-stu-id="09526-105">Locate device action result</span></span>

<span data-ttu-id="09526-106">Herda de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="09526-106">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="09526-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="09526-107">Properties</span></span>
|<span data-ttu-id="09526-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="09526-108">Property</span></span>|<span data-ttu-id="09526-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="09526-109">Type</span></span>|<span data-ttu-id="09526-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="09526-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="09526-111">actionName</span><span class="sxs-lookup"><span data-stu-id="09526-111">actionName</span></span>|<span data-ttu-id="09526-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="09526-112">String</span></span>|<span data-ttu-id="09526-113">Nome da ação herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="09526-113">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="09526-114">actionState</span><span class="sxs-lookup"><span data-stu-id="09526-114">actionState</span></span>|[<span data-ttu-id="09526-115">actionState</span><span class="sxs-lookup"><span data-stu-id="09526-115">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="09526-116">Estado da ação Inherited de [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="09526-116">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="09526-117">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="09526-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="09526-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="09526-118">startDateTime</span></span>|<span data-ttu-id="09526-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="09526-119">DateTimeOffset</span></span>|<span data-ttu-id="09526-120">Hora em que ação foi iniciada, herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="09526-120">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="09526-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="09526-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="09526-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="09526-122">DateTimeOffset</span></span>|<span data-ttu-id="09526-123">Hora da última atualização do estado da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="09526-123">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="09526-124">deviceLocation</span><span class="sxs-lookup"><span data-stu-id="09526-124">deviceLocation</span></span>|[<span data-ttu-id="09526-125">deviceGeoLocation</span><span class="sxs-lookup"><span data-stu-id="09526-125">deviceGeoLocation</span></span>](../resources/intune-devices-devicegeolocation.md)|<span data-ttu-id="09526-126">local do dispositivo</span><span class="sxs-lookup"><span data-stu-id="09526-126">device location</span></span>|

## <a name="relationships"></a><span data-ttu-id="09526-127">Relações</span><span class="sxs-lookup"><span data-stu-id="09526-127">Relationships</span></span>
<span data-ttu-id="09526-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="09526-128">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="09526-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="09526-129">JSON Representation</span></span>
<span data-ttu-id="09526-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="09526-130">Here is a JSON representation of the resource.</span></span>
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



