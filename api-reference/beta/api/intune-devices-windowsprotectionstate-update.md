---
title: Atualizar Windowsprotectionstate foi
description: Atualiza as propriedades de um objeto Windowsprotectionstate foi.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6c5317326018404986a63243678455c59302683f
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49212689"
---
# <a name="update-windowsprotectionstate"></a><span data-ttu-id="3acdf-103">Atualizar Windowsprotectionstate foi</span><span class="sxs-lookup"><span data-stu-id="3acdf-103">Update windowsProtectionState</span></span>

<span data-ttu-id="3acdf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3acdf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3acdf-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3acdf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3acdf-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3acdf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3acdf-107">Atualiza as propriedades de um objeto [windowsprotectionstate foi](../resources/intune-devices-windowsprotectionstate.md) .</span><span class="sxs-lookup"><span data-stu-id="3acdf-107">Update the properties of a [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3acdf-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3acdf-108">Prerequisites</span></span>
<span data-ttu-id="3acdf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3acdf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3acdf-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3acdf-111">Permission type</span></span>|<span data-ttu-id="3acdf-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3acdf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3acdf-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3acdf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3acdf-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3acdf-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="3acdf-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3acdf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3acdf-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3acdf-116">Not supported.</span></span>|
|<span data-ttu-id="3acdf-117">Application</span><span class="sxs-lookup"><span data-stu-id="3acdf-117">Application</span></span>|<span data-ttu-id="3acdf-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3acdf-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3acdf-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3acdf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/windowsProtectionState
```

## <a name="request-headers"></a><span data-ttu-id="3acdf-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3acdf-120">Request headers</span></span>
|<span data-ttu-id="3acdf-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3acdf-121">Header</span></span>|<span data-ttu-id="3acdf-122">Valor</span><span class="sxs-lookup"><span data-stu-id="3acdf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3acdf-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3acdf-123">Authorization</span></span>|<span data-ttu-id="3acdf-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3acdf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3acdf-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3acdf-125">Accept</span></span>|<span data-ttu-id="3acdf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3acdf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3acdf-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3acdf-127">Request body</span></span>
<span data-ttu-id="3acdf-128">No corpo da solicitação, forneça uma representação JSON do objeto [windowsprotectionstate foi](../resources/intune-devices-windowsprotectionstate.md) .</span><span class="sxs-lookup"><span data-stu-id="3acdf-128">In the request body, supply a JSON representation for the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>

<span data-ttu-id="3acdf-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsprotectionstate foi](../resources/intune-devices-windowsprotectionstate.md).</span><span class="sxs-lookup"><span data-stu-id="3acdf-129">The following table shows the properties that are required when you create the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md).</span></span>

|<span data-ttu-id="3acdf-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3acdf-130">Property</span></span>|<span data-ttu-id="3acdf-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="3acdf-131">Type</span></span>|<span data-ttu-id="3acdf-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="3acdf-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3acdf-133">id</span><span class="sxs-lookup"><span data-stu-id="3acdf-133">id</span></span>|<span data-ttu-id="3acdf-134">String</span><span class="sxs-lookup"><span data-stu-id="3acdf-134">String</span></span>|<span data-ttu-id="3acdf-135">O identificador exclusivo do objeto de status de proteção de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3acdf-135">The unique Identifier for the device protection status object.</span></span> <span data-ttu-id="3acdf-136">Esta é a ID do dispositivo</span><span class="sxs-lookup"><span data-stu-id="3acdf-136">This is device id of the device</span></span>|
|<span data-ttu-id="3acdf-137">malwareProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="3acdf-137">malwareProtectionEnabled</span></span>|<span data-ttu-id="3acdf-138">Booliano</span><span class="sxs-lookup"><span data-stu-id="3acdf-138">Boolean</span></span>|<span data-ttu-id="3acdf-139">O anti-malware está habilitado ou não</span><span class="sxs-lookup"><span data-stu-id="3acdf-139">Anti malware is enabled or not</span></span>|
|<span data-ttu-id="3acdf-140">DeviceState</span><span class="sxs-lookup"><span data-stu-id="3acdf-140">deviceState</span></span>|[<span data-ttu-id="3acdf-141">windowsDeviceHealthState</span><span class="sxs-lookup"><span data-stu-id="3acdf-141">windowsDeviceHealthState</span></span>](../resources/intune-devices-windowsdevicehealthstate.md)|<span data-ttu-id="3acdf-142">Estado do computador (como verificação completa ou pendente ou reinicialização pendente, etc.).</span><span class="sxs-lookup"><span data-stu-id="3acdf-142">Computer's state (like clean or pending full scan or pending reboot etc).</span></span> <span data-ttu-id="3acdf-143">Os possíveis valores são: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span><span class="sxs-lookup"><span data-stu-id="3acdf-143">Possible values are: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span></span>|
|<span data-ttu-id="3acdf-144">realTimeProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="3acdf-144">realTimeProtectionEnabled</span></span>|<span data-ttu-id="3acdf-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="3acdf-145">Boolean</span></span>|<span data-ttu-id="3acdf-146">A proteção em tempo real está habilitada ou não?</span><span class="sxs-lookup"><span data-stu-id="3acdf-146">Real time protection is enabled or not?</span></span>|
|<span data-ttu-id="3acdf-147">networkInspectionSystemEnabled</span><span class="sxs-lookup"><span data-stu-id="3acdf-147">networkInspectionSystemEnabled</span></span>|<span data-ttu-id="3acdf-148">Booliano</span><span class="sxs-lookup"><span data-stu-id="3acdf-148">Boolean</span></span>|<span data-ttu-id="3acdf-149">Sistema de inspeção de rede habilitado ou não?</span><span class="sxs-lookup"><span data-stu-id="3acdf-149">Network inspection system enabled or not?</span></span>|
|<span data-ttu-id="3acdf-150">quickScanOverdue</span><span class="sxs-lookup"><span data-stu-id="3acdf-150">quickScanOverdue</span></span>|<span data-ttu-id="3acdf-151">Booliano</span><span class="sxs-lookup"><span data-stu-id="3acdf-151">Boolean</span></span>|<span data-ttu-id="3acdf-152">Verificação rápida em atraso ou não?</span><span class="sxs-lookup"><span data-stu-id="3acdf-152">Quick scan overdue or not?</span></span>|
|<span data-ttu-id="3acdf-153">fullScanOverdue</span><span class="sxs-lookup"><span data-stu-id="3acdf-153">fullScanOverdue</span></span>|<span data-ttu-id="3acdf-154">Booliano</span><span class="sxs-lookup"><span data-stu-id="3acdf-154">Boolean</span></span>|<span data-ttu-id="3acdf-155">Verificação completa em atraso ou não?</span><span class="sxs-lookup"><span data-stu-id="3acdf-155">Full scan overdue or not?</span></span>|
|<span data-ttu-id="3acdf-156">signatureUpdateOverdue</span><span class="sxs-lookup"><span data-stu-id="3acdf-156">signatureUpdateOverdue</span></span>|<span data-ttu-id="3acdf-157">Booliano</span><span class="sxs-lookup"><span data-stu-id="3acdf-157">Boolean</span></span>|<span data-ttu-id="3acdf-158">Assinatura desatualizada ou não?</span><span class="sxs-lookup"><span data-stu-id="3acdf-158">Signature out of date or not?</span></span>|
|<span data-ttu-id="3acdf-159">rebootRequired</span><span class="sxs-lookup"><span data-stu-id="3acdf-159">rebootRequired</span></span>|<span data-ttu-id="3acdf-160">Booliano</span><span class="sxs-lookup"><span data-stu-id="3acdf-160">Boolean</span></span>|<span data-ttu-id="3acdf-161">Reinicialização necessária ou não?</span><span class="sxs-lookup"><span data-stu-id="3acdf-161">Reboot required or not?</span></span>|
|<span data-ttu-id="3acdf-162">fullScanRequired</span><span class="sxs-lookup"><span data-stu-id="3acdf-162">fullScanRequired</span></span>|<span data-ttu-id="3acdf-163">Booliano</span><span class="sxs-lookup"><span data-stu-id="3acdf-163">Boolean</span></span>|<span data-ttu-id="3acdf-164">Verificação completa necessária ou não?</span><span class="sxs-lookup"><span data-stu-id="3acdf-164">Full scan required or not?</span></span>|
|<span data-ttu-id="3acdf-165">engineVersion</span><span class="sxs-lookup"><span data-stu-id="3acdf-165">engineVersion</span></span>|<span data-ttu-id="3acdf-166">String</span><span class="sxs-lookup"><span data-stu-id="3acdf-166">String</span></span>|<span data-ttu-id="3acdf-167">Versão atual do mecanismo do Endpoint Protection</span><span class="sxs-lookup"><span data-stu-id="3acdf-167">Current endpoint protection engine's version</span></span>|
|<span data-ttu-id="3acdf-168">signatureVersion</span><span class="sxs-lookup"><span data-stu-id="3acdf-168">signatureVersion</span></span>|<span data-ttu-id="3acdf-169">String</span><span class="sxs-lookup"><span data-stu-id="3acdf-169">String</span></span>|<span data-ttu-id="3acdf-170">Versão atual de definições de malware</span><span class="sxs-lookup"><span data-stu-id="3acdf-170">Current malware definitions version</span></span>|
|<span data-ttu-id="3acdf-171">antiMalwareVersion</span><span class="sxs-lookup"><span data-stu-id="3acdf-171">antiMalwareVersion</span></span>|<span data-ttu-id="3acdf-172">String</span><span class="sxs-lookup"><span data-stu-id="3acdf-172">String</span></span>|<span data-ttu-id="3acdf-173">Versão Antimalware atual</span><span class="sxs-lookup"><span data-stu-id="3acdf-173">Current anti malware version</span></span>|
|<span data-ttu-id="3acdf-174">lastQuickScanDateTime</span><span class="sxs-lookup"><span data-stu-id="3acdf-174">lastQuickScanDateTime</span></span>|<span data-ttu-id="3acdf-175">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3acdf-175">DateTimeOffset</span></span>|<span data-ttu-id="3acdf-176">Data e hora da última verificação rápida</span><span class="sxs-lookup"><span data-stu-id="3acdf-176">Last quick scan datetime</span></span>|
|<span data-ttu-id="3acdf-177">lastFullScanDateTime</span><span class="sxs-lookup"><span data-stu-id="3acdf-177">lastFullScanDateTime</span></span>|<span data-ttu-id="3acdf-178">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3acdf-178">DateTimeOffset</span></span>|<span data-ttu-id="3acdf-179">Data e hora da última verificação rápida</span><span class="sxs-lookup"><span data-stu-id="3acdf-179">Last quick scan datetime</span></span>|
|<span data-ttu-id="3acdf-180">lastQuickScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="3acdf-180">lastQuickScanSignatureVersion</span></span>|<span data-ttu-id="3acdf-181">String</span><span class="sxs-lookup"><span data-stu-id="3acdf-181">String</span></span>|<span data-ttu-id="3acdf-182">Versão da última assinatura de verificação rápida</span><span class="sxs-lookup"><span data-stu-id="3acdf-182">Last quick scan signature version</span></span>|
|<span data-ttu-id="3acdf-183">lastFullScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="3acdf-183">lastFullScanSignatureVersion</span></span>|<span data-ttu-id="3acdf-184">String</span><span class="sxs-lookup"><span data-stu-id="3acdf-184">String</span></span>|<span data-ttu-id="3acdf-185">Versão da última assinatura de verificação completa</span><span class="sxs-lookup"><span data-stu-id="3acdf-185">Last full scan signature version</span></span>|
|<span data-ttu-id="3acdf-186">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="3acdf-186">lastReportedDateTime</span></span>|<span data-ttu-id="3acdf-187">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3acdf-187">DateTimeOffset</span></span>|<span data-ttu-id="3acdf-188">Hora do último status de integridade do dispositivo relatado</span><span class="sxs-lookup"><span data-stu-id="3acdf-188">Last device health status reported time</span></span>|
|<span data-ttu-id="3acdf-189">productStatus</span><span class="sxs-lookup"><span data-stu-id="3acdf-189">productStatus</span></span>|[<span data-ttu-id="3acdf-190">windowsDefenderProductStatus</span><span class="sxs-lookup"><span data-stu-id="3acdf-190">windowsDefenderProductStatus</span></span>](../resources/intune-devices-windowsdefenderproductstatus.md)|<span data-ttu-id="3acdf-191">Status do produto do Windows Defender antivírus.</span><span class="sxs-lookup"><span data-stu-id="3acdf-191">Product Status of Windows Defender Antivirus.</span></span> <span data-ttu-id="3acdf-192">Os valores possíveis são:,,,,,,,,,,,,,,, `noStatus` `serviceNotRunning` `serviceStartedWithoutMalwareProtection` `pendingFullScanDueToThreatAction` `pendingRebootDueToThreatAction` `pendingManualStepsDueToThreatAction` `avSignaturesOutOfDate` `asSignaturesOutOfDate` `noQuickScanHappenedForSpecifiedPeriod` `noFullScanHappenedForSpecifiedPeriod` `systemInitiatedScanInProgress` `systemInitiatedCleanInProgress` `samplesPendingSubmission` `productRunningInEvaluationMode` `productRunningInNonGenuineMode` `productExpired` `offlineScanRequired` , `serviceShutdownAsPartOfSystemShutdown` , `threatRemediationFailedCritically` , `threatRemediationFailedNonCritically` `noStatusFlagsSet` `platformOutOfDate` `platformUpdateInProgress` `platformAboutToBeOutdated` `signatureOrPlatformEndOfLifeIsPastOrIsImpending` `windowsSModeSignaturesInUseOnNonWin10SInstall` ,,,,,,,,,,,,,,,.</span><span class="sxs-lookup"><span data-stu-id="3acdf-192">Possible values are: `noStatus`, `serviceNotRunning`, `serviceStartedWithoutMalwareProtection`, `pendingFullScanDueToThreatAction`, `pendingRebootDueToThreatAction`, `pendingManualStepsDueToThreatAction`, `avSignaturesOutOfDate`, `asSignaturesOutOfDate`, `noQuickScanHappenedForSpecifiedPeriod`, `noFullScanHappenedForSpecifiedPeriod`, `systemInitiatedScanInProgress`, `systemInitiatedCleanInProgress`, `samplesPendingSubmission`, `productRunningInEvaluationMode`, `productRunningInNonGenuineMode`, `productExpired`, `offlineScanRequired`, `serviceShutdownAsPartOfSystemShutdown`, `threatRemediationFailedCritically`, `threatRemediationFailedNonCritically`, `noStatusFlagsSet`, `platformOutOfDate`, `platformUpdateInProgress`, `platformAboutToBeOutdated`, `signatureOrPlatformEndOfLifeIsPastOrIsImpending`, `windowsSModeSignaturesInUseOnNonWin10SInstall`.</span></span>|
|<span data-ttu-id="3acdf-193">isVirtualMachine</span><span class="sxs-lookup"><span data-stu-id="3acdf-193">isVirtualMachine</span></span>|<span data-ttu-id="3acdf-194">Booliano</span><span class="sxs-lookup"><span data-stu-id="3acdf-194">Boolean</span></span>|<span data-ttu-id="3acdf-195">Indica se o dispositivo é uma máquina virtual.</span><span class="sxs-lookup"><span data-stu-id="3acdf-195">Indicates whether the device is a virtual machine.</span></span>|
|<span data-ttu-id="3acdf-196">tamperProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="3acdf-196">tamperProtectionEnabled</span></span>|<span data-ttu-id="3acdf-197">Booliano</span><span class="sxs-lookup"><span data-stu-id="3acdf-197">Boolean</span></span>|<span data-ttu-id="3acdf-198">Indica se o recurso proteção de violação do Windows Defender está habilitado.</span><span class="sxs-lookup"><span data-stu-id="3acdf-198">Indicates whether the Windows Defender tamper protection feature is enabled.</span></span>|



## <a name="response"></a><span data-ttu-id="3acdf-199">Resposta</span><span class="sxs-lookup"><span data-stu-id="3acdf-199">Response</span></span>
<span data-ttu-id="3acdf-200">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [windowsprotectionstate foi](../resources/intune-devices-windowsprotectionstate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3acdf-200">If successful, this method returns a `200 OK` response code and an updated [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3acdf-201">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3acdf-201">Example</span></span>

### <a name="request"></a><span data-ttu-id="3acdf-202">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3acdf-202">Request</span></span>
<span data-ttu-id="3acdf-203">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3acdf-203">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/windowsProtectionState
Content-type: application/json
Content-length: 971

{
  "@odata.type": "#microsoft.graph.windowsProtectionState",
  "malwareProtectionEnabled": true,
  "deviceState": "fullScanPending",
  "realTimeProtectionEnabled": true,
  "networkInspectionSystemEnabled": true,
  "quickScanOverdue": true,
  "fullScanOverdue": true,
  "signatureUpdateOverdue": true,
  "rebootRequired": true,
  "fullScanRequired": true,
  "engineVersion": "Engine Version value",
  "signatureVersion": "Signature Version value",
  "antiMalwareVersion": "Anti Malware Version value",
  "lastQuickScanDateTime": "2016-12-31T23:58:27.5900669-08:00",
  "lastFullScanDateTime": "2017-01-01T00:01:44.9405639-08:00",
  "lastQuickScanSignatureVersion": "Last Quick Scan Signature Version value",
  "lastFullScanSignatureVersion": "Last Full Scan Signature Version value",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "productStatus": "serviceNotRunning",
  "isVirtualMachine": true,
  "tamperProtectionEnabled": true
}
```

### <a name="response"></a><span data-ttu-id="3acdf-204">Resposta</span><span class="sxs-lookup"><span data-stu-id="3acdf-204">Response</span></span>
<span data-ttu-id="3acdf-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3acdf-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1020

{
  "@odata.type": "#microsoft.graph.windowsProtectionState",
  "id": "1ac6ea5a-ea5a-1ac6-5aea-c61a5aeac61a",
  "malwareProtectionEnabled": true,
  "deviceState": "fullScanPending",
  "realTimeProtectionEnabled": true,
  "networkInspectionSystemEnabled": true,
  "quickScanOverdue": true,
  "fullScanOverdue": true,
  "signatureUpdateOverdue": true,
  "rebootRequired": true,
  "fullScanRequired": true,
  "engineVersion": "Engine Version value",
  "signatureVersion": "Signature Version value",
  "antiMalwareVersion": "Anti Malware Version value",
  "lastQuickScanDateTime": "2016-12-31T23:58:27.5900669-08:00",
  "lastFullScanDateTime": "2017-01-01T00:01:44.9405639-08:00",
  "lastQuickScanSignatureVersion": "Last Quick Scan Signature Version value",
  "lastFullScanSignatureVersion": "Last Full Scan Signature Version value",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "productStatus": "serviceNotRunning",
  "isVirtualMachine": true,
  "tamperProtectionEnabled": true
}
```




