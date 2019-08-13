---
title: Tipo de recurso locateDeviceActionResult
description: Resultado de ação de localizar dispositivo
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 41992c5b5b1cd4a620d3e2433524478a931b6c7f
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36372332"
---
# <a name="locatedeviceactionresult-resource-type"></a><span data-ttu-id="a7f49-103">Tipo de recurso locateDeviceActionResult</span><span class="sxs-lookup"><span data-stu-id="a7f49-103">locateDeviceActionResult resource type</span></span>

> <span data-ttu-id="a7f49-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a7f49-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a7f49-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a7f49-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a7f49-106">Resultado da ação de localização do dispositivo</span><span class="sxs-lookup"><span data-stu-id="a7f49-106">Locate device action result</span></span>


<span data-ttu-id="a7f49-107">Herda de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="a7f49-107">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a7f49-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a7f49-108">Properties</span></span>
|<span data-ttu-id="a7f49-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a7f49-109">Property</span></span>|<span data-ttu-id="a7f49-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="a7f49-110">Type</span></span>|<span data-ttu-id="a7f49-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="a7f49-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a7f49-112">actionName</span><span class="sxs-lookup"><span data-stu-id="a7f49-112">actionName</span></span>|<span data-ttu-id="a7f49-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a7f49-113">String</span></span>|<span data-ttu-id="a7f49-114">Nome da ação Herdado de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="a7f49-114">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="a7f49-115">actionState</span><span class="sxs-lookup"><span data-stu-id="a7f49-115">actionState</span></span>|[<span data-ttu-id="a7f49-116">actionState</span><span class="sxs-lookup"><span data-stu-id="a7f49-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="a7f49-117">Estado da ação herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="a7f49-117">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="a7f49-118">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="a7f49-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="a7f49-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="a7f49-119">startDateTime</span></span>|<span data-ttu-id="a7f49-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a7f49-120">DateTimeOffset</span></span>|<span data-ttu-id="a7f49-121">Hora de início da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="a7f49-121">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="a7f49-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="a7f49-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="a7f49-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a7f49-123">DateTimeOffset</span></span>|<span data-ttu-id="a7f49-124">Hora da última atualização do estado da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="a7f49-124">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="a7f49-125">deviceLocation</span><span class="sxs-lookup"><span data-stu-id="a7f49-125">deviceLocation</span></span>|[<span data-ttu-id="a7f49-126">deviceGeoLocation</span><span class="sxs-lookup"><span data-stu-id="a7f49-126">deviceGeoLocation</span></span>](../resources/intune-devices-devicegeolocation.md)|<span data-ttu-id="a7f49-127">local do dispositivo</span><span class="sxs-lookup"><span data-stu-id="a7f49-127">device location</span></span>|

## <a name="relationships"></a><span data-ttu-id="a7f49-128">Relações</span><span class="sxs-lookup"><span data-stu-id="a7f49-128">Relationships</span></span>
<span data-ttu-id="a7f49-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a7f49-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a7f49-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a7f49-130">JSON Representation</span></span>
<span data-ttu-id="a7f49-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a7f49-131">Here is a JSON representation of the resource.</span></span>
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



