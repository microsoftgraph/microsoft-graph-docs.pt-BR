---
title: Tipo de recurso locateDeviceActionResult
description: Resultado da ação de localização do dispositivo
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 682b2267369a80b3d2cb37d17dd1b2aafdef1f63
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29416885"
---
# <a name="locatedeviceactionresult-resource-type"></a><span data-ttu-id="f7ad3-103">Tipo de recurso locateDeviceActionResult</span><span class="sxs-lookup"><span data-stu-id="f7ad3-103">locateDeviceActionResult resource type</span></span>

> <span data-ttu-id="f7ad3-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="f7ad3-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f7ad3-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f7ad3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f7ad3-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="f7ad3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f7ad3-107">Resultado da ação de localização do dispositivo</span><span class="sxs-lookup"><span data-stu-id="f7ad3-107">Locate device action result</span></span>


<span data-ttu-id="f7ad3-108">Herda de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="f7ad3-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f7ad3-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f7ad3-109">Properties</span></span>
|<span data-ttu-id="f7ad3-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f7ad3-110">Property</span></span>|<span data-ttu-id="f7ad3-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="f7ad3-111">Type</span></span>|<span data-ttu-id="f7ad3-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="f7ad3-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f7ad3-113">actionName</span><span class="sxs-lookup"><span data-stu-id="f7ad3-113">actionName</span></span>|<span data-ttu-id="f7ad3-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f7ad3-114">String</span></span>|<span data-ttu-id="f7ad3-115">Nome da ação herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="f7ad3-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="f7ad3-116">actionState</span><span class="sxs-lookup"><span data-stu-id="f7ad3-116">actionState</span></span>|[<span data-ttu-id="f7ad3-117">actionState</span><span class="sxs-lookup"><span data-stu-id="f7ad3-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="f7ad3-118">Estado da ação Inherited de [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="f7ad3-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="f7ad3-119">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="f7ad3-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="f7ad3-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="f7ad3-120">startDateTime</span></span>|<span data-ttu-id="f7ad3-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f7ad3-121">DateTimeOffset</span></span>|<span data-ttu-id="f7ad3-122">Hora em que ação foi iniciada, herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="f7ad3-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="f7ad3-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="f7ad3-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="f7ad3-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f7ad3-124">DateTimeOffset</span></span>|<span data-ttu-id="f7ad3-125">Hora da última atualização do estado da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="f7ad3-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="f7ad3-126">deviceLocation</span><span class="sxs-lookup"><span data-stu-id="f7ad3-126">deviceLocation</span></span>|[<span data-ttu-id="f7ad3-127">deviceGeoLocation</span><span class="sxs-lookup"><span data-stu-id="f7ad3-127">deviceGeoLocation</span></span>](../resources/intune-devices-devicegeolocation.md)|<span data-ttu-id="f7ad3-128">local do dispositivo</span><span class="sxs-lookup"><span data-stu-id="f7ad3-128">device location</span></span>|

## <a name="relationships"></a><span data-ttu-id="f7ad3-129">Relações</span><span class="sxs-lookup"><span data-stu-id="f7ad3-129">Relationships</span></span>
<span data-ttu-id="f7ad3-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f7ad3-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f7ad3-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f7ad3-131">JSON Representation</span></span>
<span data-ttu-id="f7ad3-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f7ad3-132">Here is a JSON representation of the resource.</span></span>
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




