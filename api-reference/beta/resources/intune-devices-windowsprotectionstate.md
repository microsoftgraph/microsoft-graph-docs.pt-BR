---
title: tipo de recurso Windowsprotectionstate foi
description: Entidade de status de proteção de dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b2651aa9fad173654d8fff554bdf89f7ab36da14
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49207558"
---
# <a name="windowsprotectionstate-resource-type"></a><span data-ttu-id="23876-103">tipo de recurso Windowsprotectionstate foi</span><span class="sxs-lookup"><span data-stu-id="23876-103">windowsProtectionState resource type</span></span>

<span data-ttu-id="23876-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="23876-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="23876-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="23876-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="23876-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="23876-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="23876-107">Entidade de status de proteção de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="23876-107">Device protection status entity.</span></span>

## <a name="methods"></a><span data-ttu-id="23876-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="23876-108">Methods</span></span>
|<span data-ttu-id="23876-109">Método</span><span class="sxs-lookup"><span data-stu-id="23876-109">Method</span></span>|<span data-ttu-id="23876-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="23876-110">Return Type</span></span>|<span data-ttu-id="23876-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="23876-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="23876-112">Obter Windowsprotectionstate foi</span><span class="sxs-lookup"><span data-stu-id="23876-112">Get windowsProtectionState</span></span>](../api/intune-devices-windowsprotectionstate-get.md)|[<span data-ttu-id="23876-113">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="23876-113">windowsProtectionState</span></span>](../resources/intune-devices-windowsprotectionstate.md)|<span data-ttu-id="23876-114">Leia as propriedades e as relações do objeto [windowsprotectionstate foi](../resources/intune-devices-windowsprotectionstate.md) .</span><span class="sxs-lookup"><span data-stu-id="23876-114">Read properties and relationships of the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>|
|[<span data-ttu-id="23876-115">Atualizar Windowsprotectionstate foi</span><span class="sxs-lookup"><span data-stu-id="23876-115">Update windowsProtectionState</span></span>](../api/intune-devices-windowsprotectionstate-update.md)|[<span data-ttu-id="23876-116">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="23876-116">windowsProtectionState</span></span>](../resources/intune-devices-windowsprotectionstate.md)|<span data-ttu-id="23876-117">Atualiza as propriedades de um objeto [windowsprotectionstate foi](../resources/intune-devices-windowsprotectionstate.md) .</span><span class="sxs-lookup"><span data-stu-id="23876-117">Update the properties of a [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="23876-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="23876-118">Properties</span></span>
|<span data-ttu-id="23876-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="23876-119">Property</span></span>|<span data-ttu-id="23876-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="23876-120">Type</span></span>|<span data-ttu-id="23876-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="23876-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23876-122">id</span><span class="sxs-lookup"><span data-stu-id="23876-122">id</span></span>|<span data-ttu-id="23876-123">String</span><span class="sxs-lookup"><span data-stu-id="23876-123">String</span></span>|<span data-ttu-id="23876-124">O identificador exclusivo do objeto de status de proteção de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="23876-124">The unique Identifier for the device protection status object.</span></span> <span data-ttu-id="23876-125">Esta é a ID do dispositivo</span><span class="sxs-lookup"><span data-stu-id="23876-125">This is device id of the device</span></span>|
|<span data-ttu-id="23876-126">malwareProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="23876-126">malwareProtectionEnabled</span></span>|<span data-ttu-id="23876-127">Booliano</span><span class="sxs-lookup"><span data-stu-id="23876-127">Boolean</span></span>|<span data-ttu-id="23876-128">O anti-malware está habilitado ou não</span><span class="sxs-lookup"><span data-stu-id="23876-128">Anti malware is enabled or not</span></span>|
|<span data-ttu-id="23876-129">DeviceState</span><span class="sxs-lookup"><span data-stu-id="23876-129">deviceState</span></span>|[<span data-ttu-id="23876-130">windowsDeviceHealthState</span><span class="sxs-lookup"><span data-stu-id="23876-130">windowsDeviceHealthState</span></span>](../resources/intune-devices-windowsdevicehealthstate.md)|<span data-ttu-id="23876-131">Estado do computador (como verificação completa ou pendente ou reinicialização pendente, etc.).</span><span class="sxs-lookup"><span data-stu-id="23876-131">Computer's state (like clean or pending full scan or pending reboot etc).</span></span> <span data-ttu-id="23876-132">Os possíveis valores são: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span><span class="sxs-lookup"><span data-stu-id="23876-132">Possible values are: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span></span>|
|<span data-ttu-id="23876-133">realTimeProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="23876-133">realTimeProtectionEnabled</span></span>|<span data-ttu-id="23876-134">Booliano</span><span class="sxs-lookup"><span data-stu-id="23876-134">Boolean</span></span>|<span data-ttu-id="23876-135">A proteção em tempo real está habilitada ou não?</span><span class="sxs-lookup"><span data-stu-id="23876-135">Real time protection is enabled or not?</span></span>|
|<span data-ttu-id="23876-136">networkInspectionSystemEnabled</span><span class="sxs-lookup"><span data-stu-id="23876-136">networkInspectionSystemEnabled</span></span>|<span data-ttu-id="23876-137">Booliano</span><span class="sxs-lookup"><span data-stu-id="23876-137">Boolean</span></span>|<span data-ttu-id="23876-138">Sistema de inspeção de rede habilitado ou não?</span><span class="sxs-lookup"><span data-stu-id="23876-138">Network inspection system enabled or not?</span></span>|
|<span data-ttu-id="23876-139">quickScanOverdue</span><span class="sxs-lookup"><span data-stu-id="23876-139">quickScanOverdue</span></span>|<span data-ttu-id="23876-140">Booliano</span><span class="sxs-lookup"><span data-stu-id="23876-140">Boolean</span></span>|<span data-ttu-id="23876-141">Verificação rápida em atraso ou não?</span><span class="sxs-lookup"><span data-stu-id="23876-141">Quick scan overdue or not?</span></span>|
|<span data-ttu-id="23876-142">fullScanOverdue</span><span class="sxs-lookup"><span data-stu-id="23876-142">fullScanOverdue</span></span>|<span data-ttu-id="23876-143">Booliano</span><span class="sxs-lookup"><span data-stu-id="23876-143">Boolean</span></span>|<span data-ttu-id="23876-144">Verificação completa em atraso ou não?</span><span class="sxs-lookup"><span data-stu-id="23876-144">Full scan overdue or not?</span></span>|
|<span data-ttu-id="23876-145">signatureUpdateOverdue</span><span class="sxs-lookup"><span data-stu-id="23876-145">signatureUpdateOverdue</span></span>|<span data-ttu-id="23876-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="23876-146">Boolean</span></span>|<span data-ttu-id="23876-147">Assinatura desatualizada ou não?</span><span class="sxs-lookup"><span data-stu-id="23876-147">Signature out of date or not?</span></span>|
|<span data-ttu-id="23876-148">rebootRequired</span><span class="sxs-lookup"><span data-stu-id="23876-148">rebootRequired</span></span>|<span data-ttu-id="23876-149">Booliano</span><span class="sxs-lookup"><span data-stu-id="23876-149">Boolean</span></span>|<span data-ttu-id="23876-150">Reinicialização necessária ou não?</span><span class="sxs-lookup"><span data-stu-id="23876-150">Reboot required or not?</span></span>|
|<span data-ttu-id="23876-151">fullScanRequired</span><span class="sxs-lookup"><span data-stu-id="23876-151">fullScanRequired</span></span>|<span data-ttu-id="23876-152">Booliano</span><span class="sxs-lookup"><span data-stu-id="23876-152">Boolean</span></span>|<span data-ttu-id="23876-153">Verificação completa necessária ou não?</span><span class="sxs-lookup"><span data-stu-id="23876-153">Full scan required or not?</span></span>|
|<span data-ttu-id="23876-154">engineVersion</span><span class="sxs-lookup"><span data-stu-id="23876-154">engineVersion</span></span>|<span data-ttu-id="23876-155">String</span><span class="sxs-lookup"><span data-stu-id="23876-155">String</span></span>|<span data-ttu-id="23876-156">Versão atual do mecanismo do Endpoint Protection</span><span class="sxs-lookup"><span data-stu-id="23876-156">Current endpoint protection engine's version</span></span>|
|<span data-ttu-id="23876-157">signatureVersion</span><span class="sxs-lookup"><span data-stu-id="23876-157">signatureVersion</span></span>|<span data-ttu-id="23876-158">String</span><span class="sxs-lookup"><span data-stu-id="23876-158">String</span></span>|<span data-ttu-id="23876-159">Versão atual de definições de malware</span><span class="sxs-lookup"><span data-stu-id="23876-159">Current malware definitions version</span></span>|
|<span data-ttu-id="23876-160">antiMalwareVersion</span><span class="sxs-lookup"><span data-stu-id="23876-160">antiMalwareVersion</span></span>|<span data-ttu-id="23876-161">String</span><span class="sxs-lookup"><span data-stu-id="23876-161">String</span></span>|<span data-ttu-id="23876-162">Versão Antimalware atual</span><span class="sxs-lookup"><span data-stu-id="23876-162">Current anti malware version</span></span>|
|<span data-ttu-id="23876-163">lastQuickScanDateTime</span><span class="sxs-lookup"><span data-stu-id="23876-163">lastQuickScanDateTime</span></span>|<span data-ttu-id="23876-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="23876-164">DateTimeOffset</span></span>|<span data-ttu-id="23876-165">Data e hora da última verificação rápida</span><span class="sxs-lookup"><span data-stu-id="23876-165">Last quick scan datetime</span></span>|
|<span data-ttu-id="23876-166">lastFullScanDateTime</span><span class="sxs-lookup"><span data-stu-id="23876-166">lastFullScanDateTime</span></span>|<span data-ttu-id="23876-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="23876-167">DateTimeOffset</span></span>|<span data-ttu-id="23876-168">Data e hora da última verificação rápida</span><span class="sxs-lookup"><span data-stu-id="23876-168">Last quick scan datetime</span></span>|
|<span data-ttu-id="23876-169">lastQuickScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="23876-169">lastQuickScanSignatureVersion</span></span>|<span data-ttu-id="23876-170">String</span><span class="sxs-lookup"><span data-stu-id="23876-170">String</span></span>|<span data-ttu-id="23876-171">Versão da última assinatura de verificação rápida</span><span class="sxs-lookup"><span data-stu-id="23876-171">Last quick scan signature version</span></span>|
|<span data-ttu-id="23876-172">lastFullScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="23876-172">lastFullScanSignatureVersion</span></span>|<span data-ttu-id="23876-173">String</span><span class="sxs-lookup"><span data-stu-id="23876-173">String</span></span>|<span data-ttu-id="23876-174">Versão da última assinatura de verificação completa</span><span class="sxs-lookup"><span data-stu-id="23876-174">Last full scan signature version</span></span>|
|<span data-ttu-id="23876-175">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="23876-175">lastReportedDateTime</span></span>|<span data-ttu-id="23876-176">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="23876-176">DateTimeOffset</span></span>|<span data-ttu-id="23876-177">Hora do último status de integridade do dispositivo relatado</span><span class="sxs-lookup"><span data-stu-id="23876-177">Last device health status reported time</span></span>|
|<span data-ttu-id="23876-178">productStatus</span><span class="sxs-lookup"><span data-stu-id="23876-178">productStatus</span></span>|[<span data-ttu-id="23876-179">windowsDefenderProductStatus</span><span class="sxs-lookup"><span data-stu-id="23876-179">windowsDefenderProductStatus</span></span>](../resources/intune-devices-windowsdefenderproductstatus.md)|<span data-ttu-id="23876-180">Status do produto do Windows Defender antivírus.</span><span class="sxs-lookup"><span data-stu-id="23876-180">Product Status of Windows Defender Antivirus.</span></span> <span data-ttu-id="23876-181">Os valores possíveis são:,,,,,,,,,,,,,,, `noStatus` `serviceNotRunning` `serviceStartedWithoutMalwareProtection` `pendingFullScanDueToThreatAction` `pendingRebootDueToThreatAction` `pendingManualStepsDueToThreatAction` `avSignaturesOutOfDate` `asSignaturesOutOfDate` `noQuickScanHappenedForSpecifiedPeriod` `noFullScanHappenedForSpecifiedPeriod` `systemInitiatedScanInProgress` `systemInitiatedCleanInProgress` `samplesPendingSubmission` `productRunningInEvaluationMode` `productRunningInNonGenuineMode` `productExpired` `offlineScanRequired` , `serviceShutdownAsPartOfSystemShutdown` , `threatRemediationFailedCritically` , `threatRemediationFailedNonCritically` `noStatusFlagsSet` `platformOutOfDate` `platformUpdateInProgress` `platformAboutToBeOutdated` `signatureOrPlatformEndOfLifeIsPastOrIsImpending` `windowsSModeSignaturesInUseOnNonWin10SInstall` ,,,,,,,,,,,,,,,.</span><span class="sxs-lookup"><span data-stu-id="23876-181">Possible values are: `noStatus`, `serviceNotRunning`, `serviceStartedWithoutMalwareProtection`, `pendingFullScanDueToThreatAction`, `pendingRebootDueToThreatAction`, `pendingManualStepsDueToThreatAction`, `avSignaturesOutOfDate`, `asSignaturesOutOfDate`, `noQuickScanHappenedForSpecifiedPeriod`, `noFullScanHappenedForSpecifiedPeriod`, `systemInitiatedScanInProgress`, `systemInitiatedCleanInProgress`, `samplesPendingSubmission`, `productRunningInEvaluationMode`, `productRunningInNonGenuineMode`, `productExpired`, `offlineScanRequired`, `serviceShutdownAsPartOfSystemShutdown`, `threatRemediationFailedCritically`, `threatRemediationFailedNonCritically`, `noStatusFlagsSet`, `platformOutOfDate`, `platformUpdateInProgress`, `platformAboutToBeOutdated`, `signatureOrPlatformEndOfLifeIsPastOrIsImpending`, `windowsSModeSignaturesInUseOnNonWin10SInstall`.</span></span>|
|<span data-ttu-id="23876-182">isVirtualMachine</span><span class="sxs-lookup"><span data-stu-id="23876-182">isVirtualMachine</span></span>|<span data-ttu-id="23876-183">Booliano</span><span class="sxs-lookup"><span data-stu-id="23876-183">Boolean</span></span>|<span data-ttu-id="23876-184">Indica se o dispositivo é uma máquina virtual.</span><span class="sxs-lookup"><span data-stu-id="23876-184">Indicates whether the device is a virtual machine.</span></span>|
|<span data-ttu-id="23876-185">tamperProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="23876-185">tamperProtectionEnabled</span></span>|<span data-ttu-id="23876-186">Booliano</span><span class="sxs-lookup"><span data-stu-id="23876-186">Boolean</span></span>|<span data-ttu-id="23876-187">Indica se o recurso proteção de violação do Windows Defender está habilitado.</span><span class="sxs-lookup"><span data-stu-id="23876-187">Indicates whether the Windows Defender tamper protection feature is enabled.</span></span>|

## <a name="relationships"></a><span data-ttu-id="23876-188">Relações</span><span class="sxs-lookup"><span data-stu-id="23876-188">Relationships</span></span>
|<span data-ttu-id="23876-189">Relação</span><span class="sxs-lookup"><span data-stu-id="23876-189">Relationship</span></span>|<span data-ttu-id="23876-190">Tipo</span><span class="sxs-lookup"><span data-stu-id="23876-190">Type</span></span>|<span data-ttu-id="23876-191">Descrição</span><span class="sxs-lookup"><span data-stu-id="23876-191">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23876-192">detectedMalwareState</span><span class="sxs-lookup"><span data-stu-id="23876-192">detectedMalwareState</span></span>|<span data-ttu-id="23876-193">coleção [windowsDeviceMalwareState](../resources/intune-devices-windowsdevicemalwarestate.md)</span><span class="sxs-lookup"><span data-stu-id="23876-193">[windowsDeviceMalwareState](../resources/intune-devices-windowsdevicemalwarestate.md) collection</span></span>|<span data-ttu-id="23876-194">Lista de malware do dispositivo</span><span class="sxs-lookup"><span data-stu-id="23876-194">Device malware list</span></span>|

## <a name="json-representation"></a><span data-ttu-id="23876-195">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="23876-195">JSON Representation</span></span>
<span data-ttu-id="23876-196">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="23876-196">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsProtectionState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsProtectionState",
  "id": "String (identifier)",
  "malwareProtectionEnabled": true,
  "deviceState": "String",
  "realTimeProtectionEnabled": true,
  "networkInspectionSystemEnabled": true,
  "quickScanOverdue": true,
  "fullScanOverdue": true,
  "signatureUpdateOverdue": true,
  "rebootRequired": true,
  "fullScanRequired": true,
  "engineVersion": "String",
  "signatureVersion": "String",
  "antiMalwareVersion": "String",
  "lastQuickScanDateTime": "String (timestamp)",
  "lastFullScanDateTime": "String (timestamp)",
  "lastQuickScanSignatureVersion": "String",
  "lastFullScanSignatureVersion": "String",
  "lastReportedDateTime": "String (timestamp)",
  "productStatus": "String",
  "isVirtualMachine": true,
  "tamperProtectionEnabled": true
}
```




