---
title: Tipo de recurso deviceCompliancePolicyDeviceStateSummary
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 68e66c7b63b8d17bf6f68ec4408cdfe113b2a9a6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32526325"
---
# <a name="devicecompliancepolicydevicestatesummary-resource-type"></a><span data-ttu-id="c801f-103">Tipo de recurso deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="c801f-103">deviceCompliancePolicyDeviceStateSummary resource type</span></span>

> <span data-ttu-id="c801f-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c801f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c801f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c801f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c801f-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="c801f-106">Not yet documented</span></span>

## <a name="methods"></a><span data-ttu-id="c801f-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="c801f-107">Methods</span></span>
|<span data-ttu-id="c801f-108">Método</span><span class="sxs-lookup"><span data-stu-id="c801f-108">Method</span></span>|<span data-ttu-id="c801f-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c801f-109">Return Type</span></span>|<span data-ttu-id="c801f-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c801f-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c801f-111">Obter deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="c801f-111">Get deviceCompliancePolicyDeviceStateSummary</span></span>](../api/intune-deviceconfig-devicecompliancepolicydevicestatesummary-get.md)|[<span data-ttu-id="c801f-112">deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="c801f-112">deviceCompliancePolicyDeviceStateSummary</span></span>](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md)|<span data-ttu-id="c801f-113">Ler propriedades e relações de objetos de [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="c801f-113">Read properties and relationships of the [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>|
|[<span data-ttu-id="c801f-114">Atualizar deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="c801f-114">Update deviceCompliancePolicyDeviceStateSummary</span></span>](../api/intune-deviceconfig-devicecompliancepolicydevicestatesummary-update.md)|[<span data-ttu-id="c801f-115">deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="c801f-115">deviceCompliancePolicyDeviceStateSummary</span></span>](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md)|<span data-ttu-id="c801f-116">Atualizar as propriedades de um objeto de [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="c801f-116">Update the properties of a [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c801f-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c801f-117">Properties</span></span>
|<span data-ttu-id="c801f-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c801f-118">Property</span></span>|<span data-ttu-id="c801f-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="c801f-119">Type</span></span>|<span data-ttu-id="c801f-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="c801f-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c801f-121">inGracePeriodCount</span><span class="sxs-lookup"><span data-stu-id="c801f-121">inGracePeriodCount</span></span>|<span data-ttu-id="c801f-122">Int32</span><span class="sxs-lookup"><span data-stu-id="c801f-122">Int32</span></span>|<span data-ttu-id="c801f-123">Quantidade de dispositivos que estão no período de cortesia</span><span class="sxs-lookup"><span data-stu-id="c801f-123">Number of devices that are in grace period</span></span>|
|<span data-ttu-id="c801f-124">configManagerCount</span><span class="sxs-lookup"><span data-stu-id="c801f-124">configManagerCount</span></span>|<span data-ttu-id="c801f-125">Int32</span><span class="sxs-lookup"><span data-stu-id="c801f-125">Int32</span></span>|<span data-ttu-id="c801f-126">Quantidade de dispositivos que estão em conformidade gerenciada pelo System Center Configuration Manager</span><span class="sxs-lookup"><span data-stu-id="c801f-126">Number of devices that have compliance managed by System Center Configuration Manager</span></span>|
|<span data-ttu-id="c801f-127">id</span><span class="sxs-lookup"><span data-stu-id="c801f-127">id</span></span>|<span data-ttu-id="c801f-128">String</span><span class="sxs-lookup"><span data-stu-id="c801f-128">String</span></span>|<span data-ttu-id="c801f-129">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="c801f-129">Key of the entity.</span></span>|
|<span data-ttu-id="c801f-130">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c801f-130">unknownDeviceCount</span></span>|<span data-ttu-id="c801f-131">Int32</span><span class="sxs-lookup"><span data-stu-id="c801f-131">Int32</span></span>|<span data-ttu-id="c801f-132">Número de dispositivos desconhecidos</span><span class="sxs-lookup"><span data-stu-id="c801f-132">Number of unknown devices</span></span>|
|<span data-ttu-id="c801f-133">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c801f-133">notApplicableDeviceCount</span></span>|<span data-ttu-id="c801f-134">Int32</span><span class="sxs-lookup"><span data-stu-id="c801f-134">Int32</span></span>|<span data-ttu-id="c801f-135">Número de dispositivos não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="c801f-135">Number of not applicable devices</span></span>|
|<span data-ttu-id="c801f-136">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c801f-136">compliantDeviceCount</span></span>|<span data-ttu-id="c801f-137">Int32</span><span class="sxs-lookup"><span data-stu-id="c801f-137">Int32</span></span>|<span data-ttu-id="c801f-138">Número de dispositivos em conformidade</span><span class="sxs-lookup"><span data-stu-id="c801f-138">Number of compliant devices</span></span>|
|<span data-ttu-id="c801f-139">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c801f-139">remediatedDeviceCount</span></span>|<span data-ttu-id="c801f-140">Int32</span><span class="sxs-lookup"><span data-stu-id="c801f-140">Int32</span></span>|<span data-ttu-id="c801f-141">Número de dispositivos corrigidos</span><span class="sxs-lookup"><span data-stu-id="c801f-141">Number of remediated devices</span></span>|
|<span data-ttu-id="c801f-142">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c801f-142">nonCompliantDeviceCount</span></span>|<span data-ttu-id="c801f-143">Int32</span><span class="sxs-lookup"><span data-stu-id="c801f-143">Int32</span></span>|<span data-ttu-id="c801f-144">Número de dispositivos sem conformidade</span><span class="sxs-lookup"><span data-stu-id="c801f-144">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="c801f-145">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c801f-145">errorDeviceCount</span></span>|<span data-ttu-id="c801f-146">Int32</span><span class="sxs-lookup"><span data-stu-id="c801f-146">Int32</span></span>|<span data-ttu-id="c801f-147">Número de dispositivos com erro</span><span class="sxs-lookup"><span data-stu-id="c801f-147">Number of error devices</span></span>|
|<span data-ttu-id="c801f-148">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c801f-148">conflictDeviceCount</span></span>|<span data-ttu-id="c801f-149">Int32</span><span class="sxs-lookup"><span data-stu-id="c801f-149">Int32</span></span>|<span data-ttu-id="c801f-150">Número de dispositivos em conflito</span><span class="sxs-lookup"><span data-stu-id="c801f-150">Number of conflict devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="c801f-151">Relações</span><span class="sxs-lookup"><span data-stu-id="c801f-151">Relationships</span></span>
<span data-ttu-id="c801f-152">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c801f-152">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c801f-153">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c801f-153">JSON Representation</span></span>
<span data-ttu-id="c801f-154">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c801f-154">Here is a JSON representation of the resource.</span></span>
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





