---
title: tipo de recurso rotateBitLockerKeysDeviceActionResult
description: Resultado da ação do dispositivo RotateBitLockerKeys
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 46b0f00f38e453edbd2e5214a1fe1e900a418639
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/09/2019
ms.locfileid: "38088242"
---
# <a name="rotatebitlockerkeysdeviceactionresult-resource-type"></a><span data-ttu-id="863f4-103">tipo de recurso rotateBitLockerKeysDeviceActionResult</span><span class="sxs-lookup"><span data-stu-id="863f4-103">rotateBitLockerKeysDeviceActionResult resource type</span></span>

> <span data-ttu-id="863f4-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="863f4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="863f4-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="863f4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="863f4-106">Resultado da ação do dispositivo RotateBitLockerKeys</span><span class="sxs-lookup"><span data-stu-id="863f4-106">RotateBitLockerKeys device action result</span></span>


<span data-ttu-id="863f4-107">Herda de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="863f4-107">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="863f4-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="863f4-108">Properties</span></span>
|<span data-ttu-id="863f4-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="863f4-109">Property</span></span>|<span data-ttu-id="863f4-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="863f4-110">Type</span></span>|<span data-ttu-id="863f4-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="863f4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="863f4-112">actionName</span><span class="sxs-lookup"><span data-stu-id="863f4-112">actionName</span></span>|<span data-ttu-id="863f4-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="863f4-113">String</span></span>|<span data-ttu-id="863f4-114">Nome da ação Herdado de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="863f4-114">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="863f4-115">actionState</span><span class="sxs-lookup"><span data-stu-id="863f4-115">actionState</span></span>|[<span data-ttu-id="863f4-116">actionState</span><span class="sxs-lookup"><span data-stu-id="863f4-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="863f4-117">Estado da ação herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="863f4-117">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="863f4-118">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="863f4-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="863f4-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="863f4-119">startDateTime</span></span>|<span data-ttu-id="863f4-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="863f4-120">DateTimeOffset</span></span>|<span data-ttu-id="863f4-121">Hora de início da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="863f4-121">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="863f4-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="863f4-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="863f4-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="863f4-123">DateTimeOffset</span></span>|<span data-ttu-id="863f4-124">Hora da última atualização do estado da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="863f4-124">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="863f4-125">errorCode</span><span class="sxs-lookup"><span data-stu-id="863f4-125">errorCode</span></span>|<span data-ttu-id="863f4-126">Int32</span><span class="sxs-lookup"><span data-stu-id="863f4-126">Int32</span></span>|<span data-ttu-id="863f4-127">Código de erro de ação RotateBitLockerKeys</span><span class="sxs-lookup"><span data-stu-id="863f4-127">RotateBitLockerKeys action error code</span></span>|

## <a name="relationships"></a><span data-ttu-id="863f4-128">Relações</span><span class="sxs-lookup"><span data-stu-id="863f4-128">Relationships</span></span>
<span data-ttu-id="863f4-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="863f4-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="863f4-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="863f4-130">JSON Representation</span></span>
<span data-ttu-id="863f4-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="863f4-131">Here is a JSON representation of the resource.</span></span>
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



