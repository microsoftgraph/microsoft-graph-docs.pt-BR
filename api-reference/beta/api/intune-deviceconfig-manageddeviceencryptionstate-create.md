---
title: Criar managedDeviceEncryptionState
description: Criar um novo objeto managedDeviceEncryptionState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 495d40ae9da2c11845b99a65d7dcdfad28e02a6f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48086212"
---
# <a name="create-manageddeviceencryptionstate"></a><span data-ttu-id="c7c60-103">Criar managedDeviceEncryptionState</span><span class="sxs-lookup"><span data-stu-id="c7c60-103">Create managedDeviceEncryptionState</span></span>

<span data-ttu-id="c7c60-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c7c60-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c7c60-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c7c60-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c7c60-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c7c60-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c7c60-107">Criar um novo objeto [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) .</span><span class="sxs-lookup"><span data-stu-id="c7c60-107">Create a new [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c7c60-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c7c60-108">Prerequisites</span></span>
<span data-ttu-id="c7c60-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c7c60-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c7c60-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c7c60-111">Permission type</span></span>|<span data-ttu-id="c7c60-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c7c60-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c7c60-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c7c60-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c7c60-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7c60-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c7c60-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c7c60-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c7c60-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c7c60-116">Not supported.</span></span>|
|<span data-ttu-id="c7c60-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c7c60-117">Application</span></span>|<span data-ttu-id="c7c60-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7c60-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c7c60-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c7c60-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDeviceEncryptionStates
```

## <a name="request-headers"></a><span data-ttu-id="c7c60-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c7c60-120">Request headers</span></span>
|<span data-ttu-id="c7c60-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c7c60-121">Header</span></span>|<span data-ttu-id="c7c60-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c7c60-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c7c60-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c7c60-123">Authorization</span></span>|<span data-ttu-id="c7c60-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c7c60-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c7c60-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c7c60-125">Accept</span></span>|<span data-ttu-id="c7c60-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c7c60-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c7c60-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c7c60-127">Request body</span></span>
<span data-ttu-id="c7c60-128">No corpo da solicitação, forneça uma representação JSON do objeto managedDeviceEncryptionState.</span><span class="sxs-lookup"><span data-stu-id="c7c60-128">In the request body, supply a JSON representation for the managedDeviceEncryptionState object.</span></span>

<span data-ttu-id="c7c60-129">A tabela a seguir mostra as propriedades que são necessárias ao criar managedDeviceEncryptionState.</span><span class="sxs-lookup"><span data-stu-id="c7c60-129">The following table shows the properties that are required when you create the managedDeviceEncryptionState.</span></span>

|<span data-ttu-id="c7c60-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c7c60-130">Property</span></span>|<span data-ttu-id="c7c60-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="c7c60-131">Type</span></span>|<span data-ttu-id="c7c60-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="c7c60-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7c60-133">id</span><span class="sxs-lookup"><span data-stu-id="c7c60-133">id</span></span>|<span data-ttu-id="c7c60-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c7c60-134">String</span></span>|<span data-ttu-id="c7c60-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="c7c60-135">Key of the entity.</span></span>|
|<span data-ttu-id="c7c60-136">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c7c60-136">userPrincipalName</span></span>|<span data-ttu-id="c7c60-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c7c60-137">String</span></span>|<span data-ttu-id="c7c60-138">Nome de usuário</span><span class="sxs-lookup"><span data-stu-id="c7c60-138">User name</span></span>|
|<span data-ttu-id="c7c60-139">deviceType</span><span class="sxs-lookup"><span data-stu-id="c7c60-139">deviceType</span></span>|[<span data-ttu-id="c7c60-140">deviceType</span><span class="sxs-lookup"><span data-stu-id="c7c60-140">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="c7c60-141">Plataforma do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c7c60-141">Platform of the device.</span></span> <span data-ttu-id="c7c60-142">Os valores possíveis são:,,,,,,,,,,,,,,,,,,,, `desktop` `windowsRT` `winMO6` `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer` , `unix` , `macMDM` ,, `holoLens` `surfaceHub` , `androidForWork` `androidEnterprise` `blackberry` `palm` `unknown` ,,,,,.</span><span class="sxs-lookup"><span data-stu-id="c7c60-142">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="c7c60-143">osVersion</span><span class="sxs-lookup"><span data-stu-id="c7c60-143">osVersion</span></span>|<span data-ttu-id="c7c60-144">String</span><span class="sxs-lookup"><span data-stu-id="c7c60-144">String</span></span>|<span data-ttu-id="c7c60-145">Versão do sistema operacional do dispositivo</span><span class="sxs-lookup"><span data-stu-id="c7c60-145">Operating system version of the device</span></span>|
|<span data-ttu-id="c7c60-146">tpmSpecificationVersion</span><span class="sxs-lookup"><span data-stu-id="c7c60-146">tpmSpecificationVersion</span></span>|<span data-ttu-id="c7c60-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c7c60-147">String</span></span>|<span data-ttu-id="c7c60-148">Versão do TPM do dispositivo</span><span class="sxs-lookup"><span data-stu-id="c7c60-148">Device TPM Version</span></span>|
|<span data-ttu-id="c7c60-149">deviceName</span><span class="sxs-lookup"><span data-stu-id="c7c60-149">deviceName</span></span>|<span data-ttu-id="c7c60-150">String</span><span class="sxs-lookup"><span data-stu-id="c7c60-150">String</span></span>|<span data-ttu-id="c7c60-151">Nome do dispositivo</span><span class="sxs-lookup"><span data-stu-id="c7c60-151">Device name</span></span>|
|<span data-ttu-id="c7c60-152">encryptionReadinessState</span><span class="sxs-lookup"><span data-stu-id="c7c60-152">encryptionReadinessState</span></span>|[<span data-ttu-id="c7c60-153">encryptionReadinessState</span><span class="sxs-lookup"><span data-stu-id="c7c60-153">encryptionReadinessState</span></span>](../resources/intune-deviceconfig-encryptionreadinessstate.md)|<span data-ttu-id="c7c60-154">Estado de preparação de criptografia.</span><span class="sxs-lookup"><span data-stu-id="c7c60-154">Encryption readiness state.</span></span> <span data-ttu-id="c7c60-155">Os valores possíveis são: `notReady` e `ready`.</span><span class="sxs-lookup"><span data-stu-id="c7c60-155">Possible values are: `notReady`, `ready`.</span></span>|
|<span data-ttu-id="c7c60-156">encryptionState</span><span class="sxs-lookup"><span data-stu-id="c7c60-156">encryptionState</span></span>|[<span data-ttu-id="c7c60-157">encryptionState</span><span class="sxs-lookup"><span data-stu-id="c7c60-157">encryptionState</span></span>](../resources/intune-deviceconfig-encryptionstate.md)|<span data-ttu-id="c7c60-158">Estado de criptografia do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c7c60-158">Device encryption state.</span></span> <span data-ttu-id="c7c60-159">Os valores possíveis são: `notEncrypted` e `encrypted`.</span><span class="sxs-lookup"><span data-stu-id="c7c60-159">Possible values are: `notEncrypted`, `encrypted`.</span></span>|
|<span data-ttu-id="c7c60-160">encryptionPolicySettingState</span><span class="sxs-lookup"><span data-stu-id="c7c60-160">encryptionPolicySettingState</span></span>|[<span data-ttu-id="c7c60-161">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="c7c60-161">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="c7c60-162">Estado da configuração da política de criptografia.</span><span class="sxs-lookup"><span data-stu-id="c7c60-162">Encryption policy setting state.</span></span> <span data-ttu-id="c7c60-163">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="c7c60-163">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="c7c60-164">advancedBitLockerStates</span><span class="sxs-lookup"><span data-stu-id="c7c60-164">advancedBitLockerStates</span></span>|[<span data-ttu-id="c7c60-165">advancedBitLockerState</span><span class="sxs-lookup"><span data-stu-id="c7c60-165">advancedBitLockerState</span></span>](../resources/intune-deviceconfig-advancedbitlockerstate.md)|<span data-ttu-id="c7c60-166">Estado do BitLocker avançado.</span><span class="sxs-lookup"><span data-stu-id="c7c60-166">Advanced BitLocker State.</span></span> <span data-ttu-id="c7c60-167">Os valores possíveis são:, `success` `noUserConsent` , `osVolumeEncryptionMethodMismatch` , `osVolumeTpmRequired` , `osVolumeTpmOnlyRequired` , `osVolumeTpmPinRequired` ,,,,,,,,,,,,,,, `osVolumeTpmStartupKeyRequired` `osVolumeTpmPinStartupKeyRequired` `osVolumeUnprotected` `recoveryKeyBackupFailed` `fixedDriveNotEncrypted` `fixedDriveEncryptionMethodMismatch` `loggedOnUserNonAdmin` , `windowsRecoveryEnvironmentNotConfigured` , `tpmNotAvailable` , `tpmNotReady` , `networkError` .</span><span class="sxs-lookup"><span data-stu-id="c7c60-167">Possible values are: `success`, `noUserConsent`, `osVolumeEncryptionMethodMismatch`, `osVolumeTpmRequired`, `osVolumeTpmOnlyRequired`, `osVolumeTpmPinRequired`, `osVolumeTpmStartupKeyRequired`, `osVolumeTpmPinStartupKeyRequired`, `osVolumeUnprotected`, `recoveryKeyBackupFailed`, `fixedDriveNotEncrypted`, `fixedDriveEncryptionMethodMismatch`, `loggedOnUserNonAdmin`, `windowsRecoveryEnvironmentNotConfigured`, `tpmNotAvailable`, `tpmNotReady`, `networkError`.</span></span>|
|<span data-ttu-id="c7c60-168">fileVaultStates</span><span class="sxs-lookup"><span data-stu-id="c7c60-168">fileVaultStates</span></span>|[<span data-ttu-id="c7c60-169">fileVaultState</span><span class="sxs-lookup"><span data-stu-id="c7c60-169">fileVaultState</span></span>](../resources/intune-deviceconfig-filevaultstate.md)|<span data-ttu-id="c7c60-170">Estado FileVault.</span><span class="sxs-lookup"><span data-stu-id="c7c60-170">FileVault State.</span></span> <span data-ttu-id="c7c60-171">Os valores possíveis são: `success`, `driveEncryptedByUser`, `userDeferredEncryption`, `escrowNotEnabled`.</span><span class="sxs-lookup"><span data-stu-id="c7c60-171">Possible values are: `success`, `driveEncryptedByUser`, `userDeferredEncryption`, `escrowNotEnabled`.</span></span>|
|<span data-ttu-id="c7c60-172">policyDetails</span><span class="sxs-lookup"><span data-stu-id="c7c60-172">policyDetails</span></span>|<span data-ttu-id="c7c60-173">coleção [encryptionReportPolicyDetails](../resources/intune-deviceconfig-encryptionreportpolicydetails.md)</span><span class="sxs-lookup"><span data-stu-id="c7c60-173">[encryptionReportPolicyDetails](../resources/intune-deviceconfig-encryptionreportpolicydetails.md) collection</span></span>|<span data-ttu-id="c7c60-174">Detalhes da política</span><span class="sxs-lookup"><span data-stu-id="c7c60-174">Policy Details</span></span>|



## <a name="response"></a><span data-ttu-id="c7c60-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="c7c60-175">Response</span></span>
<span data-ttu-id="c7c60-176">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c7c60-176">If successful, this method returns a `201 Created` response code and a [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c7c60-177">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c7c60-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="c7c60-178">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c7c60-178">Request</span></span>
<span data-ttu-id="c7c60-179">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c7c60-179">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c7c60-180">Resposta</span><span class="sxs-lookup"><span data-stu-id="c7c60-180">Response</span></span>
<span data-ttu-id="c7c60-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c7c60-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






