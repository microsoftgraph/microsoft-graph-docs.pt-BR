---
title: Tipo de recurso locateDeviceActionResult
description: Resultado da ação de localização do dispositivo
author: tfitzmac
ms.openlocfilehash: 82f8b5ba1bd1f1ce1584af50a4a2b3037e588adc
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27345448"
---
# <a name="locatedeviceactionresult-resource-type"></a><span data-ttu-id="4665b-103">Tipo de recurso locateDeviceActionResult</span><span class="sxs-lookup"><span data-stu-id="4665b-103">locateDeviceActionResult resource type</span></span>

> <span data-ttu-id="4665b-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="4665b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4665b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="4665b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4665b-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="4665b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4665b-107">Resultado da ação de localização do dispositivo</span><span class="sxs-lookup"><span data-stu-id="4665b-107">Locate device action result</span></span>

<span data-ttu-id="4665b-108">Herda de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="4665b-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4665b-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4665b-109">Properties</span></span>
|<span data-ttu-id="4665b-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4665b-110">Property</span></span>|<span data-ttu-id="4665b-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="4665b-111">Type</span></span>|<span data-ttu-id="4665b-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="4665b-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4665b-113">actionName</span><span class="sxs-lookup"><span data-stu-id="4665b-113">actionName</span></span>|<span data-ttu-id="4665b-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4665b-114">String</span></span>|<span data-ttu-id="4665b-115">Nome da ação herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="4665b-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="4665b-116">actionState</span><span class="sxs-lookup"><span data-stu-id="4665b-116">actionState</span></span>|[<span data-ttu-id="4665b-117">actionState</span><span class="sxs-lookup"><span data-stu-id="4665b-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="4665b-118">Estado da ação Inherited de [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="4665b-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="4665b-119">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="4665b-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="4665b-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="4665b-120">startDateTime</span></span>|<span data-ttu-id="4665b-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4665b-121">DateTimeOffset</span></span>|<span data-ttu-id="4665b-122">Hora em que ação foi iniciada, herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="4665b-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="4665b-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="4665b-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="4665b-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4665b-124">DateTimeOffset</span></span>|<span data-ttu-id="4665b-125">Hora da última atualização do estado da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="4665b-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="4665b-126">deviceLocation</span><span class="sxs-lookup"><span data-stu-id="4665b-126">deviceLocation</span></span>|[<span data-ttu-id="4665b-127">deviceGeoLocation</span><span class="sxs-lookup"><span data-stu-id="4665b-127">deviceGeoLocation</span></span>](../resources/intune-devices-devicegeolocation.md)|<span data-ttu-id="4665b-128">local do dispositivo</span><span class="sxs-lookup"><span data-stu-id="4665b-128">device location</span></span>|

## <a name="relationships"></a><span data-ttu-id="4665b-129">Relações</span><span class="sxs-lookup"><span data-stu-id="4665b-129">Relationships</span></span>
<span data-ttu-id="4665b-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4665b-130">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4665b-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4665b-131">JSON Representation</span></span>
<span data-ttu-id="4665b-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4665b-132">Here is a JSON representation of the resource.</span></span>
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





