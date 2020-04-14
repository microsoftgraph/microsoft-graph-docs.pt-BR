---
title: tipo de recurso rotateBitLockerKeysDeviceActionResult
description: Resultado da ação do dispositivo RotateBitLockerKeys
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 91f21809f7ba1ab0af27a969fb1646b571ea87ed
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43383077"
---
# <a name="rotatebitlockerkeysdeviceactionresult-resource-type"></a><span data-ttu-id="d0bd5-103">tipo de recurso rotateBitLockerKeysDeviceActionResult</span><span class="sxs-lookup"><span data-stu-id="d0bd5-103">rotateBitLockerKeysDeviceActionResult resource type</span></span>

<span data-ttu-id="d0bd5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d0bd5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d0bd5-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d0bd5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d0bd5-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d0bd5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d0bd5-107">Resultado da ação do dispositivo RotateBitLockerKeys</span><span class="sxs-lookup"><span data-stu-id="d0bd5-107">RotateBitLockerKeys device action result</span></span>


<span data-ttu-id="d0bd5-108">Herda de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="d0bd5-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d0bd5-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d0bd5-109">Properties</span></span>
|<span data-ttu-id="d0bd5-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d0bd5-110">Property</span></span>|<span data-ttu-id="d0bd5-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="d0bd5-111">Type</span></span>|<span data-ttu-id="d0bd5-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="d0bd5-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d0bd5-113">actionName</span><span class="sxs-lookup"><span data-stu-id="d0bd5-113">actionName</span></span>|<span data-ttu-id="d0bd5-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d0bd5-114">String</span></span>|<span data-ttu-id="d0bd5-115">Nome da ação Herdado de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="d0bd5-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="d0bd5-116">actionState</span><span class="sxs-lookup"><span data-stu-id="d0bd5-116">actionState</span></span>|[<span data-ttu-id="d0bd5-117">actionState</span><span class="sxs-lookup"><span data-stu-id="d0bd5-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="d0bd5-118">Estado da ação herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="d0bd5-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="d0bd5-119">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="d0bd5-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="d0bd5-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="d0bd5-120">startDateTime</span></span>|<span data-ttu-id="d0bd5-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d0bd5-121">DateTimeOffset</span></span>|<span data-ttu-id="d0bd5-122">Hora de início da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="d0bd5-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="d0bd5-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="d0bd5-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="d0bd5-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d0bd5-124">DateTimeOffset</span></span>|<span data-ttu-id="d0bd5-125">Hora da última atualização do estado da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="d0bd5-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="d0bd5-126">errorCode</span><span class="sxs-lookup"><span data-stu-id="d0bd5-126">errorCode</span></span>|<span data-ttu-id="d0bd5-127">Int32</span><span class="sxs-lookup"><span data-stu-id="d0bd5-127">Int32</span></span>|<span data-ttu-id="d0bd5-128">Código de erro de ação RotateBitLockerKeys</span><span class="sxs-lookup"><span data-stu-id="d0bd5-128">RotateBitLockerKeys action error code</span></span>|

## <a name="relationships"></a><span data-ttu-id="d0bd5-129">Relações</span><span class="sxs-lookup"><span data-stu-id="d0bd5-129">Relationships</span></span>
<span data-ttu-id="d0bd5-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d0bd5-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d0bd5-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d0bd5-131">JSON Representation</span></span>
<span data-ttu-id="d0bd5-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d0bd5-132">Here is a JSON representation of the resource.</span></span>
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



