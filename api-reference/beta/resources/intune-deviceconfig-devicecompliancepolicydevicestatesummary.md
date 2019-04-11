---
title: Tipo de recurso deviceCompliancePolicyDeviceStateSummary
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 68e66c7b63b8d17bf6f68ec4408cdfe113b2a9a6
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31786851"
---
# <a name="devicecompliancepolicydevicestatesummary-resource-type"></a><span data-ttu-id="07aa0-103">Tipo de recurso deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="07aa0-103">deviceCompliancePolicyDeviceStateSummary resource type</span></span>

> <span data-ttu-id="07aa0-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="07aa0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="07aa0-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="07aa0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="07aa0-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="07aa0-106">Not yet documented</span></span>

## <a name="methods"></a><span data-ttu-id="07aa0-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="07aa0-107">Methods</span></span>
|<span data-ttu-id="07aa0-108">Método</span><span class="sxs-lookup"><span data-stu-id="07aa0-108">Method</span></span>|<span data-ttu-id="07aa0-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="07aa0-109">Return Type</span></span>|<span data-ttu-id="07aa0-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="07aa0-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="07aa0-111">Acessar deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="07aa0-111">Get deviceCompliancePolicyDeviceStateSummary</span></span>](../api/intune-deviceconfig-devicecompliancepolicydevicestatesummary-get.md)|[<span data-ttu-id="07aa0-112">deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="07aa0-112">deviceCompliancePolicyDeviceStateSummary</span></span>](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md)|<span data-ttu-id="07aa0-113">Leia as propriedades e as relações do objeto [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="07aa0-113">Read properties and relationships of the [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>|
|[<span data-ttu-id="07aa0-114">Atualizar deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="07aa0-114">Update deviceCompliancePolicyDeviceStateSummary</span></span>](../api/intune-deviceconfig-devicecompliancepolicydevicestatesummary-update.md)|[<span data-ttu-id="07aa0-115">deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="07aa0-115">deviceCompliancePolicyDeviceStateSummary</span></span>](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md)|<span data-ttu-id="07aa0-116">Atualizar as propriedades de um objeto de [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="07aa0-116">Update the properties of a [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="07aa0-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="07aa0-117">Properties</span></span>
|<span data-ttu-id="07aa0-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="07aa0-118">Property</span></span>|<span data-ttu-id="07aa0-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="07aa0-119">Type</span></span>|<span data-ttu-id="07aa0-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="07aa0-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="07aa0-121">inGracePeriodCount</span><span class="sxs-lookup"><span data-stu-id="07aa0-121">inGracePeriodCount</span></span>|<span data-ttu-id="07aa0-122">Int32</span><span class="sxs-lookup"><span data-stu-id="07aa0-122">Int32</span></span>|<span data-ttu-id="07aa0-123">Quantidade de dispositivos que estão no período de cortesia</span><span class="sxs-lookup"><span data-stu-id="07aa0-123">Number of devices that are in grace period</span></span>|
|<span data-ttu-id="07aa0-124">configManagerCount</span><span class="sxs-lookup"><span data-stu-id="07aa0-124">configManagerCount</span></span>|<span data-ttu-id="07aa0-125">Int32</span><span class="sxs-lookup"><span data-stu-id="07aa0-125">Int32</span></span>|<span data-ttu-id="07aa0-126">Quantidade de dispositivos que estão em conformidade gerenciada pelo System Center Configuration Manager</span><span class="sxs-lookup"><span data-stu-id="07aa0-126">Number of devices that have compliance managed by System Center Configuration Manager</span></span>|
|<span data-ttu-id="07aa0-127">id</span><span class="sxs-lookup"><span data-stu-id="07aa0-127">id</span></span>|<span data-ttu-id="07aa0-128">String</span><span class="sxs-lookup"><span data-stu-id="07aa0-128">String</span></span>|<span data-ttu-id="07aa0-129">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="07aa0-129">Key of the entity.</span></span>|
|<span data-ttu-id="07aa0-130">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="07aa0-130">unknownDeviceCount</span></span>|<span data-ttu-id="07aa0-131">Int32</span><span class="sxs-lookup"><span data-stu-id="07aa0-131">Int32</span></span>|<span data-ttu-id="07aa0-132">Número de dispositivos desconhecidos</span><span class="sxs-lookup"><span data-stu-id="07aa0-132">Number of unknown devices</span></span>|
|<span data-ttu-id="07aa0-133">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="07aa0-133">notApplicableDeviceCount</span></span>|<span data-ttu-id="07aa0-134">Int32</span><span class="sxs-lookup"><span data-stu-id="07aa0-134">Int32</span></span>|<span data-ttu-id="07aa0-135">Número de dispositivos não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="07aa0-135">Number of not applicable devices</span></span>|
|<span data-ttu-id="07aa0-136">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="07aa0-136">compliantDeviceCount</span></span>|<span data-ttu-id="07aa0-137">Int32</span><span class="sxs-lookup"><span data-stu-id="07aa0-137">Int32</span></span>|<span data-ttu-id="07aa0-138">Número de dispositivos em conformidade</span><span class="sxs-lookup"><span data-stu-id="07aa0-138">Number of compliant devices</span></span>|
|<span data-ttu-id="07aa0-139">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="07aa0-139">remediatedDeviceCount</span></span>|<span data-ttu-id="07aa0-140">Int32</span><span class="sxs-lookup"><span data-stu-id="07aa0-140">Int32</span></span>|<span data-ttu-id="07aa0-141">Número de dispositivos corrigidos</span><span class="sxs-lookup"><span data-stu-id="07aa0-141">Number of remediated devices</span></span>|
|<span data-ttu-id="07aa0-142">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="07aa0-142">nonCompliantDeviceCount</span></span>|<span data-ttu-id="07aa0-143">Int32</span><span class="sxs-lookup"><span data-stu-id="07aa0-143">Int32</span></span>|<span data-ttu-id="07aa0-144">Número de dispositivos sem conformidade</span><span class="sxs-lookup"><span data-stu-id="07aa0-144">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="07aa0-145">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="07aa0-145">errorDeviceCount</span></span>|<span data-ttu-id="07aa0-146">Int32</span><span class="sxs-lookup"><span data-stu-id="07aa0-146">Int32</span></span>|<span data-ttu-id="07aa0-147">Número de dispositivos com erro</span><span class="sxs-lookup"><span data-stu-id="07aa0-147">Number of error devices</span></span>|
|<span data-ttu-id="07aa0-148">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="07aa0-148">conflictDeviceCount</span></span>|<span data-ttu-id="07aa0-149">Int32</span><span class="sxs-lookup"><span data-stu-id="07aa0-149">Int32</span></span>|<span data-ttu-id="07aa0-150">Número de dispositivos em conflito</span><span class="sxs-lookup"><span data-stu-id="07aa0-150">Number of conflict devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="07aa0-151">Relações</span><span class="sxs-lookup"><span data-stu-id="07aa0-151">Relationships</span></span>
<span data-ttu-id="07aa0-152">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="07aa0-152">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="07aa0-153">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="07aa0-153">JSON Representation</span></span>
<span data-ttu-id="07aa0-154">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="07aa0-154">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceCompliancePolicyDeviceStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyDeviceStateSummary",
  "inGracePeriodCount": 1024,
  "configManagerCount": 1024,
  "id": "String (identifier)",
  "unknownDeviceCount": 1024,
  "notApplicableDeviceCount": 1024,
  "compliantDeviceCount": 1024,
  "remediatedDeviceCount": 1024,
  "nonCompliantDeviceCount": 1024,
  "errorDeviceCount": 1024,
  "conflictDeviceCount": 1024
}
```





