---
title: Tipo de recurso remoteLockActionResult
description: Resultado da ação de bloquear com um pin para desbloquear
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b16a99c793d60de04201fc057a58da122c83fd6c
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31788517"
---
# <a name="remotelockactionresult-resource-type"></a><span data-ttu-id="badcd-103">Tipo de recurso remoteLockActionResult</span><span class="sxs-lookup"><span data-stu-id="badcd-103">remoteLockActionResult resource type</span></span>

> <span data-ttu-id="badcd-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="badcd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="badcd-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="badcd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="badcd-106">Resultado da ação de bloquear com um pin para desbloquear</span><span class="sxs-lookup"><span data-stu-id="badcd-106">Lock action result with a pin to unlock</span></span>


<span data-ttu-id="badcd-107">Herda de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="badcd-107">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="badcd-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="badcd-108">Properties</span></span>
|<span data-ttu-id="badcd-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="badcd-109">Property</span></span>|<span data-ttu-id="badcd-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="badcd-110">Type</span></span>|<span data-ttu-id="badcd-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="badcd-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="badcd-112">actionName</span><span class="sxs-lookup"><span data-stu-id="badcd-112">actionName</span></span>|<span data-ttu-id="badcd-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="badcd-113">String</span></span>|<span data-ttu-id="badcd-114">Nome da ação Herdado de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="badcd-114">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="badcd-115">actionState</span><span class="sxs-lookup"><span data-stu-id="badcd-115">actionState</span></span>|[<span data-ttu-id="badcd-116">actionState</span><span class="sxs-lookup"><span data-stu-id="badcd-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="badcd-117">Estado da ação herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="badcd-117">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="badcd-118">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="badcd-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="badcd-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="badcd-119">startDateTime</span></span>|<span data-ttu-id="badcd-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="badcd-120">DateTimeOffset</span></span>|<span data-ttu-id="badcd-121">Hora de início da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="badcd-121">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="badcd-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="badcd-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="badcd-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="badcd-123">DateTimeOffset</span></span>|<span data-ttu-id="badcd-124">Hora em que o estado da ação foi atualizado pela última vez, herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="badcd-124">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="badcd-125">unlockPin</span><span class="sxs-lookup"><span data-stu-id="badcd-125">unlockPin</span></span>|<span data-ttu-id="badcd-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="badcd-126">String</span></span>|<span data-ttu-id="badcd-127">PIN para desbloquear o cliente</span><span class="sxs-lookup"><span data-stu-id="badcd-127">Pin to unlock the client</span></span>|

## <a name="relationships"></a><span data-ttu-id="badcd-128">Relações</span><span class="sxs-lookup"><span data-stu-id="badcd-128">Relationships</span></span>
<span data-ttu-id="badcd-129">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="badcd-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="badcd-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="badcd-130">JSON Representation</span></span>
<span data-ttu-id="badcd-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="badcd-131">Here is a JSON representation of the resource.</span></span>
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





