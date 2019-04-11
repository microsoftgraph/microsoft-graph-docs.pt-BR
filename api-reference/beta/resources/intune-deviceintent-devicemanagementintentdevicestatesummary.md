---
title: tipo de recurso deviceManagementIntentDeviceStateSummary
description: Entidade que representa o resumo de estado do dispositivo para uma intenção
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f78f35a11241b5bf0376816827e79c6b1cc3e7bf
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31805856"
---
# <a name="devicemanagementintentdevicestatesummary-resource-type"></a><span data-ttu-id="30d91-103">tipo de recurso deviceManagementIntentDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="30d91-103">deviceManagementIntentDeviceStateSummary resource type</span></span>

> <span data-ttu-id="30d91-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="30d91-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="30d91-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="30d91-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="30d91-106">Entidade que representa o resumo de estado do dispositivo para uma intenção</span><span class="sxs-lookup"><span data-stu-id="30d91-106">Entity that represents device state summary for an intent</span></span>

## <a name="methods"></a><span data-ttu-id="30d91-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="30d91-107">Methods</span></span>
|<span data-ttu-id="30d91-108">Método</span><span class="sxs-lookup"><span data-stu-id="30d91-108">Method</span></span>|<span data-ttu-id="30d91-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="30d91-109">Return Type</span></span>|<span data-ttu-id="30d91-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="30d91-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="30d91-111">Obter deviceManagementIntentDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="30d91-111">Get deviceManagementIntentDeviceStateSummary</span></span>](../api/intune-deviceintent-devicemanagementintentdevicestatesummary-get.md)|[<span data-ttu-id="30d91-112">deviceManagementIntentDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="30d91-112">deviceManagementIntentDeviceStateSummary</span></span>](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md)|<span data-ttu-id="30d91-113">Leia as propriedades e as relações do objeto [deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="30d91-113">Read properties and relationships of the [deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md) object.</span></span>|
|[<span data-ttu-id="30d91-114">Atualizar deviceManagementIntentDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="30d91-114">Update deviceManagementIntentDeviceStateSummary</span></span>](../api/intune-deviceintent-devicemanagementintentdevicestatesummary-update.md)|[<span data-ttu-id="30d91-115">deviceManagementIntentDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="30d91-115">deviceManagementIntentDeviceStateSummary</span></span>](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md)|<span data-ttu-id="30d91-116">Atualiza as propriedades de um objeto [deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="30d91-116">Update the properties of a [deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="30d91-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="30d91-117">Properties</span></span>
|<span data-ttu-id="30d91-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="30d91-118">Property</span></span>|<span data-ttu-id="30d91-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="30d91-119">Type</span></span>|<span data-ttu-id="30d91-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="30d91-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="30d91-121">id</span><span class="sxs-lookup"><span data-stu-id="30d91-121">id</span></span>|<span data-ttu-id="30d91-122">String</span><span class="sxs-lookup"><span data-stu-id="30d91-122">String</span></span>|<span data-ttu-id="30d91-123">A ID</span><span class="sxs-lookup"><span data-stu-id="30d91-123">The ID</span></span>|
|<span data-ttu-id="30d91-124">conflictCount</span><span class="sxs-lookup"><span data-stu-id="30d91-124">conflictCount</span></span>|<span data-ttu-id="30d91-125">Int32</span><span class="sxs-lookup"><span data-stu-id="30d91-125">Int32</span></span>|<span data-ttu-id="30d91-126">Número de dispositivos em conflito</span><span class="sxs-lookup"><span data-stu-id="30d91-126">Number of devices in conflict</span></span>|
|<span data-ttu-id="30d91-127">errorCount</span><span class="sxs-lookup"><span data-stu-id="30d91-127">errorCount</span></span>|<span data-ttu-id="30d91-128">Int32</span><span class="sxs-lookup"><span data-stu-id="30d91-128">Int32</span></span>|<span data-ttu-id="30d91-129">Número de dispositivos com erro</span><span class="sxs-lookup"><span data-stu-id="30d91-129">Number of error devices</span></span>|
|<span data-ttu-id="30d91-130">failedCount</span><span class="sxs-lookup"><span data-stu-id="30d91-130">failedCount</span></span>|<span data-ttu-id="30d91-131">Int32</span><span class="sxs-lookup"><span data-stu-id="30d91-131">Int32</span></span>|<span data-ttu-id="30d91-132">Número de dispositivos com falha</span><span class="sxs-lookup"><span data-stu-id="30d91-132">Number of failed devices</span></span>|
|<span data-ttu-id="30d91-133">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="30d91-133">notApplicableCount</span></span>|<span data-ttu-id="30d91-134">Int32</span><span class="sxs-lookup"><span data-stu-id="30d91-134">Int32</span></span>|<span data-ttu-id="30d91-135">Número de dispositivos não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="30d91-135">Number of not applicable devices</span></span>|
|<span data-ttu-id="30d91-136">notApplicablePlatformCount</span><span class="sxs-lookup"><span data-stu-id="30d91-136">notApplicablePlatformCount</span></span>|<span data-ttu-id="30d91-137">Int32</span><span class="sxs-lookup"><span data-stu-id="30d91-137">Int32</span></span>|<span data-ttu-id="30d91-138">Número de dispositivos não aplicáveis devido à plataforma e à política incompatíveis</span><span class="sxs-lookup"><span data-stu-id="30d91-138">Number of not applicable devices due to mismatch platform and policy</span></span>|
|<span data-ttu-id="30d91-139">successCount</span><span class="sxs-lookup"><span data-stu-id="30d91-139">successCount</span></span>|<span data-ttu-id="30d91-140">Int32</span><span class="sxs-lookup"><span data-stu-id="30d91-140">Int32</span></span>|<span data-ttu-id="30d91-141">Número de dispositivos com êxito</span><span class="sxs-lookup"><span data-stu-id="30d91-141">Number of succeeded devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="30d91-142">Relações</span><span class="sxs-lookup"><span data-stu-id="30d91-142">Relationships</span></span>
<span data-ttu-id="30d91-143">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="30d91-143">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="30d91-144">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="30d91-144">JSON Representation</span></span>
<span data-ttu-id="30d91-145">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="30d91-145">Here is a JSON representation of the resource.</span></span>
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





