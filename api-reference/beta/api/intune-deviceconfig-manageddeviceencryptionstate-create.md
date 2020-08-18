---
title: Criar managedDeviceEncryptionState
description: Criar um novo objeto managedDeviceEncryptionState.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4498cf04a586cb5e758f8e2213eb956765fb803f
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/18/2020
ms.locfileid: "46790921"
---
# <a name="create-manageddeviceencryptionstate"></a><span data-ttu-id="5005e-103">Criar managedDeviceEncryptionState</span><span class="sxs-lookup"><span data-stu-id="5005e-103">Create managedDeviceEncryptionState</span></span>

<span data-ttu-id="5005e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5005e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5005e-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5005e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5005e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5005e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5005e-107">Criar um novo objeto [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) .</span><span class="sxs-lookup"><span data-stu-id="5005e-107">Create a new [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5005e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5005e-108">Prerequisites</span></span>
<span data-ttu-id="5005e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5005e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5005e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5005e-111">Permission type</span></span>|<span data-ttu-id="5005e-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5005e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5005e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5005e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5005e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5005e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5005e-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5005e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5005e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5005e-116">Not supported.</span></span>|
|<span data-ttu-id="5005e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5005e-117">Application</span></span>|<span data-ttu-id="5005e-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5005e-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5005e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5005e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDeviceEncryptionStates
```

## <a name="request-headers"></a><span data-ttu-id="5005e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5005e-120">Request headers</span></span>
|<span data-ttu-id="5005e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5005e-121">Header</span></span>|<span data-ttu-id="5005e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="5005e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5005e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="5005e-123">Authorization</span></span>|<span data-ttu-id="5005e-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5005e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5005e-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5005e-125">Accept</span></span>|<span data-ttu-id="5005e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5005e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5005e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5005e-127">Request body</span></span>
<span data-ttu-id="5005e-128">No corpo da solicitação, forneça uma representação JSON do objeto managedDeviceEncryptionState.</span><span class="sxs-lookup"><span data-stu-id="5005e-128">In the request body, supply a JSON representation for the managedDeviceEncryptionState object.</span></span>

<span data-ttu-id="5005e-129">A tabela a seguir mostra as propriedades que são necessárias ao criar managedDeviceEncryptionState.</span><span class="sxs-lookup"><span data-stu-id="5005e-129">The following table shows the properties that are required when you create the managedDeviceEncryptionState.</span></span>

|<span data-ttu-id="5005e-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5005e-130">Property</span></span>|<span data-ttu-id="5005e-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="5005e-131">Type</span></span>|<span data-ttu-id="5005e-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="5005e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5005e-133">id</span><span class="sxs-lookup"><span data-stu-id="5005e-133">id</span></span>|<span data-ttu-id="5005e-134">String</span><span class="sxs-lookup"><span data-stu-id="5005e-134">String</span></span>|<span data-ttu-id="5005e-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="5005e-135">Key of the entity.</span></span>|
|<span data-ttu-id="5005e-136">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="5005e-136">userPrincipalName</span></span>|<span data-ttu-id="5005e-137">String</span><span class="sxs-lookup"><span data-stu-id="5005e-137">String</span></span>|<span data-ttu-id="5005e-138">Nome de usuário</span><span class="sxs-lookup"><span data-stu-id="5005e-138">User name</span></span>|
|<span data-ttu-id="5005e-139">deviceType</span><span class="sxs-lookup"><span data-stu-id="5005e-139">deviceType</span></span>|[<span data-ttu-id="5005e-140">deviceTypes</span><span class="sxs-lookup"><span data-stu-id="5005e-140">deviceTypes</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="5005e-141">Plataforma do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5005e-141">Platform of the device.</span></span> <span data-ttu-id="5005e-142">Os valores possíveis são:,,,,,,,,,,,,,,,,,,,, `desktop` `windowsRT` `winMO6` `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer` , `unix` , `macMDM` ,, `holoLens` `surfaceHub` , `androidForWork` `androidEnterprise` `blackberry` `palm` `unknown` ,,,,,.</span><span class="sxs-lookup"><span data-stu-id="5005e-142">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="5005e-143">osVersion</span><span class="sxs-lookup"><span data-stu-id="5005e-143">osVersion</span></span>|<span data-ttu-id="5005e-144">String</span><span class="sxs-lookup"><span data-stu-id="5005e-144">String</span></span>|<span data-ttu-id="5005e-145">Versão do sistema operacional do dispositivo</span><span class="sxs-lookup"><span data-stu-id="5005e-145">Operating system version of the device</span></span>|
|<span data-ttu-id="5005e-146">tpmSpecificationVersion</span><span class="sxs-lookup"><span data-stu-id="5005e-146">tpmSpecificationVersion</span></span>|<span data-ttu-id="5005e-147">String</span><span class="sxs-lookup"><span data-stu-id="5005e-147">String</span></span>|<span data-ttu-id="5005e-148">Versão do TPM do dispositivo</span><span class="sxs-lookup"><span data-stu-id="5005e-148">Device TPM Version</span></span>|
|<span data-ttu-id="5005e-149">deviceName</span><span class="sxs-lookup"><span data-stu-id="5005e-149">deviceName</span></span>|<span data-ttu-id="5005e-150">String</span><span class="sxs-lookup"><span data-stu-id="5005e-150">String</span></span>|<span data-ttu-id="5005e-151">Nome do dispositivo</span><span class="sxs-lookup"><span data-stu-id="5005e-151">Device name</span></span>|
|<span data-ttu-id="5005e-152">encryptionReadinessState</span><span class="sxs-lookup"><span data-stu-id="5005e-152">encryptionReadinessState</span></span>|[<span data-ttu-id="5005e-153">encryptionReadinessState</span><span class="sxs-lookup"><span data-stu-id="5005e-153">encryptionReadinessState</span></span>](../resources/intune-deviceconfig-encryptionreadinessstate.md)|<span data-ttu-id="5005e-154">Estado de preparação de criptografia.</span><span class="sxs-lookup"><span data-stu-id="5005e-154">Encryption readiness state.</span></span> <span data-ttu-id="5005e-155">Os valores possíveis são: `notReady` e `ready`.</span><span class="sxs-lookup"><span data-stu-id="5005e-155">Possible values are: `notReady`, `ready`.</span></span>|
|<span data-ttu-id="5005e-156">encryptionState</span><span class="sxs-lookup"><span data-stu-id="5005e-156">encryptionState</span></span>|[<span data-ttu-id="5005e-157">encryptionState</span><span class="sxs-lookup"><span data-stu-id="5005e-157">encryptionState</span></span>](../resources/intune-deviceconfig-encryptionstate.md)|<span data-ttu-id="5005e-158">Estado de criptografia do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5005e-158">Device encryption state.</span></span> <span data-ttu-id="5005e-159">Os valores possíveis são: `notEncrypted` e `encrypted`.</span><span class="sxs-lookup"><span data-stu-id="5005e-159">Possible values are: `notEncrypted`, `encrypted`.</span></span>|
|<span data-ttu-id="5005e-160">encryptionPolicySettingState</span><span class="sxs-lookup"><span data-stu-id="5005e-160">encryptionPolicySettingState</span></span>|[<span data-ttu-id="5005e-161">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="5005e-161">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="5005e-162">Estado da configuração da política de criptografia.</span><span class="sxs-lookup"><span data-stu-id="5005e-162">Encryption policy setting state.</span></span> <span data-ttu-id="5005e-163">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="5005e-163">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="5005e-164">advancedBitLockerStates</span><span class="sxs-lookup"><span data-stu-id="5005e-164">advancedBitLockerStates</span></span>|[<span data-ttu-id="5005e-165">advancedBitLockerState</span><span class="sxs-lookup"><span data-stu-id="5005e-165">advancedBitLockerState</span></span>](../resources/intune-deviceconfig-advancedbitlockerstate.md)|<span data-ttu-id="5005e-166">Estado do BitLocker avançado.</span><span class="sxs-lookup"><span data-stu-id="5005e-166">Advanced BitLocker State.</span></span> <span data-ttu-id="5005e-167">Os valores possíveis são:, `success` `noUserConsent` , `osVolumeEncryptionMethodMismatch` , `osVolumeTpmRequired` , `osVolumeTpmOnlyRequired` , `osVolumeTpmPinRequired` ,,,,,,,,,,,,,,, `osVolumeTpmStartupKeyRequired` `osVolumeTpmPinStartupKeyRequired` `osVolumeUnprotected` `recoveryKeyBackupFailed` `fixedDriveNotEncrypted` `fixedDriveEncryptionMethodMismatch` `loggedOnUserNonAdmin` , `windowsRecoveryEnvironmentNotConfigured` , `tpmNotAvailable` , `tpmNotReady` , `networkError` .</span><span class="sxs-lookup"><span data-stu-id="5005e-167">Possible values are: `success`, `noUserConsent`, `osVolumeEncryptionMethodMismatch`, `osVolumeTpmRequired`, `osVolumeTpmOnlyRequired`, `osVolumeTpmPinRequired`, `osVolumeTpmStartupKeyRequired`, `osVolumeTpmPinStartupKeyRequired`, `osVolumeUnprotected`, `recoveryKeyBackupFailed`, `fixedDriveNotEncrypted`, `fixedDriveEncryptionMethodMismatch`, `loggedOnUserNonAdmin`, `windowsRecoveryEnvironmentNotConfigured`, `tpmNotAvailable`, `tpmNotReady`, `networkError`.</span></span>|
|<span data-ttu-id="5005e-168">fileVaultStates</span><span class="sxs-lookup"><span data-stu-id="5005e-168">fileVaultStates</span></span>|[<span data-ttu-id="5005e-169">fileVaultState</span><span class="sxs-lookup"><span data-stu-id="5005e-169">fileVaultState</span></span>](../resources/intune-deviceconfig-filevaultstate.md)|<span data-ttu-id="5005e-170">Estado FileVault.</span><span class="sxs-lookup"><span data-stu-id="5005e-170">FileVault State.</span></span> <span data-ttu-id="5005e-171">Os valores possíveis são: `success`, `driveEncryptedByUser`, `userDeferredEncryption`, `escrowNotEnabled`.</span><span class="sxs-lookup"><span data-stu-id="5005e-171">Possible values are: `success`, `driveEncryptedByUser`, `userDeferredEncryption`, `escrowNotEnabled`.</span></span>|
|<span data-ttu-id="5005e-172">policyDetails</span><span class="sxs-lookup"><span data-stu-id="5005e-172">policyDetails</span></span>|<span data-ttu-id="5005e-173">coleção [encryptionReportPolicyDetails](../resources/intune-deviceconfig-encryptionreportpolicydetails.md)</span><span class="sxs-lookup"><span data-stu-id="5005e-173">[encryptionReportPolicyDetails](../resources/intune-deviceconfig-encryptionreportpolicydetails.md) collection</span></span>|<span data-ttu-id="5005e-174">Detalhes da política</span><span class="sxs-lookup"><span data-stu-id="5005e-174">Policy Details</span></span>|



## <a name="response"></a><span data-ttu-id="5005e-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="5005e-175">Response</span></span>
<span data-ttu-id="5005e-176">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5005e-176">If successful, this method returns a `201 Created` response code and a [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5005e-177">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5005e-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="5005e-178">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5005e-178">Request</span></span>
<span data-ttu-id="5005e-179">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5005e-179">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDeviceEncryptionStates
Content-type: application/json
Content-length: 704

{
  "@odata.type": "#microsoft.graph.managedDeviceEncryptionState",
  "userPrincipalName": "User Principal Name value",
  "deviceType": "windowsRT",
  "osVersion": "Os Version value",
  "tpmSpecificationVersion": "Tpm Specification Version value",
  "deviceName": "Device Name value",
  "encryptionReadinessState": "ready",
  "encryptionState": "encrypted",
  "encryptionPolicySettingState": "notApplicable",
  "advancedBitLockerStates": "noUserConsent",
  "fileVaultStates": "driveEncryptedByUser",
  "policyDetails": [
    {
      "@odata.type": "microsoft.graph.encryptionReportPolicyDetails",
      "policyId": "Policy Id value",
      "policyName": "Policy Name value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="5005e-180">Resposta</span><span class="sxs-lookup"><span data-stu-id="5005e-180">Response</span></span>
<span data-ttu-id="5005e-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5005e-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 753

{
  "@odata.type": "#microsoft.graph.managedDeviceEncryptionState",
  "id": "f09b4ab6-4ab6-f09b-b64a-9bf0b64a9bf0",
  "userPrincipalName": "User Principal Name value",
  "deviceType": "windowsRT",
  "osVersion": "Os Version value",
  "tpmSpecificationVersion": "Tpm Specification Version value",
  "deviceName": "Device Name value",
  "encryptionReadinessState": "ready",
  "encryptionState": "encrypted",
  "encryptionPolicySettingState": "notApplicable",
  "advancedBitLockerStates": "noUserConsent",
  "fileVaultStates": "driveEncryptedByUser",
  "policyDetails": [
    {
      "@odata.type": "microsoft.graph.encryptionReportPolicyDetails",
      "policyId": "Policy Id value",
      "policyName": "Policy Name value"
    }
  ]
}
```



