---
title: tipo de recurso deviceHealthScriptRunSummary
description: Contém propriedades para o resumo de execução de um script de gerenciamento de dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: bd5a96191780b113fea84ea6534e5a47ad8890c9
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43388405"
---
# <a name="devicehealthscriptrunsummary-resource-type"></a><span data-ttu-id="d05ff-103">tipo de recurso deviceHealthScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="d05ff-103">deviceHealthScriptRunSummary resource type</span></span>

<span data-ttu-id="d05ff-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d05ff-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d05ff-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d05ff-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d05ff-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d05ff-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d05ff-107">Contém propriedades para o resumo de execução de um script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d05ff-107">Contains properties for the run summary of a device management script.</span></span>

## <a name="methods"></a><span data-ttu-id="d05ff-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="d05ff-108">Methods</span></span>
|<span data-ttu-id="d05ff-109">Método</span><span class="sxs-lookup"><span data-stu-id="d05ff-109">Method</span></span>|<span data-ttu-id="d05ff-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d05ff-110">Return Type</span></span>|<span data-ttu-id="d05ff-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d05ff-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d05ff-112">Obter deviceHealthScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="d05ff-112">Get deviceHealthScriptRunSummary</span></span>](../api/intune-devices-devicehealthscriptrunsummary-get.md)|[<span data-ttu-id="d05ff-113">deviceHealthScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="d05ff-113">deviceHealthScriptRunSummary</span></span>](../resources/intune-devices-devicehealthscriptrunsummary.md)|<span data-ttu-id="d05ff-114">Leia as propriedades e as relações do objeto [deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="d05ff-114">Read properties and relationships of the [deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md) object.</span></span>|
|[<span data-ttu-id="d05ff-115">Atualizar deviceHealthScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="d05ff-115">Update deviceHealthScriptRunSummary</span></span>](../api/intune-devices-devicehealthscriptrunsummary-update.md)|[<span data-ttu-id="d05ff-116">deviceHealthScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="d05ff-116">deviceHealthScriptRunSummary</span></span>](../resources/intune-devices-devicehealthscriptrunsummary.md)|<span data-ttu-id="d05ff-117">Atualiza as propriedades de um objeto [deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="d05ff-117">Update the properties of a [deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d05ff-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d05ff-118">Properties</span></span>
|<span data-ttu-id="d05ff-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d05ff-119">Property</span></span>|<span data-ttu-id="d05ff-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="d05ff-120">Type</span></span>|<span data-ttu-id="d05ff-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="d05ff-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d05ff-122">id</span><span class="sxs-lookup"><span data-stu-id="d05ff-122">id</span></span>|<span data-ttu-id="d05ff-123">String</span><span class="sxs-lookup"><span data-stu-id="d05ff-123">String</span></span>|<span data-ttu-id="d05ff-124">Chave da entidade de Resumo de execução de script de integridade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d05ff-124">Key of the device health script run summary entity.</span></span> <span data-ttu-id="d05ff-125">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d05ff-125">This property is read-only.</span></span>|
|<span data-ttu-id="d05ff-126">noIssueDetectedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d05ff-126">noIssueDetectedDeviceCount</span></span>|<span data-ttu-id="d05ff-127">Int32</span><span class="sxs-lookup"><span data-stu-id="d05ff-127">Int32</span></span>|<span data-ttu-id="d05ff-128">Número de dispositivos para os quais o script de detecção não encontrou um problema e o dispositivo está íntegro</span><span class="sxs-lookup"><span data-stu-id="d05ff-128">Number of devices for which the detection script did not find an issue and the device is healthy</span></span>|
|<span data-ttu-id="d05ff-129">issueDetectedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d05ff-129">issueDetectedDeviceCount</span></span>|<span data-ttu-id="d05ff-130">Int32</span><span class="sxs-lookup"><span data-stu-id="d05ff-130">Int32</span></span>|<span data-ttu-id="d05ff-131">Número de dispositivos para os quais o script de detecção encontrou um problema</span><span class="sxs-lookup"><span data-stu-id="d05ff-131">Number of devices for which the detection script found an issue</span></span>|
|<span data-ttu-id="d05ff-132">detectionScriptErrorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d05ff-132">detectionScriptErrorDeviceCount</span></span>|<span data-ttu-id="d05ff-133">Int32</span><span class="sxs-lookup"><span data-stu-id="d05ff-133">Int32</span></span>|<span data-ttu-id="d05ff-134">Número de dispositivos nos quais a execução do script de detecção encontrou um erro e não foi concluída</span><span class="sxs-lookup"><span data-stu-id="d05ff-134">Number of devices on which the detection script execution encountered an error and did not complete</span></span>|
|<span data-ttu-id="d05ff-135">detectionScriptPendingDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d05ff-135">detectionScriptPendingDeviceCount</span></span>|<span data-ttu-id="d05ff-136">Int32</span><span class="sxs-lookup"><span data-stu-id="d05ff-136">Int32</span></span>|<span data-ttu-id="d05ff-137">Número de dispositivos que ainda não executaram a versão mais recente do script de integridade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="d05ff-137">Number of devices which have not yet run the latest version of the device health script</span></span>|
|<span data-ttu-id="d05ff-138">issueRemediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d05ff-138">issueRemediatedDeviceCount</span></span>|<span data-ttu-id="d05ff-139">Int32</span><span class="sxs-lookup"><span data-stu-id="d05ff-139">Int32</span></span>|<span data-ttu-id="d05ff-140">Número de dispositivos para os quais o script de correção foi capaz de resolver o problema detectado</span><span class="sxs-lookup"><span data-stu-id="d05ff-140">Number of devices for which the remediation script was able to resolve the detected issue</span></span>|
|<span data-ttu-id="d05ff-141">remediationSkippedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d05ff-141">remediationSkippedDeviceCount</span></span>|<span data-ttu-id="d05ff-142">Int32</span><span class="sxs-lookup"><span data-stu-id="d05ff-142">Int32</span></span>|<span data-ttu-id="d05ff-143">Número de dispositivos para os quais a correção foi ignorada</span><span class="sxs-lookup"><span data-stu-id="d05ff-143">Number of devices for which remediation was skipped</span></span>|
|<span data-ttu-id="d05ff-144">issueReoccurredDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d05ff-144">issueReoccurredDeviceCount</span></span>|<span data-ttu-id="d05ff-145">Int32</span><span class="sxs-lookup"><span data-stu-id="d05ff-145">Int32</span></span>|<span data-ttu-id="d05ff-146">Número de dispositivos para os quais o script de correção foi executado com êxito, mas falhou ao resolver o problema detectado</span><span class="sxs-lookup"><span data-stu-id="d05ff-146">Number of devices for which the remediation script executed successfully but failed to resolve the detected issue</span></span>|
|<span data-ttu-id="d05ff-147">remediationScriptErrorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d05ff-147">remediationScriptErrorDeviceCount</span></span>|<span data-ttu-id="d05ff-148">Int32</span><span class="sxs-lookup"><span data-stu-id="d05ff-148">Int32</span></span>|<span data-ttu-id="d05ff-149">Número de dispositivos para os quais a execução do script de correção encontrou um erro e não foi concluída</span><span class="sxs-lookup"><span data-stu-id="d05ff-149">Number of devices for which the remediation script execution encountered an error and did not complete</span></span>|
|<span data-ttu-id="d05ff-150">lastScriptRunDateTime</span><span class="sxs-lookup"><span data-stu-id="d05ff-150">lastScriptRunDateTime</span></span>|<span data-ttu-id="d05ff-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d05ff-151">DateTimeOffset</span></span>|<span data-ttu-id="d05ff-152">Hora da última execução para o script em todos os dispositivos</span><span class="sxs-lookup"><span data-stu-id="d05ff-152">Last run time for the script across all devices</span></span>|
|<span data-ttu-id="d05ff-153">issueRemediatedCumulativeDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d05ff-153">issueRemediatedCumulativeDeviceCount</span></span>|<span data-ttu-id="d05ff-154">Int32</span><span class="sxs-lookup"><span data-stu-id="d05ff-154">Int32</span></span>|<span data-ttu-id="d05ff-155">Número de dispositivos que foram corrigidos nos últimos 30 dias</span><span class="sxs-lookup"><span data-stu-id="d05ff-155">Number of devices that were remediated over the last 30 days</span></span>|

## <a name="relationships"></a><span data-ttu-id="d05ff-156">Relações</span><span class="sxs-lookup"><span data-stu-id="d05ff-156">Relationships</span></span>
<span data-ttu-id="d05ff-157">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d05ff-157">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d05ff-158">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d05ff-158">JSON Representation</span></span>
<span data-ttu-id="d05ff-159">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d05ff-159">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceHealthScriptRunSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptRunSummary",
  "id": "String (identifier)",
  "noIssueDetectedDeviceCount": 1024,
  "issueDetectedDeviceCount": 1024,
  "detectionScriptErrorDeviceCount": 1024,
  "detectionScriptPendingDeviceCount": 1024,
  "issueRemediatedDeviceCount": 1024,
  "remediationSkippedDeviceCount": 1024,
  "issueReoccurredDeviceCount": 1024,
  "remediationScriptErrorDeviceCount": 1024,
  "lastScriptRunDateTime": "String (timestamp)",
  "issueRemediatedCumulativeDeviceCount": 1024
}
```



