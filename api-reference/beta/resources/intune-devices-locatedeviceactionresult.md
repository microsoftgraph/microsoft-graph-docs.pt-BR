---
title: Tipo de recurso locateDeviceActionResult
description: Resultado da ação de localização do dispositivo
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f342f26916b1144a317d02871364e25da2d8c4d7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912453"
---
# <a name="locatedeviceactionresult-resource-type"></a><span data-ttu-id="a4aac-103">Tipo de recurso locateDeviceActionResult</span><span class="sxs-lookup"><span data-stu-id="a4aac-103">locateDeviceActionResult resource type</span></span>

> <span data-ttu-id="a4aac-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a4aac-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a4aac-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a4aac-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a4aac-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="a4aac-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a4aac-107">Resultado da ação de localização do dispositivo</span><span class="sxs-lookup"><span data-stu-id="a4aac-107">Locate device action result</span></span>

<span data-ttu-id="a4aac-108">Herda de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="a4aac-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a4aac-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a4aac-109">Properties</span></span>
|<span data-ttu-id="a4aac-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a4aac-110">Property</span></span>|<span data-ttu-id="a4aac-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="a4aac-111">Type</span></span>|<span data-ttu-id="a4aac-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="a4aac-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a4aac-113">actionName</span><span class="sxs-lookup"><span data-stu-id="a4aac-113">actionName</span></span>|<span data-ttu-id="a4aac-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a4aac-114">String</span></span>|<span data-ttu-id="a4aac-115">Nome da ação herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="a4aac-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="a4aac-116">actionState</span><span class="sxs-lookup"><span data-stu-id="a4aac-116">actionState</span></span>|[<span data-ttu-id="a4aac-117">actionState</span><span class="sxs-lookup"><span data-stu-id="a4aac-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="a4aac-118">Estado da ação Inherited de [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="a4aac-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="a4aac-119">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="a4aac-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="a4aac-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="a4aac-120">startDateTime</span></span>|<span data-ttu-id="a4aac-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a4aac-121">DateTimeOffset</span></span>|<span data-ttu-id="a4aac-122">Hora em que ação foi iniciada, herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="a4aac-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="a4aac-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="a4aac-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="a4aac-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a4aac-124">DateTimeOffset</span></span>|<span data-ttu-id="a4aac-125">Hora da última atualização do estado da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="a4aac-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="a4aac-126">deviceLocation</span><span class="sxs-lookup"><span data-stu-id="a4aac-126">deviceLocation</span></span>|[<span data-ttu-id="a4aac-127">deviceGeoLocation</span><span class="sxs-lookup"><span data-stu-id="a4aac-127">deviceGeoLocation</span></span>](../resources/intune-devices-devicegeolocation.md)|<span data-ttu-id="a4aac-128">local do dispositivo</span><span class="sxs-lookup"><span data-stu-id="a4aac-128">device location</span></span>|

## <a name="relationships"></a><span data-ttu-id="a4aac-129">Relações</span><span class="sxs-lookup"><span data-stu-id="a4aac-129">Relationships</span></span>
<span data-ttu-id="a4aac-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a4aac-130">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a4aac-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a4aac-131">JSON Representation</span></span>
<span data-ttu-id="a4aac-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a4aac-132">Here is a JSON representation of the resource.</span></span>
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





