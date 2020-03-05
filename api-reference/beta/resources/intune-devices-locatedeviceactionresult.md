---
title: Tipo de recurso locateDeviceActionResult
description: Resultado de ação de localizar dispositivo
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 112e1102f21c193ad2c09e1326017f5c3aed776c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528553"
---
# <a name="locatedeviceactionresult-resource-type"></a><span data-ttu-id="681ca-103">Tipo de recurso locateDeviceActionResult</span><span class="sxs-lookup"><span data-stu-id="681ca-103">locateDeviceActionResult resource type</span></span>

<span data-ttu-id="681ca-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="681ca-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="681ca-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="681ca-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="681ca-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="681ca-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="681ca-107">Resultado da ação de localização do dispositivo</span><span class="sxs-lookup"><span data-stu-id="681ca-107">Locate device action result</span></span>


<span data-ttu-id="681ca-108">Herda de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="681ca-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="681ca-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="681ca-109">Properties</span></span>
|<span data-ttu-id="681ca-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="681ca-110">Property</span></span>|<span data-ttu-id="681ca-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="681ca-111">Type</span></span>|<span data-ttu-id="681ca-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="681ca-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="681ca-113">actionName</span><span class="sxs-lookup"><span data-stu-id="681ca-113">actionName</span></span>|<span data-ttu-id="681ca-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="681ca-114">String</span></span>|<span data-ttu-id="681ca-115">Nome da ação Herdado de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="681ca-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="681ca-116">actionState</span><span class="sxs-lookup"><span data-stu-id="681ca-116">actionState</span></span>|[<span data-ttu-id="681ca-117">actionState</span><span class="sxs-lookup"><span data-stu-id="681ca-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="681ca-118">Estado da ação herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="681ca-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="681ca-119">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="681ca-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="681ca-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="681ca-120">startDateTime</span></span>|<span data-ttu-id="681ca-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="681ca-121">DateTimeOffset</span></span>|<span data-ttu-id="681ca-122">Hora de início da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="681ca-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="681ca-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="681ca-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="681ca-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="681ca-124">DateTimeOffset</span></span>|<span data-ttu-id="681ca-125">Hora da última atualização do estado da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="681ca-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="681ca-126">deviceLocation</span><span class="sxs-lookup"><span data-stu-id="681ca-126">deviceLocation</span></span>|[<span data-ttu-id="681ca-127">deviceGeoLocation</span><span class="sxs-lookup"><span data-stu-id="681ca-127">deviceGeoLocation</span></span>](../resources/intune-devices-devicegeolocation.md)|<span data-ttu-id="681ca-128">local do dispositivo</span><span class="sxs-lookup"><span data-stu-id="681ca-128">device location</span></span>|

## <a name="relationships"></a><span data-ttu-id="681ca-129">Relações</span><span class="sxs-lookup"><span data-stu-id="681ca-129">Relationships</span></span>
<span data-ttu-id="681ca-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="681ca-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="681ca-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="681ca-131">JSON Representation</span></span>
<span data-ttu-id="681ca-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="681ca-132">Here is a JSON representation of the resource.</span></span>
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



