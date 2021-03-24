---
title: Atualizar windowsProtectionState
description: Atualize as propriedades de um objeto windowsProtectionState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2a500c5f1510a28638e58be0ef32d328cc598776
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51135828"
---
# <a name="update-windowsprotectionstate"></a><span data-ttu-id="8bf19-103">Atualizar windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="8bf19-103">Update windowsProtectionState</span></span>

<span data-ttu-id="8bf19-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8bf19-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8bf19-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8bf19-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8bf19-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8bf19-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8bf19-107">Atualize as propriedades de um [objeto windowsProtectionState.](../resources/intune-devices-windowsprotectionstate.md)</span><span class="sxs-lookup"><span data-stu-id="8bf19-107">Update the properties of a [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8bf19-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8bf19-108">Prerequisites</span></span>
<span data-ttu-id="8bf19-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8bf19-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8bf19-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8bf19-111">Permission type</span></span>|<span data-ttu-id="8bf19-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8bf19-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8bf19-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8bf19-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8bf19-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8bf19-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="8bf19-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8bf19-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8bf19-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8bf19-116">Not supported.</span></span>|
|<span data-ttu-id="8bf19-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8bf19-117">Application</span></span>|<span data-ttu-id="8bf19-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8bf19-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8bf19-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8bf19-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/windowsProtectionState
```

## <a name="request-headers"></a><span data-ttu-id="8bf19-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8bf19-120">Request headers</span></span>
|<span data-ttu-id="8bf19-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8bf19-121">Header</span></span>|<span data-ttu-id="8bf19-122">Valor</span><span class="sxs-lookup"><span data-stu-id="8bf19-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8bf19-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8bf19-123">Authorization</span></span>|<span data-ttu-id="8bf19-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8bf19-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8bf19-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8bf19-125">Accept</span></span>|<span data-ttu-id="8bf19-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8bf19-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8bf19-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8bf19-127">Request body</span></span>
<span data-ttu-id="8bf19-128">No corpo da solicitação, fornece uma representação JSON para o [objeto windowsProtectionState.](../resources/intune-devices-windowsprotectionstate.md)</span><span class="sxs-lookup"><span data-stu-id="8bf19-128">In the request body, supply a JSON representation for the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>

<span data-ttu-id="8bf19-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md).</span><span class="sxs-lookup"><span data-stu-id="8bf19-129">The following table shows the properties that are required when you create the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md).</span></span>

|<span data-ttu-id="8bf19-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8bf19-130">Property</span></span>|<span data-ttu-id="8bf19-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="8bf19-131">Type</span></span>|<span data-ttu-id="8bf19-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="8bf19-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8bf19-133">id</span><span class="sxs-lookup"><span data-stu-id="8bf19-133">id</span></span>|<span data-ttu-id="8bf19-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8bf19-134">String</span></span>|<span data-ttu-id="8bf19-135">O Identificador exclusivo do objeto de status de proteção do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8bf19-135">The unique Identifier for the device protection status object.</span></span> <span data-ttu-id="8bf19-136">Esta é a ID do dispositivo</span><span class="sxs-lookup"><span data-stu-id="8bf19-136">This is device id of the device</span></span>|
|<span data-ttu-id="8bf19-137">malwareProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="8bf19-137">malwareProtectionEnabled</span></span>|<span data-ttu-id="8bf19-138">Booleano</span><span class="sxs-lookup"><span data-stu-id="8bf19-138">Boolean</span></span>|<span data-ttu-id="8bf19-139">O anti malware está habilitado ou não</span><span class="sxs-lookup"><span data-stu-id="8bf19-139">Anti malware is enabled or not</span></span>|
|<span data-ttu-id="8bf19-140">deviceState</span><span class="sxs-lookup"><span data-stu-id="8bf19-140">deviceState</span></span>|[<span data-ttu-id="8bf19-141">windowsDeviceHealthState</span><span class="sxs-lookup"><span data-stu-id="8bf19-141">windowsDeviceHealthState</span></span>](../resources/intune-devices-windowsdevicehealthstate.md)|<span data-ttu-id="8bf19-142">Estado do computador (como verificação completa ou pendente ou reinicialização pendente etc.).</span><span class="sxs-lookup"><span data-stu-id="8bf19-142">Computer's state (like clean or pending full scan or pending reboot etc).</span></span> <span data-ttu-id="8bf19-143">Os possíveis valores são: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span><span class="sxs-lookup"><span data-stu-id="8bf19-143">Possible values are: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span></span>|
|<span data-ttu-id="8bf19-144">realTimeProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="8bf19-144">realTimeProtectionEnabled</span></span>|<span data-ttu-id="8bf19-145">Booleano</span><span class="sxs-lookup"><span data-stu-id="8bf19-145">Boolean</span></span>|<span data-ttu-id="8bf19-146">A proteção em tempo real está habilitada ou não?</span><span class="sxs-lookup"><span data-stu-id="8bf19-146">Real time protection is enabled or not?</span></span>|
|<span data-ttu-id="8bf19-147">networkInspectionSystemEnabled</span><span class="sxs-lookup"><span data-stu-id="8bf19-147">networkInspectionSystemEnabled</span></span>|<span data-ttu-id="8bf19-148">Booleano</span><span class="sxs-lookup"><span data-stu-id="8bf19-148">Boolean</span></span>|<span data-ttu-id="8bf19-149">Sistema de inspeção de rede habilitado ou não?</span><span class="sxs-lookup"><span data-stu-id="8bf19-149">Network inspection system enabled or not?</span></span>|
|<span data-ttu-id="8bf19-150">quickScanOverdue</span><span class="sxs-lookup"><span data-stu-id="8bf19-150">quickScanOverdue</span></span>|<span data-ttu-id="8bf19-151">Booleano</span><span class="sxs-lookup"><span data-stu-id="8bf19-151">Boolean</span></span>|<span data-ttu-id="8bf19-152">Verificação rápida atrasada ou não?</span><span class="sxs-lookup"><span data-stu-id="8bf19-152">Quick scan overdue or not?</span></span>|
|<span data-ttu-id="8bf19-153">fullScanOverdue</span><span class="sxs-lookup"><span data-stu-id="8bf19-153">fullScanOverdue</span></span>|<span data-ttu-id="8bf19-154">Booleano</span><span class="sxs-lookup"><span data-stu-id="8bf19-154">Boolean</span></span>|<span data-ttu-id="8bf19-155">Verificação completa atrasada ou não?</span><span class="sxs-lookup"><span data-stu-id="8bf19-155">Full scan overdue or not?</span></span>|
|<span data-ttu-id="8bf19-156">signatureUpdateOverdue</span><span class="sxs-lookup"><span data-stu-id="8bf19-156">signatureUpdateOverdue</span></span>|<span data-ttu-id="8bf19-157">Booleano</span><span class="sxs-lookup"><span data-stu-id="8bf19-157">Boolean</span></span>|<span data-ttu-id="8bf19-158">Assinatura desa datada ou não?</span><span class="sxs-lookup"><span data-stu-id="8bf19-158">Signature out of date or not?</span></span>|
|<span data-ttu-id="8bf19-159">rebootRequired</span><span class="sxs-lookup"><span data-stu-id="8bf19-159">rebootRequired</span></span>|<span data-ttu-id="8bf19-160">Booleano</span><span class="sxs-lookup"><span data-stu-id="8bf19-160">Boolean</span></span>|<span data-ttu-id="8bf19-161">Reiniciar obrigatório ou não?</span><span class="sxs-lookup"><span data-stu-id="8bf19-161">Reboot required or not?</span></span>|
|<span data-ttu-id="8bf19-162">fullScanRequired</span><span class="sxs-lookup"><span data-stu-id="8bf19-162">fullScanRequired</span></span>|<span data-ttu-id="8bf19-163">Booleano</span><span class="sxs-lookup"><span data-stu-id="8bf19-163">Boolean</span></span>|<span data-ttu-id="8bf19-164">Verificação completa necessária ou não?</span><span class="sxs-lookup"><span data-stu-id="8bf19-164">Full scan required or not?</span></span>|
|<span data-ttu-id="8bf19-165">engineVersion</span><span class="sxs-lookup"><span data-stu-id="8bf19-165">engineVersion</span></span>|<span data-ttu-id="8bf19-166">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8bf19-166">String</span></span>|<span data-ttu-id="8bf19-167">Versão atual do mecanismo de proteção de ponto de extremidade</span><span class="sxs-lookup"><span data-stu-id="8bf19-167">Current endpoint protection engine's version</span></span>|
|<span data-ttu-id="8bf19-168">signatureVersion</span><span class="sxs-lookup"><span data-stu-id="8bf19-168">signatureVersion</span></span>|<span data-ttu-id="8bf19-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8bf19-169">String</span></span>|<span data-ttu-id="8bf19-170">Versão atual das definições de malware</span><span class="sxs-lookup"><span data-stu-id="8bf19-170">Current malware definitions version</span></span>|
|<span data-ttu-id="8bf19-171">antiMalwareVersion</span><span class="sxs-lookup"><span data-stu-id="8bf19-171">antiMalwareVersion</span></span>|<span data-ttu-id="8bf19-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8bf19-172">String</span></span>|<span data-ttu-id="8bf19-173">Versão anti malware atual</span><span class="sxs-lookup"><span data-stu-id="8bf19-173">Current anti malware version</span></span>|
|<span data-ttu-id="8bf19-174">lastQuickScanDateTime</span><span class="sxs-lookup"><span data-stu-id="8bf19-174">lastQuickScanDateTime</span></span>|<span data-ttu-id="8bf19-175">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8bf19-175">DateTimeOffset</span></span>|<span data-ttu-id="8bf19-176">Data da última verificação rápida</span><span class="sxs-lookup"><span data-stu-id="8bf19-176">Last quick scan datetime</span></span>|
|<span data-ttu-id="8bf19-177">lastFullScanDateTime</span><span class="sxs-lookup"><span data-stu-id="8bf19-177">lastFullScanDateTime</span></span>|<span data-ttu-id="8bf19-178">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8bf19-178">DateTimeOffset</span></span>|<span data-ttu-id="8bf19-179">Data da última verificação rápida</span><span class="sxs-lookup"><span data-stu-id="8bf19-179">Last quick scan datetime</span></span>|
|<span data-ttu-id="8bf19-180">lastQuickScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="8bf19-180">lastQuickScanSignatureVersion</span></span>|<span data-ttu-id="8bf19-181">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8bf19-181">String</span></span>|<span data-ttu-id="8bf19-182">Última versão de assinatura de verificação rápida</span><span class="sxs-lookup"><span data-stu-id="8bf19-182">Last quick scan signature version</span></span>|
|<span data-ttu-id="8bf19-183">lastFullScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="8bf19-183">lastFullScanSignatureVersion</span></span>|<span data-ttu-id="8bf19-184">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8bf19-184">String</span></span>|<span data-ttu-id="8bf19-185">Última versão de assinatura de verificação completa</span><span class="sxs-lookup"><span data-stu-id="8bf19-185">Last full scan signature version</span></span>|
|<span data-ttu-id="8bf19-186">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="8bf19-186">lastReportedDateTime</span></span>|<span data-ttu-id="8bf19-187">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8bf19-187">DateTimeOffset</span></span>|<span data-ttu-id="8bf19-188">Tempo de notificado do último status de saúde do dispositivo</span><span class="sxs-lookup"><span data-stu-id="8bf19-188">Last device health status reported time</span></span>|
|<span data-ttu-id="8bf19-189">productStatus</span><span class="sxs-lookup"><span data-stu-id="8bf19-189">productStatus</span></span>|[<span data-ttu-id="8bf19-190">windowsDefenderProductStatus</span><span class="sxs-lookup"><span data-stu-id="8bf19-190">windowsDefenderProductStatus</span></span>](../resources/intune-devices-windowsdefenderproductstatus.md)|<span data-ttu-id="8bf19-191">Status do produto do Windows Defender Antivírus.</span><span class="sxs-lookup"><span data-stu-id="8bf19-191">Product Status of Windows Defender Antivirus.</span></span> <span data-ttu-id="8bf19-192">Os valores possíveis são: `noStatus` , , , , , , , , `serviceNotRunning` `serviceStartedWithoutMalwareProtection` `pendingFullScanDueToThreatAction` `pendingRebootDueToThreatAction` `pendingManualStepsDueToThreatAction` `avSignaturesOutOfDate` `asSignaturesOutOfDate` `noQuickScanHappenedForSpecifiedPeriod` `noFullScanHappenedForSpecifiedPeriod` `systemInitiatedScanInProgress` `systemInitiatedCleanInProgress` `samplesPendingSubmission` `productRunningInEvaluationMode` , `productRunningInNonGenuineMode` `productExpired` `offlineScanRequired` `serviceShutdownAsPartOfSystemShutdown` `threatRemediationFailedCritically` `threatRemediationFailedNonCritically` `noStatusFlagsSet` `platformOutOfDate` `platformUpdateInProgress` `platformAboutToBeOutdated` `signatureOrPlatformEndOfLifeIsPastOrIsImpending` `windowsSModeSignaturesInUseOnNonWin10SInstall`</span><span class="sxs-lookup"><span data-stu-id="8bf19-192">Possible values are: `noStatus`, `serviceNotRunning`, `serviceStartedWithoutMalwareProtection`, `pendingFullScanDueToThreatAction`, `pendingRebootDueToThreatAction`, `pendingManualStepsDueToThreatAction`, `avSignaturesOutOfDate`, `asSignaturesOutOfDate`, `noQuickScanHappenedForSpecifiedPeriod`, `noFullScanHappenedForSpecifiedPeriod`, `systemInitiatedScanInProgress`, `systemInitiatedCleanInProgress`, `samplesPendingSubmission`, `productRunningInEvaluationMode`, `productRunningInNonGenuineMode`, `productExpired`, `offlineScanRequired`, `serviceShutdownAsPartOfSystemShutdown`, `threatRemediationFailedCritically`, `threatRemediationFailedNonCritically`, `noStatusFlagsSet`, `platformOutOfDate`, `platformUpdateInProgress`, `platformAboutToBeOutdated`, `signatureOrPlatformEndOfLifeIsPastOrIsImpending`, `windowsSModeSignaturesInUseOnNonWin10SInstall`.</span></span>|
|<span data-ttu-id="8bf19-193">isVirtualMachine</span><span class="sxs-lookup"><span data-stu-id="8bf19-193">isVirtualMachine</span></span>|<span data-ttu-id="8bf19-194">Booleano</span><span class="sxs-lookup"><span data-stu-id="8bf19-194">Boolean</span></span>|<span data-ttu-id="8bf19-195">Indica se o dispositivo é uma máquina virtual.</span><span class="sxs-lookup"><span data-stu-id="8bf19-195">Indicates whether the device is a virtual machine.</span></span>|
|<span data-ttu-id="8bf19-196">tamperProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="8bf19-196">tamperProtectionEnabled</span></span>|<span data-ttu-id="8bf19-197">Booleano</span><span class="sxs-lookup"><span data-stu-id="8bf19-197">Boolean</span></span>|<span data-ttu-id="8bf19-198">Indica se o recurso Windows Defender proteção contra adulteração está habilitado.</span><span class="sxs-lookup"><span data-stu-id="8bf19-198">Indicates whether the Windows Defender tamper protection feature is enabled.</span></span>|



## <a name="response"></a><span data-ttu-id="8bf19-199">Resposta</span><span class="sxs-lookup"><span data-stu-id="8bf19-199">Response</span></span>
<span data-ttu-id="8bf19-200">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8bf19-200">If successful, this method returns a `200 OK` response code and an updated [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8bf19-201">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8bf19-201">Example</span></span>

### <a name="request"></a><span data-ttu-id="8bf19-202">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8bf19-202">Request</span></span>
<span data-ttu-id="8bf19-203">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8bf19-203">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8bf19-204">Resposta</span><span class="sxs-lookup"><span data-stu-id="8bf19-204">Response</span></span>
<span data-ttu-id="8bf19-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8bf19-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




