---
title: tipo de recurso rotateBitLockerKeysDeviceActionResult
description: Resultado da ação do dispositivo RotateBitLockerKeys
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7189a1c2a1d7de349aa6b92811428849d8f3ab62
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48081010"
---
# <a name="rotatebitlockerkeysdeviceactionresult-resource-type"></a><span data-ttu-id="ebbd8-103">tipo de recurso rotateBitLockerKeysDeviceActionResult</span><span class="sxs-lookup"><span data-stu-id="ebbd8-103">rotateBitLockerKeysDeviceActionResult resource type</span></span>

<span data-ttu-id="ebbd8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ebbd8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ebbd8-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ebbd8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ebbd8-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ebbd8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ebbd8-107">Resultado da ação do dispositivo RotateBitLockerKeys</span><span class="sxs-lookup"><span data-stu-id="ebbd8-107">RotateBitLockerKeys device action result</span></span>


<span data-ttu-id="ebbd8-108">Herda de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="ebbd8-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ebbd8-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ebbd8-109">Properties</span></span>
|<span data-ttu-id="ebbd8-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ebbd8-110">Property</span></span>|<span data-ttu-id="ebbd8-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="ebbd8-111">Type</span></span>|<span data-ttu-id="ebbd8-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="ebbd8-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ebbd8-113">actionName</span><span class="sxs-lookup"><span data-stu-id="ebbd8-113">actionName</span></span>|<span data-ttu-id="ebbd8-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ebbd8-114">String</span></span>|<span data-ttu-id="ebbd8-115">Nome da ação Herdado de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="ebbd8-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="ebbd8-116">actionState</span><span class="sxs-lookup"><span data-stu-id="ebbd8-116">actionState</span></span>|[<span data-ttu-id="ebbd8-117">actionState</span><span class="sxs-lookup"><span data-stu-id="ebbd8-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="ebbd8-118">Estado da ação herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="ebbd8-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="ebbd8-119">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="ebbd8-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="ebbd8-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="ebbd8-120">startDateTime</span></span>|<span data-ttu-id="ebbd8-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ebbd8-121">DateTimeOffset</span></span>|<span data-ttu-id="ebbd8-122">Hora de início da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="ebbd8-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="ebbd8-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="ebbd8-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="ebbd8-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ebbd8-124">DateTimeOffset</span></span>|<span data-ttu-id="ebbd8-125">Hora da última atualização do estado da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="ebbd8-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="ebbd8-126">errorCode</span><span class="sxs-lookup"><span data-stu-id="ebbd8-126">errorCode</span></span>|<span data-ttu-id="ebbd8-127">Int32</span><span class="sxs-lookup"><span data-stu-id="ebbd8-127">Int32</span></span>|<span data-ttu-id="ebbd8-128">Código de erro de ação RotateBitLockerKeys</span><span class="sxs-lookup"><span data-stu-id="ebbd8-128">RotateBitLockerKeys action error code</span></span>|

## <a name="relationships"></a><span data-ttu-id="ebbd8-129">Relações</span><span class="sxs-lookup"><span data-stu-id="ebbd8-129">Relationships</span></span>
<span data-ttu-id="ebbd8-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ebbd8-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ebbd8-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ebbd8-131">JSON Representation</span></span>
<span data-ttu-id="ebbd8-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ebbd8-132">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.rotateBitLockerKeysDeviceActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.rotateBitLockerKeysDeviceActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "errorCode": 1024
}
```






