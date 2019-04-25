---
title: Tipo de recurso remoteLockActionResult
description: Resultado da ação de bloquear com um pin para desbloquear
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c533d9590acba1518ac3d0dc791af804b9d84452
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32550634"
---
# <a name="remotelockactionresult-resource-type"></a><span data-ttu-id="fb713-103">Tipo de recurso remoteLockActionResult</span><span class="sxs-lookup"><span data-stu-id="fb713-103">remoteLockActionResult resource type</span></span>

> <span data-ttu-id="fb713-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fb713-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fb713-105">Resultado da ação de bloquear com um pin para desbloquear</span><span class="sxs-lookup"><span data-stu-id="fb713-105">Lock action result with a pin to unlock</span></span>


<span data-ttu-id="fb713-106">Herda de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="fb713-106">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="fb713-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fb713-107">Properties</span></span>
|<span data-ttu-id="fb713-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fb713-108">Property</span></span>|<span data-ttu-id="fb713-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="fb713-109">Type</span></span>|<span data-ttu-id="fb713-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="fb713-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fb713-111">actionName</span><span class="sxs-lookup"><span data-stu-id="fb713-111">actionName</span></span>|<span data-ttu-id="fb713-112">String</span><span class="sxs-lookup"><span data-stu-id="fb713-112">String</span></span>|<span data-ttu-id="fb713-113">Nome da ação Herdado de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="fb713-113">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="fb713-114">actionState</span><span class="sxs-lookup"><span data-stu-id="fb713-114">actionState</span></span>|[<span data-ttu-id="fb713-115">actionState</span><span class="sxs-lookup"><span data-stu-id="fb713-115">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="fb713-116">Estado da ação herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="fb713-116">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="fb713-117">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="fb713-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="fb713-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="fb713-118">startDateTime</span></span>|<span data-ttu-id="fb713-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fb713-119">DateTimeOffset</span></span>|<span data-ttu-id="fb713-120">Hora de início da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="fb713-120">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="fb713-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="fb713-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="fb713-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fb713-122">DateTimeOffset</span></span>|<span data-ttu-id="fb713-123">Hora em que o estado da ação foi atualizado pela última vez, herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="fb713-123">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="fb713-124">unlockPin</span><span class="sxs-lookup"><span data-stu-id="fb713-124">unlockPin</span></span>|<span data-ttu-id="fb713-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fb713-125">String</span></span>|<span data-ttu-id="fb713-126">PIN para desbloquear o cliente</span><span class="sxs-lookup"><span data-stu-id="fb713-126">Pin to unlock the client</span></span>|

## <a name="relationships"></a><span data-ttu-id="fb713-127">Relações</span><span class="sxs-lookup"><span data-stu-id="fb713-127">Relationships</span></span>
<span data-ttu-id="fb713-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fb713-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fb713-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fb713-129">JSON Representation</span></span>
<span data-ttu-id="fb713-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fb713-130">Here is a JSON representation of the resource.</span></span>
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



