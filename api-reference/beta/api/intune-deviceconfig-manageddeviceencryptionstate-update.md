---
title: Atualizar managedDeviceEncryptionState
description: Atualize as propriedades de um objeto managedDeviceEncryptionState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8dd4c44cf373b5aa5ac20208308394ede5fe2d05
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51155131"
---
# <a name="update-manageddeviceencryptionstate"></a><span data-ttu-id="2142d-103">Atualizar managedDeviceEncryptionState</span><span class="sxs-lookup"><span data-stu-id="2142d-103">Update managedDeviceEncryptionState</span></span>

<span data-ttu-id="2142d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2142d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2142d-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2142d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2142d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2142d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2142d-107">Atualize as propriedades de [um objeto managedDeviceEncryptionState.](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)</span><span class="sxs-lookup"><span data-stu-id="2142d-107">Update the properties of a [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2142d-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2142d-108">Prerequisites</span></span>
<span data-ttu-id="2142d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2142d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2142d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2142d-111">Permission type</span></span>|<span data-ttu-id="2142d-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2142d-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2142d-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2142d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2142d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2142d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2142d-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2142d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2142d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2142d-116">Not supported.</span></span>|
|<span data-ttu-id="2142d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2142d-117">Application</span></span>|<span data-ttu-id="2142d-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2142d-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2142d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2142d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managedDeviceEncryptionStates/{managedDeviceEncryptionStateId}
```

## <a name="request-headers"></a><span data-ttu-id="2142d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2142d-120">Request headers</span></span>
|<span data-ttu-id="2142d-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2142d-121">Header</span></span>|<span data-ttu-id="2142d-122">Valor</span><span class="sxs-lookup"><span data-stu-id="2142d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2142d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="2142d-123">Authorization</span></span>|<span data-ttu-id="2142d-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2142d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2142d-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2142d-125">Accept</span></span>|<span data-ttu-id="2142d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2142d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2142d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2142d-127">Request body</span></span>
<span data-ttu-id="2142d-128">No corpo da solicitação, fornece uma representação JSON para o [objeto managedDeviceEncryptionState.](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)</span><span class="sxs-lookup"><span data-stu-id="2142d-128">In the request body, supply a JSON representation for the [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) object.</span></span>

<span data-ttu-id="2142d-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md).</span><span class="sxs-lookup"><span data-stu-id="2142d-129">The following table shows the properties that are required when you create the [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md).</span></span>

|<span data-ttu-id="2142d-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2142d-130">Property</span></span>|<span data-ttu-id="2142d-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="2142d-131">Type</span></span>|<span data-ttu-id="2142d-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="2142d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2142d-133">id</span><span class="sxs-lookup"><span data-stu-id="2142d-133">id</span></span>|<span data-ttu-id="2142d-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2142d-134">String</span></span>|<span data-ttu-id="2142d-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="2142d-135">Key of the entity.</span></span>|
|<span data-ttu-id="2142d-136">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="2142d-136">userPrincipalName</span></span>|<span data-ttu-id="2142d-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2142d-137">String</span></span>|<span data-ttu-id="2142d-138">Nome de usuário</span><span class="sxs-lookup"><span data-stu-id="2142d-138">User name</span></span>|
|<span data-ttu-id="2142d-139">deviceType</span><span class="sxs-lookup"><span data-stu-id="2142d-139">deviceType</span></span>|[<span data-ttu-id="2142d-140">deviceTypes</span><span class="sxs-lookup"><span data-stu-id="2142d-140">deviceTypes</span></span>](../resources/intune-deviceconfig-devicetypes.md)|<span data-ttu-id="2142d-141">Plataforma do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2142d-141">Platform of the device.</span></span> <span data-ttu-id="2142d-142">Os valores possíveis são: `desktop` , , , , , , , , `windowsRT` `winMO6` , , , `nokia` `windowsPhone` `mac` , `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer` `unix` `macMDM` `holoLens` `surfaceHub` , `androidForWork` `androidEnterprise` `blackberry` `palm` `unknown` , .</span><span class="sxs-lookup"><span data-stu-id="2142d-142">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="2142d-143">osVersion</span><span class="sxs-lookup"><span data-stu-id="2142d-143">osVersion</span></span>|<span data-ttu-id="2142d-144">String</span><span class="sxs-lookup"><span data-stu-id="2142d-144">String</span></span>|<span data-ttu-id="2142d-145">Versão do sistema operacional do dispositivo</span><span class="sxs-lookup"><span data-stu-id="2142d-145">Operating system version of the device</span></span>|
|<span data-ttu-id="2142d-146">tpmSpecificationVersion</span><span class="sxs-lookup"><span data-stu-id="2142d-146">tpmSpecificationVersion</span></span>|<span data-ttu-id="2142d-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2142d-147">String</span></span>|<span data-ttu-id="2142d-148">Versão TPM do dispositivo</span><span class="sxs-lookup"><span data-stu-id="2142d-148">Device TPM Version</span></span>|
|<span data-ttu-id="2142d-149">deviceName</span><span class="sxs-lookup"><span data-stu-id="2142d-149">deviceName</span></span>|<span data-ttu-id="2142d-150">String</span><span class="sxs-lookup"><span data-stu-id="2142d-150">String</span></span>|<span data-ttu-id="2142d-151">Nome do dispositivo</span><span class="sxs-lookup"><span data-stu-id="2142d-151">Device name</span></span>|
|<span data-ttu-id="2142d-152">encryptionReadinessState</span><span class="sxs-lookup"><span data-stu-id="2142d-152">encryptionReadinessState</span></span>|[<span data-ttu-id="2142d-153">encryptionReadinessState</span><span class="sxs-lookup"><span data-stu-id="2142d-153">encryptionReadinessState</span></span>](../resources/intune-deviceconfig-encryptionreadinessstate.md)|<span data-ttu-id="2142d-154">Estado de preparação da criptografia.</span><span class="sxs-lookup"><span data-stu-id="2142d-154">Encryption readiness state.</span></span> <span data-ttu-id="2142d-155">Os valores possíveis são: `notReady` e `ready`.</span><span class="sxs-lookup"><span data-stu-id="2142d-155">Possible values are: `notReady`, `ready`.</span></span>|
|<span data-ttu-id="2142d-156">encryptionState</span><span class="sxs-lookup"><span data-stu-id="2142d-156">encryptionState</span></span>|[<span data-ttu-id="2142d-157">encryptionState</span><span class="sxs-lookup"><span data-stu-id="2142d-157">encryptionState</span></span>](../resources/intune-deviceconfig-encryptionstate.md)|<span data-ttu-id="2142d-158">Estado de criptografia de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2142d-158">Device encryption state.</span></span> <span data-ttu-id="2142d-159">Os valores possíveis são: `notEncrypted` e `encrypted`.</span><span class="sxs-lookup"><span data-stu-id="2142d-159">Possible values are: `notEncrypted`, `encrypted`.</span></span>|
|<span data-ttu-id="2142d-160">encryptionPolicySettingState</span><span class="sxs-lookup"><span data-stu-id="2142d-160">encryptionPolicySettingState</span></span>|[<span data-ttu-id="2142d-161">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="2142d-161">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="2142d-162">Estado de configuração da política de criptografia.</span><span class="sxs-lookup"><span data-stu-id="2142d-162">Encryption policy setting state.</span></span> <span data-ttu-id="2142d-163">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="2142d-163">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="2142d-164">advancedBitLockerStates</span><span class="sxs-lookup"><span data-stu-id="2142d-164">advancedBitLockerStates</span></span>|[<span data-ttu-id="2142d-165">advancedBitLockerState</span><span class="sxs-lookup"><span data-stu-id="2142d-165">advancedBitLockerState</span></span>](../resources/intune-deviceconfig-advancedbitlockerstate.md)|<span data-ttu-id="2142d-166">Estado avançado do BitLocker.</span><span class="sxs-lookup"><span data-stu-id="2142d-166">Advanced BitLocker State.</span></span> <span data-ttu-id="2142d-167">Os valores possíveis são: `success` , , , , , , , , `noUserConsent` , , , `osVolumeUnprotected` , , `osVolumeTpmRequired` , , , `osVolumeTpmOnlyRequired` `osVolumeTpmPinRequired` `osVolumeTpmStartupKeyRequired` , `osVolumeTpmPinStartupKeyRequired` `osVolumeEncryptionMethodMismatch` `recoveryKeyBackupFailed` `fixedDriveNotEncrypted` `fixedDriveEncryptionMethodMismatch` `loggedOnUserNonAdmin` `windowsRecoveryEnvironmentNotConfigured` `tpmNotAvailable` `tpmNotReady` `networkError` .</span><span class="sxs-lookup"><span data-stu-id="2142d-167">Possible values are: `success`, `noUserConsent`, `osVolumeUnprotected`, `osVolumeTpmRequired`, `osVolumeTpmOnlyRequired`, `osVolumeTpmPinRequired`, `osVolumeTpmStartupKeyRequired`, `osVolumeTpmPinStartupKeyRequired`, `osVolumeEncryptionMethodMismatch`, `recoveryKeyBackupFailed`, `fixedDriveNotEncrypted`, `fixedDriveEncryptionMethodMismatch`, `loggedOnUserNonAdmin`, `windowsRecoveryEnvironmentNotConfigured`, `tpmNotAvailable`, `tpmNotReady`, `networkError`.</span></span>|
|<span data-ttu-id="2142d-168">fileVaultStates</span><span class="sxs-lookup"><span data-stu-id="2142d-168">fileVaultStates</span></span>|[<span data-ttu-id="2142d-169">fileVaultState</span><span class="sxs-lookup"><span data-stu-id="2142d-169">fileVaultState</span></span>](../resources/intune-deviceconfig-filevaultstate.md)|<span data-ttu-id="2142d-170">Estado FileVault.</span><span class="sxs-lookup"><span data-stu-id="2142d-170">FileVault State.</span></span> <span data-ttu-id="2142d-171">Os valores possíveis são: `success`, `driveEncryptedByUser`, `userDeferredEncryption`, `escrowNotEnabled`.</span><span class="sxs-lookup"><span data-stu-id="2142d-171">Possible values are: `success`, `driveEncryptedByUser`, `userDeferredEncryption`, `escrowNotEnabled`.</span></span>|
|<span data-ttu-id="2142d-172">policyDetails</span><span class="sxs-lookup"><span data-stu-id="2142d-172">policyDetails</span></span>|<span data-ttu-id="2142d-173">[Coleção encryptionReportPolicyDetails](../resources/intune-deviceconfig-encryptionreportpolicydetails.md)</span><span class="sxs-lookup"><span data-stu-id="2142d-173">[encryptionReportPolicyDetails](../resources/intune-deviceconfig-encryptionreportpolicydetails.md) collection</span></span>|<span data-ttu-id="2142d-174">Detalhes da política</span><span class="sxs-lookup"><span data-stu-id="2142d-174">Policy Details</span></span>|



## <a name="response"></a><span data-ttu-id="2142d-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="2142d-175">Response</span></span>
<span data-ttu-id="2142d-176">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2142d-176">If successful, this method returns a `200 OK` response code and an updated [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2142d-177">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2142d-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="2142d-178">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2142d-178">Request</span></span>
<span data-ttu-id="2142d-179">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2142d-179">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managedDeviceEncryptionStates/{managedDeviceEncryptionStateId}
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

### <a name="response"></a><span data-ttu-id="2142d-180">Resposta</span><span class="sxs-lookup"><span data-stu-id="2142d-180">Response</span></span>
<span data-ttu-id="2142d-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2142d-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




