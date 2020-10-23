---
title: tipo de recurso rotateBitLockerKeysDeviceActionResult
description: Resultado da ação do dispositivo RotateBitLockerKeys
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6457b87007fe24084c35b27c1b658de564767984
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48724492"
---
# <a name="rotatebitlockerkeysdeviceactionresult-resource-type"></a><span data-ttu-id="a238a-103">tipo de recurso rotateBitLockerKeysDeviceActionResult</span><span class="sxs-lookup"><span data-stu-id="a238a-103">rotateBitLockerKeysDeviceActionResult resource type</span></span>

<span data-ttu-id="a238a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a238a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a238a-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a238a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a238a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a238a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a238a-107">Resultado da ação do dispositivo RotateBitLockerKeys</span><span class="sxs-lookup"><span data-stu-id="a238a-107">RotateBitLockerKeys device action result</span></span>


<span data-ttu-id="a238a-108">Herda de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="a238a-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a238a-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a238a-109">Properties</span></span>
|<span data-ttu-id="a238a-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a238a-110">Property</span></span>|<span data-ttu-id="a238a-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="a238a-111">Type</span></span>|<span data-ttu-id="a238a-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="a238a-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a238a-113">actionName</span><span class="sxs-lookup"><span data-stu-id="a238a-113">actionName</span></span>|<span data-ttu-id="a238a-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a238a-114">String</span></span>|<span data-ttu-id="a238a-115">Nome da ação Herdado de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="a238a-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="a238a-116">actionState</span><span class="sxs-lookup"><span data-stu-id="a238a-116">actionState</span></span>|[<span data-ttu-id="a238a-117">actionState</span><span class="sxs-lookup"><span data-stu-id="a238a-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="a238a-118">Estado da ação herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="a238a-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="a238a-119">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="a238a-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="a238a-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="a238a-120">startDateTime</span></span>|<span data-ttu-id="a238a-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a238a-121">DateTimeOffset</span></span>|<span data-ttu-id="a238a-122">Hora de início da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="a238a-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="a238a-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="a238a-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="a238a-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a238a-124">DateTimeOffset</span></span>|<span data-ttu-id="a238a-125">Hora da última atualização do estado da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="a238a-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="a238a-126">errorCode</span><span class="sxs-lookup"><span data-stu-id="a238a-126">errorCode</span></span>|<span data-ttu-id="a238a-127">Int32</span><span class="sxs-lookup"><span data-stu-id="a238a-127">Int32</span></span>|<span data-ttu-id="a238a-128">Código de erro de ação RotateBitLockerKeys</span><span class="sxs-lookup"><span data-stu-id="a238a-128">RotateBitLockerKeys action error code</span></span>|

## <a name="relationships"></a><span data-ttu-id="a238a-129">Relações</span><span class="sxs-lookup"><span data-stu-id="a238a-129">Relationships</span></span>
<span data-ttu-id="a238a-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a238a-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a238a-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a238a-131">JSON Representation</span></span>
<span data-ttu-id="a238a-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a238a-132">Here is a JSON representation of the resource.</span></span>
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





