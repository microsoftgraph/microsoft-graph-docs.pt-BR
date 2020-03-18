---
title: tipo de recurso deviceManagementIntentDeviceStateSummary
description: Entidade que representa o resumo de estado do dispositivo para uma intenção
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f90ef59e668b8ae053cb4abf6a6a7174860a1297
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42785411"
---
# <a name="devicemanagementintentdevicestatesummary-resource-type"></a><span data-ttu-id="9b048-103">tipo de recurso deviceManagementIntentDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="9b048-103">deviceManagementIntentDeviceStateSummary resource type</span></span>

> <span data-ttu-id="9b048-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9b048-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9b048-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9b048-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9b048-106">Entidade que representa o resumo de estado do dispositivo para uma intenção</span><span class="sxs-lookup"><span data-stu-id="9b048-106">Entity that represents device state summary for an intent</span></span>

## <a name="methods"></a><span data-ttu-id="9b048-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="9b048-107">Methods</span></span>
|<span data-ttu-id="9b048-108">Método</span><span class="sxs-lookup"><span data-stu-id="9b048-108">Method</span></span>|<span data-ttu-id="9b048-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="9b048-109">Return Type</span></span>|<span data-ttu-id="9b048-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="9b048-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9b048-111">Obter deviceManagementIntentDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="9b048-111">Get deviceManagementIntentDeviceStateSummary</span></span>](../api/intune-deviceintent-devicemanagementintentdevicestatesummary-get.md)|[<span data-ttu-id="9b048-112">deviceManagementIntentDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="9b048-112">deviceManagementIntentDeviceStateSummary</span></span>](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md)|<span data-ttu-id="9b048-113">Leia as propriedades e as relações do objeto [deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="9b048-113">Read properties and relationships of the [deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md) object.</span></span>|
|[<span data-ttu-id="9b048-114">Atualizar deviceManagementIntentDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="9b048-114">Update deviceManagementIntentDeviceStateSummary</span></span>](../api/intune-deviceintent-devicemanagementintentdevicestatesummary-update.md)|[<span data-ttu-id="9b048-115">deviceManagementIntentDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="9b048-115">deviceManagementIntentDeviceStateSummary</span></span>](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md)|<span data-ttu-id="9b048-116">Atualiza as propriedades de um objeto [deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="9b048-116">Update the properties of a [deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="9b048-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9b048-117">Properties</span></span>
|<span data-ttu-id="9b048-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9b048-118">Property</span></span>|<span data-ttu-id="9b048-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="9b048-119">Type</span></span>|<span data-ttu-id="9b048-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="9b048-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9b048-121">id</span><span class="sxs-lookup"><span data-stu-id="9b048-121">id</span></span>|<span data-ttu-id="9b048-122">String</span><span class="sxs-lookup"><span data-stu-id="9b048-122">String</span></span>|<span data-ttu-id="9b048-123">A ID</span><span class="sxs-lookup"><span data-stu-id="9b048-123">The ID</span></span>|
|<span data-ttu-id="9b048-124">conflictCount</span><span class="sxs-lookup"><span data-stu-id="9b048-124">conflictCount</span></span>|<span data-ttu-id="9b048-125">Int32</span><span class="sxs-lookup"><span data-stu-id="9b048-125">Int32</span></span>|<span data-ttu-id="9b048-126">Número de dispositivos em conflito</span><span class="sxs-lookup"><span data-stu-id="9b048-126">Number of devices in conflict</span></span>|
|<span data-ttu-id="9b048-127">errorCount</span><span class="sxs-lookup"><span data-stu-id="9b048-127">errorCount</span></span>|<span data-ttu-id="9b048-128">Int32</span><span class="sxs-lookup"><span data-stu-id="9b048-128">Int32</span></span>|<span data-ttu-id="9b048-129">Número de dispositivos com erro</span><span class="sxs-lookup"><span data-stu-id="9b048-129">Number of error devices</span></span>|
|<span data-ttu-id="9b048-130">failedCount</span><span class="sxs-lookup"><span data-stu-id="9b048-130">failedCount</span></span>|<span data-ttu-id="9b048-131">Int32</span><span class="sxs-lookup"><span data-stu-id="9b048-131">Int32</span></span>|<span data-ttu-id="9b048-132">Número de dispositivos com falha</span><span class="sxs-lookup"><span data-stu-id="9b048-132">Number of failed devices</span></span>|
|<span data-ttu-id="9b048-133">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="9b048-133">notApplicableCount</span></span>|<span data-ttu-id="9b048-134">Int32</span><span class="sxs-lookup"><span data-stu-id="9b048-134">Int32</span></span>|<span data-ttu-id="9b048-135">Número de dispositivos não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="9b048-135">Number of not applicable devices</span></span>|
|<span data-ttu-id="9b048-136">notApplicablePlatformCount</span><span class="sxs-lookup"><span data-stu-id="9b048-136">notApplicablePlatformCount</span></span>|<span data-ttu-id="9b048-137">Int32</span><span class="sxs-lookup"><span data-stu-id="9b048-137">Int32</span></span>|<span data-ttu-id="9b048-138">Número de dispositivos não aplicáveis devido à plataforma e à política incompatíveis</span><span class="sxs-lookup"><span data-stu-id="9b048-138">Number of not applicable devices due to mismatch platform and policy</span></span>|
|<span data-ttu-id="9b048-139">successCount</span><span class="sxs-lookup"><span data-stu-id="9b048-139">successCount</span></span>|<span data-ttu-id="9b048-140">Int32</span><span class="sxs-lookup"><span data-stu-id="9b048-140">Int32</span></span>|<span data-ttu-id="9b048-141">Número de dispositivos com êxito</span><span class="sxs-lookup"><span data-stu-id="9b048-141">Number of succeeded devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="9b048-142">Relações</span><span class="sxs-lookup"><span data-stu-id="9b048-142">Relationships</span></span>
<span data-ttu-id="9b048-143">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9b048-143">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9b048-144">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9b048-144">JSON Representation</span></span>
<span data-ttu-id="9b048-145">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9b048-145">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementIntentDeviceStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementIntentDeviceStateSummary",
  "id": "String (identifier)",
  "conflictCount": 1024,
  "errorCount": 1024,
  "failedCount": 1024,
  "notApplicableCount": 1024,
  "notApplicablePlatformCount": 1024,
  "successCount": 1024
}
```



