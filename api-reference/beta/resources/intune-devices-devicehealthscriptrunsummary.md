---
title: Tipo de recurso deviceHealthScriptRunSummary
description: Contém propriedades para o resumo de executar um script de gerenciamento de dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b1c1b31413c19436c7dceb34a2055a238fe5881a
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665228"
---
# <a name="devicehealthscriptrunsummary-resource-type"></a><span data-ttu-id="21ec7-103">Tipo de recurso deviceHealthScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="21ec7-103">deviceHealthScriptRunSummary resource type</span></span>

<span data-ttu-id="21ec7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="21ec7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="21ec7-105">**Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="21ec7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="21ec7-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="21ec7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="21ec7-107">Contém propriedades para o resumo de executar um script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="21ec7-107">Contains properties for the run summary of a device management script.</span></span>

## <a name="methods"></a><span data-ttu-id="21ec7-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="21ec7-108">Methods</span></span>
|<span data-ttu-id="21ec7-109">Método</span><span class="sxs-lookup"><span data-stu-id="21ec7-109">Method</span></span>|<span data-ttu-id="21ec7-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="21ec7-110">Return Type</span></span>|<span data-ttu-id="21ec7-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="21ec7-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="21ec7-112">Obter deviceHealthScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="21ec7-112">Get deviceHealthScriptRunSummary</span></span>](../api/intune-devices-devicehealthscriptrunsummary-get.md)|[<span data-ttu-id="21ec7-113">deviceHealthScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="21ec7-113">deviceHealthScriptRunSummary</span></span>](../resources/intune-devices-devicehealthscriptrunsummary.md)|<span data-ttu-id="21ec7-114">Leia propriedades e relações do [objeto deviceHealthScriptRunSummary.](../resources/intune-devices-devicehealthscriptrunsummary.md)</span><span class="sxs-lookup"><span data-stu-id="21ec7-114">Read properties and relationships of the [deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md) object.</span></span>|
|[<span data-ttu-id="21ec7-115">Atualizar deviceHealthScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="21ec7-115">Update deviceHealthScriptRunSummary</span></span>](../api/intune-devices-devicehealthscriptrunsummary-update.md)|[<span data-ttu-id="21ec7-116">deviceHealthScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="21ec7-116">deviceHealthScriptRunSummary</span></span>](../resources/intune-devices-devicehealthscriptrunsummary.md)|<span data-ttu-id="21ec7-117">Atualize as propriedades de [um objeto deviceHealthScriptRunSummary.](../resources/intune-devices-devicehealthscriptrunsummary.md)</span><span class="sxs-lookup"><span data-stu-id="21ec7-117">Update the properties of a [deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="21ec7-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="21ec7-118">Properties</span></span>
|<span data-ttu-id="21ec7-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="21ec7-119">Property</span></span>|<span data-ttu-id="21ec7-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="21ec7-120">Type</span></span>|<span data-ttu-id="21ec7-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="21ec7-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21ec7-122">id</span><span class="sxs-lookup"><span data-stu-id="21ec7-122">id</span></span>|<span data-ttu-id="21ec7-123">String</span><span class="sxs-lookup"><span data-stu-id="21ec7-123">String</span></span>|<span data-ttu-id="21ec7-124">Chave da entidade resumo do script de saúde do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="21ec7-124">Key of the device health script run summary entity.</span></span> <span data-ttu-id="21ec7-125">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="21ec7-125">This property is read-only.</span></span>|
|<span data-ttu-id="21ec7-126">noIssueDetectedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="21ec7-126">noIssueDetectedDeviceCount</span></span>|<span data-ttu-id="21ec7-127">Int32</span><span class="sxs-lookup"><span data-stu-id="21ec7-127">Int32</span></span>|<span data-ttu-id="21ec7-128">Número de dispositivos para os quais o script de detecção não encontrou um problema e o dispositivo está saudável</span><span class="sxs-lookup"><span data-stu-id="21ec7-128">Number of devices for which the detection script did not find an issue and the device is healthy</span></span>|
|<span data-ttu-id="21ec7-129">issueDetectedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="21ec7-129">issueDetectedDeviceCount</span></span>|<span data-ttu-id="21ec7-130">Int32</span><span class="sxs-lookup"><span data-stu-id="21ec7-130">Int32</span></span>|<span data-ttu-id="21ec7-131">Número de dispositivos para os quais o script de detecção encontrou um problema</span><span class="sxs-lookup"><span data-stu-id="21ec7-131">Number of devices for which the detection script found an issue</span></span>|
|<span data-ttu-id="21ec7-132">detectionScriptErrorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="21ec7-132">detectionScriptErrorDeviceCount</span></span>|<span data-ttu-id="21ec7-133">Int32</span><span class="sxs-lookup"><span data-stu-id="21ec7-133">Int32</span></span>|<span data-ttu-id="21ec7-134">Número de dispositivos nos quais a execução do script de detecção encontrou um erro e não foi concluída</span><span class="sxs-lookup"><span data-stu-id="21ec7-134">Number of devices on which the detection script execution encountered an error and did not complete</span></span>|
|<span data-ttu-id="21ec7-135">detectionScriptPendingDeviceCount</span><span class="sxs-lookup"><span data-stu-id="21ec7-135">detectionScriptPendingDeviceCount</span></span>|<span data-ttu-id="21ec7-136">Int32</span><span class="sxs-lookup"><span data-stu-id="21ec7-136">Int32</span></span>|<span data-ttu-id="21ec7-137">Número de dispositivos que ainda não executaram a versão mais recente do script de saúde do dispositivo</span><span class="sxs-lookup"><span data-stu-id="21ec7-137">Number of devices which have not yet run the latest version of the device health script</span></span>|
|<span data-ttu-id="21ec7-138">detectionScriptNotApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="21ec7-138">detectionScriptNotApplicableDeviceCount</span></span>|<span data-ttu-id="21ec7-139">Int32</span><span class="sxs-lookup"><span data-stu-id="21ec7-139">Int32</span></span>|<span data-ttu-id="21ec7-140">Número de dispositivos para os quais o script de detecção não foi aplicável</span><span class="sxs-lookup"><span data-stu-id="21ec7-140">Number of devices for which the detection script was not applicable</span></span>|
|<span data-ttu-id="21ec7-141">issueRemediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="21ec7-141">issueRemediatedDeviceCount</span></span>|<span data-ttu-id="21ec7-142">Int32</span><span class="sxs-lookup"><span data-stu-id="21ec7-142">Int32</span></span>|<span data-ttu-id="21ec7-143">Número de dispositivos para os quais o script de correção foi capaz de resolver o problema detectado</span><span class="sxs-lookup"><span data-stu-id="21ec7-143">Number of devices for which the remediation script was able to resolve the detected issue</span></span>|
|<span data-ttu-id="21ec7-144">remediationSkippedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="21ec7-144">remediationSkippedDeviceCount</span></span>|<span data-ttu-id="21ec7-145">Int32</span><span class="sxs-lookup"><span data-stu-id="21ec7-145">Int32</span></span>|<span data-ttu-id="21ec7-146">Número de dispositivos para os quais a correção foi ignorada</span><span class="sxs-lookup"><span data-stu-id="21ec7-146">Number of devices for which remediation was skipped</span></span>|
|<span data-ttu-id="21ec7-147">issueReoccurredDeviceCount</span><span class="sxs-lookup"><span data-stu-id="21ec7-147">issueReoccurredDeviceCount</span></span>|<span data-ttu-id="21ec7-148">Int32</span><span class="sxs-lookup"><span data-stu-id="21ec7-148">Int32</span></span>|<span data-ttu-id="21ec7-149">Número de dispositivos para os quais o script de correção foi executado com êxito, mas não conseguiu resolver o problema detectado</span><span class="sxs-lookup"><span data-stu-id="21ec7-149">Number of devices for which the remediation script executed successfully but failed to resolve the detected issue</span></span>|
|<span data-ttu-id="21ec7-150">remediationScriptErrorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="21ec7-150">remediationScriptErrorDeviceCount</span></span>|<span data-ttu-id="21ec7-151">Int32</span><span class="sxs-lookup"><span data-stu-id="21ec7-151">Int32</span></span>|<span data-ttu-id="21ec7-152">Número de dispositivos para os quais a execução do script de correção encontrou um erro e não foi concluída</span><span class="sxs-lookup"><span data-stu-id="21ec7-152">Number of devices for which the remediation script execution encountered an error and did not complete</span></span>|
|<span data-ttu-id="21ec7-153">lastScriptRunDateTime</span><span class="sxs-lookup"><span data-stu-id="21ec7-153">lastScriptRunDateTime</span></span>|<span data-ttu-id="21ec7-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="21ec7-154">DateTimeOffset</span></span>|<span data-ttu-id="21ec7-155">Tempo de última duração do script em todos os dispositivos</span><span class="sxs-lookup"><span data-stu-id="21ec7-155">Last run time for the script across all devices</span></span>|
|<span data-ttu-id="21ec7-156">issueRemediatedCumulativeDeviceCount</span><span class="sxs-lookup"><span data-stu-id="21ec7-156">issueRemediatedCumulativeDeviceCount</span></span>|<span data-ttu-id="21ec7-157">Int32</span><span class="sxs-lookup"><span data-stu-id="21ec7-157">Int32</span></span>|<span data-ttu-id="21ec7-158">Número de dispositivos que foram remediados nos últimos 30 dias</span><span class="sxs-lookup"><span data-stu-id="21ec7-158">Number of devices that were remediated over the last 30 days</span></span>|

## <a name="relationships"></a><span data-ttu-id="21ec7-159">Relações</span><span class="sxs-lookup"><span data-stu-id="21ec7-159">Relationships</span></span>
<span data-ttu-id="21ec7-160">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="21ec7-160">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="21ec7-161">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="21ec7-161">JSON Representation</span></span>
<span data-ttu-id="21ec7-162">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="21ec7-162">Here is a JSON representation of the resource.</span></span>
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
  "detectionScriptNotApplicableDeviceCount": 1024,
  "issueRemediatedDeviceCount": 1024,
  "remediationSkippedDeviceCount": 1024,
  "issueReoccurredDeviceCount": 1024,
  "remediationScriptErrorDeviceCount": 1024,
  "lastScriptRunDateTime": "String (timestamp)",
  "issueRemediatedCumulativeDeviceCount": 1024
}
```




