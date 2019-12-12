---
title: tipo de recurso deviceHealthScriptRunSummary
description: Contém propriedades para o resumo de execução de um script de gerenciamento de dispositivo.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8f17e7725802879f639ce6803f9f6c12dca21e5f
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39955480"
---
# <a name="devicehealthscriptrunsummary-resource-type"></a><span data-ttu-id="9e4ab-103">tipo de recurso deviceHealthScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="9e4ab-103">deviceHealthScriptRunSummary resource type</span></span>

> <span data-ttu-id="9e4ab-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9e4ab-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9e4ab-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9e4ab-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9e4ab-106">Contém propriedades para o resumo de execução de um script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9e4ab-106">Contains properties for the run summary of a device management script.</span></span>

## <a name="methods"></a><span data-ttu-id="9e4ab-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="9e4ab-107">Methods</span></span>
|<span data-ttu-id="9e4ab-108">Método</span><span class="sxs-lookup"><span data-stu-id="9e4ab-108">Method</span></span>|<span data-ttu-id="9e4ab-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="9e4ab-109">Return Type</span></span>|<span data-ttu-id="9e4ab-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="9e4ab-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9e4ab-111">Obter deviceHealthScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="9e4ab-111">Get deviceHealthScriptRunSummary</span></span>](../api/intune-devices-devicehealthscriptrunsummary-get.md)|[<span data-ttu-id="9e4ab-112">deviceHealthScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="9e4ab-112">deviceHealthScriptRunSummary</span></span>](../resources/intune-devices-devicehealthscriptrunsummary.md)|<span data-ttu-id="9e4ab-113">Leia as propriedades e as relações do objeto [deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="9e4ab-113">Read properties and relationships of the [deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md) object.</span></span>|
|[<span data-ttu-id="9e4ab-114">Atualizar deviceHealthScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="9e4ab-114">Update deviceHealthScriptRunSummary</span></span>](../api/intune-devices-devicehealthscriptrunsummary-update.md)|[<span data-ttu-id="9e4ab-115">deviceHealthScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="9e4ab-115">deviceHealthScriptRunSummary</span></span>](../resources/intune-devices-devicehealthscriptrunsummary.md)|<span data-ttu-id="9e4ab-116">Atualiza as propriedades de um objeto [deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="9e4ab-116">Update the properties of a [deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="9e4ab-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9e4ab-117">Properties</span></span>
|<span data-ttu-id="9e4ab-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9e4ab-118">Property</span></span>|<span data-ttu-id="9e4ab-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="9e4ab-119">Type</span></span>|<span data-ttu-id="9e4ab-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="9e4ab-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9e4ab-121">id</span><span class="sxs-lookup"><span data-stu-id="9e4ab-121">id</span></span>|<span data-ttu-id="9e4ab-122">String</span><span class="sxs-lookup"><span data-stu-id="9e4ab-122">String</span></span>|<span data-ttu-id="9e4ab-123">Chave da entidade de Resumo de execução de script de integridade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9e4ab-123">Key of the device health script run summary entity.</span></span> <span data-ttu-id="9e4ab-124">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9e4ab-124">This property is read-only.</span></span>|
|<span data-ttu-id="9e4ab-125">noIssueDetectedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9e4ab-125">noIssueDetectedDeviceCount</span></span>|<span data-ttu-id="9e4ab-126">Int32</span><span class="sxs-lookup"><span data-stu-id="9e4ab-126">Int32</span></span>|<span data-ttu-id="9e4ab-127">Número de dispositivos para os quais o script de detecção não encontrou um problema e o dispositivo está íntegro</span><span class="sxs-lookup"><span data-stu-id="9e4ab-127">Number of devices for which the detection script did not find an issue and the device is healthy</span></span>|
|<span data-ttu-id="9e4ab-128">issueDetectedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9e4ab-128">issueDetectedDeviceCount</span></span>|<span data-ttu-id="9e4ab-129">Int32</span><span class="sxs-lookup"><span data-stu-id="9e4ab-129">Int32</span></span>|<span data-ttu-id="9e4ab-130">Número de dispositivos para os quais o script de detecção encontrou um problema</span><span class="sxs-lookup"><span data-stu-id="9e4ab-130">Number of devices for which the detection script found an issue</span></span>|
|<span data-ttu-id="9e4ab-131">detectionScriptErrorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9e4ab-131">detectionScriptErrorDeviceCount</span></span>|<span data-ttu-id="9e4ab-132">Int32</span><span class="sxs-lookup"><span data-stu-id="9e4ab-132">Int32</span></span>|<span data-ttu-id="9e4ab-133">Número de dispositivos nos quais a execução do script de detecção encontrou um erro e não foi concluída</span><span class="sxs-lookup"><span data-stu-id="9e4ab-133">Number of devices on which the detection script execution encountered an error and did not complete</span></span>|
|<span data-ttu-id="9e4ab-134">detectionScriptPendingDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9e4ab-134">detectionScriptPendingDeviceCount</span></span>|<span data-ttu-id="9e4ab-135">Int32</span><span class="sxs-lookup"><span data-stu-id="9e4ab-135">Int32</span></span>|<span data-ttu-id="9e4ab-136">Número de dispositivos que ainda não executaram a versão mais recente do script de integridade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="9e4ab-136">Number of devices which have not yet run the latest version of the device health script</span></span>|
|<span data-ttu-id="9e4ab-137">issueRemediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9e4ab-137">issueRemediatedDeviceCount</span></span>|<span data-ttu-id="9e4ab-138">Int32</span><span class="sxs-lookup"><span data-stu-id="9e4ab-138">Int32</span></span>|<span data-ttu-id="9e4ab-139">Número de dispositivos para os quais o script de correção foi capaz de resolver o problema detectado</span><span class="sxs-lookup"><span data-stu-id="9e4ab-139">Number of devices for which the remediation script was able to resolve the detected issue</span></span>|
|<span data-ttu-id="9e4ab-140">remediationSkippedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9e4ab-140">remediationSkippedDeviceCount</span></span>|<span data-ttu-id="9e4ab-141">Int32</span><span class="sxs-lookup"><span data-stu-id="9e4ab-141">Int32</span></span>|<span data-ttu-id="9e4ab-142">Número de dispositivos para os quais a correção foi ignorada</span><span class="sxs-lookup"><span data-stu-id="9e4ab-142">Number of devices for which remediation was skipped</span></span>|
|<span data-ttu-id="9e4ab-143">issueReoccurredDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9e4ab-143">issueReoccurredDeviceCount</span></span>|<span data-ttu-id="9e4ab-144">Int32</span><span class="sxs-lookup"><span data-stu-id="9e4ab-144">Int32</span></span>|<span data-ttu-id="9e4ab-145">Número de dispositivos para os quais o script de correção foi executado com êxito, mas falhou ao resolver o problema detectado</span><span class="sxs-lookup"><span data-stu-id="9e4ab-145">Number of devices for which the remediation script executed successfully but failed to resolve the detected issue</span></span>|
|<span data-ttu-id="9e4ab-146">remediationScriptErrorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9e4ab-146">remediationScriptErrorDeviceCount</span></span>|<span data-ttu-id="9e4ab-147">Int32</span><span class="sxs-lookup"><span data-stu-id="9e4ab-147">Int32</span></span>|<span data-ttu-id="9e4ab-148">Número de dispositivos para os quais a execução do script de correção encontrou um erro e não foi concluída</span><span class="sxs-lookup"><span data-stu-id="9e4ab-148">Number of devices for which the remediation script execution encountered an error and did not complete</span></span>|
|<span data-ttu-id="9e4ab-149">lastScriptRunDateTime</span><span class="sxs-lookup"><span data-stu-id="9e4ab-149">lastScriptRunDateTime</span></span>|<span data-ttu-id="9e4ab-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e4ab-150">DateTimeOffset</span></span>|<span data-ttu-id="9e4ab-151">Hora da última execução para o script em todos os dispositivos</span><span class="sxs-lookup"><span data-stu-id="9e4ab-151">Last run time for the script across all devices</span></span>|
|<span data-ttu-id="9e4ab-152">issueRemediatedCumulativeDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9e4ab-152">issueRemediatedCumulativeDeviceCount</span></span>|<span data-ttu-id="9e4ab-153">Int32</span><span class="sxs-lookup"><span data-stu-id="9e4ab-153">Int32</span></span>|<span data-ttu-id="9e4ab-154">Número de dispositivos que foram corrigidos nos últimos 30 dias</span><span class="sxs-lookup"><span data-stu-id="9e4ab-154">Number of devices that were remediated over the last 30 days</span></span>|

## <a name="relationships"></a><span data-ttu-id="9e4ab-155">Relações</span><span class="sxs-lookup"><span data-stu-id="9e4ab-155">Relationships</span></span>
<span data-ttu-id="9e4ab-156">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9e4ab-156">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9e4ab-157">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9e4ab-157">JSON Representation</span></span>
<span data-ttu-id="9e4ab-158">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9e4ab-158">Here is a JSON representation of the resource.</span></span>
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



