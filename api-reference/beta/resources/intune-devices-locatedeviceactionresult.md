---
title: Tipo de recurso locateDeviceActionResult
description: Resultado de ação de localizar dispositivo
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e7f32d1eb4a47e86f072d17e2e3bcf81160f835b
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/07/2021
ms.locfileid: "51612060"
---
# <a name="locatedeviceactionresult-resource-type"></a><span data-ttu-id="8eb76-103">Tipo de recurso locateDeviceActionResult</span><span class="sxs-lookup"><span data-stu-id="8eb76-103">locateDeviceActionResult resource type</span></span>

<span data-ttu-id="8eb76-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8eb76-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8eb76-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8eb76-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8eb76-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8eb76-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8eb76-107">Resultado da ação de localização do dispositivo</span><span class="sxs-lookup"><span data-stu-id="8eb76-107">Locate device action result</span></span>


<span data-ttu-id="8eb76-108">Herda de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="8eb76-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8eb76-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8eb76-109">Properties</span></span>
|<span data-ttu-id="8eb76-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8eb76-110">Property</span></span>|<span data-ttu-id="8eb76-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="8eb76-111">Type</span></span>|<span data-ttu-id="8eb76-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="8eb76-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8eb76-113">actionName</span><span class="sxs-lookup"><span data-stu-id="8eb76-113">actionName</span></span>|<span data-ttu-id="8eb76-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8eb76-114">String</span></span>|<span data-ttu-id="8eb76-115">Nome da ação Herdado de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="8eb76-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="8eb76-116">actionState</span><span class="sxs-lookup"><span data-stu-id="8eb76-116">actionState</span></span>|[<span data-ttu-id="8eb76-117">actionState</span><span class="sxs-lookup"><span data-stu-id="8eb76-117">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="8eb76-118">Estado da ação Herdado de [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="8eb76-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="8eb76-119">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="8eb76-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="8eb76-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="8eb76-120">startDateTime</span></span>|<span data-ttu-id="8eb76-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8eb76-121">DateTimeOffset</span></span>|<span data-ttu-id="8eb76-122">Hora de início da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="8eb76-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="8eb76-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="8eb76-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="8eb76-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8eb76-124">DateTimeOffset</span></span>|<span data-ttu-id="8eb76-125">Hora da última atualização do estado da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="8eb76-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="8eb76-126">deviceLocation</span><span class="sxs-lookup"><span data-stu-id="8eb76-126">deviceLocation</span></span>|[<span data-ttu-id="8eb76-127">deviceGeoLocation</span><span class="sxs-lookup"><span data-stu-id="8eb76-127">deviceGeoLocation</span></span>](../resources/intune-devices-devicegeolocation.md)|<span data-ttu-id="8eb76-128">local do dispositivo</span><span class="sxs-lookup"><span data-stu-id="8eb76-128">device location</span></span>|

## <a name="relationships"></a><span data-ttu-id="8eb76-129">Relações</span><span class="sxs-lookup"><span data-stu-id="8eb76-129">Relationships</span></span>
<span data-ttu-id="8eb76-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8eb76-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8eb76-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8eb76-131">JSON Representation</span></span>
<span data-ttu-id="8eb76-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8eb76-132">Here is a JSON representation of the resource.</span></span>
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




