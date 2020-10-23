---
title: tipo de recurso deviceManagementIntentDeviceStateSummary
description: Entidade que representa o resumo de estado do dispositivo para uma intenção
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b87b37a61f3847f77e38fd429c9dd7096235cfff
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48708799"
---
# <a name="devicemanagementintentdevicestatesummary-resource-type"></a><span data-ttu-id="11563-103">tipo de recurso deviceManagementIntentDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="11563-103">deviceManagementIntentDeviceStateSummary resource type</span></span>

<span data-ttu-id="11563-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="11563-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="11563-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="11563-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="11563-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="11563-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="11563-107">Entidade que representa o resumo de estado do dispositivo para uma intenção</span><span class="sxs-lookup"><span data-stu-id="11563-107">Entity that represents device state summary for an intent</span></span>

## <a name="methods"></a><span data-ttu-id="11563-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="11563-108">Methods</span></span>
|<span data-ttu-id="11563-109">Método</span><span class="sxs-lookup"><span data-stu-id="11563-109">Method</span></span>|<span data-ttu-id="11563-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="11563-110">Return Type</span></span>|<span data-ttu-id="11563-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="11563-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="11563-112">Obter deviceManagementIntentDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="11563-112">Get deviceManagementIntentDeviceStateSummary</span></span>](../api/intune-deviceintent-devicemanagementintentdevicestatesummary-get.md)|[<span data-ttu-id="11563-113">deviceManagementIntentDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="11563-113">deviceManagementIntentDeviceStateSummary</span></span>](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md)|<span data-ttu-id="11563-114">Leia as propriedades e as relações do objeto [deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="11563-114">Read properties and relationships of the [deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md) object.</span></span>|
|[<span data-ttu-id="11563-115">Atualizar deviceManagementIntentDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="11563-115">Update deviceManagementIntentDeviceStateSummary</span></span>](../api/intune-deviceintent-devicemanagementintentdevicestatesummary-update.md)|[<span data-ttu-id="11563-116">deviceManagementIntentDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="11563-116">deviceManagementIntentDeviceStateSummary</span></span>](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md)|<span data-ttu-id="11563-117">Atualiza as propriedades de um objeto [deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="11563-117">Update the properties of a [deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="11563-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="11563-118">Properties</span></span>
|<span data-ttu-id="11563-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="11563-119">Property</span></span>|<span data-ttu-id="11563-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="11563-120">Type</span></span>|<span data-ttu-id="11563-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="11563-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11563-122">id</span><span class="sxs-lookup"><span data-stu-id="11563-122">id</span></span>|<span data-ttu-id="11563-123">String</span><span class="sxs-lookup"><span data-stu-id="11563-123">String</span></span>|<span data-ttu-id="11563-124">A ID</span><span class="sxs-lookup"><span data-stu-id="11563-124">The ID</span></span>|
|<span data-ttu-id="11563-125">conflictCount</span><span class="sxs-lookup"><span data-stu-id="11563-125">conflictCount</span></span>|<span data-ttu-id="11563-126">Int32</span><span class="sxs-lookup"><span data-stu-id="11563-126">Int32</span></span>|<span data-ttu-id="11563-127">Número de dispositivos em conflito</span><span class="sxs-lookup"><span data-stu-id="11563-127">Number of devices in conflict</span></span>|
|<span data-ttu-id="11563-128">errorCount</span><span class="sxs-lookup"><span data-stu-id="11563-128">errorCount</span></span>|<span data-ttu-id="11563-129">Int32</span><span class="sxs-lookup"><span data-stu-id="11563-129">Int32</span></span>|<span data-ttu-id="11563-130">Número de dispositivos com erro</span><span class="sxs-lookup"><span data-stu-id="11563-130">Number of error devices</span></span>|
|<span data-ttu-id="11563-131">failedCount</span><span class="sxs-lookup"><span data-stu-id="11563-131">failedCount</span></span>|<span data-ttu-id="11563-132">Int32</span><span class="sxs-lookup"><span data-stu-id="11563-132">Int32</span></span>|<span data-ttu-id="11563-133">Número de dispositivos com falha</span><span class="sxs-lookup"><span data-stu-id="11563-133">Number of failed devices</span></span>|
|<span data-ttu-id="11563-134">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="11563-134">notApplicableCount</span></span>|<span data-ttu-id="11563-135">Int32</span><span class="sxs-lookup"><span data-stu-id="11563-135">Int32</span></span>|<span data-ttu-id="11563-136">Número de dispositivos não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="11563-136">Number of not applicable devices</span></span>|
|<span data-ttu-id="11563-137">notApplicablePlatformCount</span><span class="sxs-lookup"><span data-stu-id="11563-137">notApplicablePlatformCount</span></span>|<span data-ttu-id="11563-138">Int32</span><span class="sxs-lookup"><span data-stu-id="11563-138">Int32</span></span>|<span data-ttu-id="11563-139">Número de dispositivos não aplicáveis devido à plataforma e à política incompatíveis</span><span class="sxs-lookup"><span data-stu-id="11563-139">Number of not applicable devices due to mismatch platform and policy</span></span>|
|<span data-ttu-id="11563-140">successCount</span><span class="sxs-lookup"><span data-stu-id="11563-140">successCount</span></span>|<span data-ttu-id="11563-141">Int32</span><span class="sxs-lookup"><span data-stu-id="11563-141">Int32</span></span>|<span data-ttu-id="11563-142">Número de dispositivos com êxito</span><span class="sxs-lookup"><span data-stu-id="11563-142">Number of succeeded devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="11563-143">Relações</span><span class="sxs-lookup"><span data-stu-id="11563-143">Relationships</span></span>
<span data-ttu-id="11563-144">Nenhum</span><span class="sxs-lookup"><span data-stu-id="11563-144">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="11563-145">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="11563-145">JSON Representation</span></span>
<span data-ttu-id="11563-146">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="11563-146">Here is a JSON representation of the resource.</span></span>
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





