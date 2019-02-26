---
title: Tipo de recurso remoteLockActionResult
description: Resultado da ação de bloquear com um pin para desbloquear
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c533d9590acba1518ac3d0dc791af804b9d84452
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30260316"
---
# <a name="remotelockactionresult-resource-type"></a><span data-ttu-id="82e89-103">Tipo de recurso remoteLockActionResult</span><span class="sxs-lookup"><span data-stu-id="82e89-103">remoteLockActionResult resource type</span></span>

> <span data-ttu-id="82e89-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="82e89-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="82e89-105">Resultado da ação de bloquear com um pin para desbloquear</span><span class="sxs-lookup"><span data-stu-id="82e89-105">Lock action result with a pin to unlock</span></span>


<span data-ttu-id="82e89-106">Herda de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="82e89-106">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="82e89-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="82e89-107">Properties</span></span>
|<span data-ttu-id="82e89-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="82e89-108">Property</span></span>|<span data-ttu-id="82e89-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="82e89-109">Type</span></span>|<span data-ttu-id="82e89-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="82e89-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="82e89-111">actionName</span><span class="sxs-lookup"><span data-stu-id="82e89-111">actionName</span></span>|<span data-ttu-id="82e89-112">String</span><span class="sxs-lookup"><span data-stu-id="82e89-112">String</span></span>|<span data-ttu-id="82e89-113">Nome da ação herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="82e89-113">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="82e89-114">actionState</span><span class="sxs-lookup"><span data-stu-id="82e89-114">actionState</span></span>|[<span data-ttu-id="82e89-115">actionState</span><span class="sxs-lookup"><span data-stu-id="82e89-115">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="82e89-116">Estado da ação herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="82e89-116">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="82e89-117">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="82e89-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="82e89-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="82e89-118">startDateTime</span></span>|<span data-ttu-id="82e89-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="82e89-119">DateTimeOffset</span></span>|<span data-ttu-id="82e89-120">Hora em que ação foi iniciada, herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="82e89-120">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="82e89-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="82e89-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="82e89-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="82e89-122">DateTimeOffset</span></span>|<span data-ttu-id="82e89-123">Hora em que o estado da ação foi atualizado pela última vez, herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="82e89-123">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="82e89-124">unlockPin</span><span class="sxs-lookup"><span data-stu-id="82e89-124">unlockPin</span></span>|<span data-ttu-id="82e89-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="82e89-125">String</span></span>|<span data-ttu-id="82e89-126">PIN para desbloquear o cliente</span><span class="sxs-lookup"><span data-stu-id="82e89-126">Pin to unlock the client</span></span>|

## <a name="relationships"></a><span data-ttu-id="82e89-127">Relações</span><span class="sxs-lookup"><span data-stu-id="82e89-127">Relationships</span></span>
<span data-ttu-id="82e89-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="82e89-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="82e89-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="82e89-129">JSON Representation</span></span>
<span data-ttu-id="82e89-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="82e89-130">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.remoteLockActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.remoteLockActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "unlockPin": "String"
}
```



