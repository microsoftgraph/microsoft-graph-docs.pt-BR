---
title: Tipo de recurso remoteLockActionResult
description: Resultado da ação de bloquear com um pin para desbloquear
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 062d287aec9f0a0be8acbf380a5300458367f014
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37356902"
---
# <a name="remotelockactionresult-resource-type"></a><span data-ttu-id="b0ec4-103">Tipo de recurso remoteLockActionResult</span><span class="sxs-lookup"><span data-stu-id="b0ec4-103">remoteLockActionResult resource type</span></span>

> <span data-ttu-id="b0ec4-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b0ec4-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b0ec4-105">Resultado da ação de bloquear com um pin para desbloquear</span><span class="sxs-lookup"><span data-stu-id="b0ec4-105">Lock action result with a pin to unlock</span></span>


<span data-ttu-id="b0ec4-106">Herda de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="b0ec4-106">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b0ec4-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b0ec4-107">Properties</span></span>
|<span data-ttu-id="b0ec4-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b0ec4-108">Property</span></span>|<span data-ttu-id="b0ec4-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="b0ec4-109">Type</span></span>|<span data-ttu-id="b0ec4-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="b0ec4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0ec4-111">actionName</span><span class="sxs-lookup"><span data-stu-id="b0ec4-111">actionName</span></span>|<span data-ttu-id="b0ec4-112">String</span><span class="sxs-lookup"><span data-stu-id="b0ec4-112">String</span></span>|<span data-ttu-id="b0ec4-113">Nome da ação Herdado de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="b0ec4-113">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="b0ec4-114">actionState</span><span class="sxs-lookup"><span data-stu-id="b0ec4-114">actionState</span></span>|[<span data-ttu-id="b0ec4-115">actionState</span><span class="sxs-lookup"><span data-stu-id="b0ec4-115">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="b0ec4-116">Estado da ação herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="b0ec4-116">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="b0ec4-117">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="b0ec4-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="b0ec4-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="b0ec4-118">startDateTime</span></span>|<span data-ttu-id="b0ec4-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b0ec4-119">DateTimeOffset</span></span>|<span data-ttu-id="b0ec4-120">Hora de início da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="b0ec4-120">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="b0ec4-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="b0ec4-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="b0ec4-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b0ec4-122">DateTimeOffset</span></span>|<span data-ttu-id="b0ec4-123">Hora em que o estado da ação foi atualizado pela última vez, herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="b0ec4-123">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="b0ec4-124">unlockPin</span><span class="sxs-lookup"><span data-stu-id="b0ec4-124">unlockPin</span></span>|<span data-ttu-id="b0ec4-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b0ec4-125">String</span></span>|<span data-ttu-id="b0ec4-126">PIN para desbloquear o cliente</span><span class="sxs-lookup"><span data-stu-id="b0ec4-126">Pin to unlock the client</span></span>|

## <a name="relationships"></a><span data-ttu-id="b0ec4-127">Relações</span><span class="sxs-lookup"><span data-stu-id="b0ec4-127">Relationships</span></span>
<span data-ttu-id="b0ec4-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b0ec4-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b0ec4-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b0ec4-129">JSON Representation</span></span>
<span data-ttu-id="b0ec4-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b0ec4-130">Here is a JSON representation of the resource.</span></span>
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




