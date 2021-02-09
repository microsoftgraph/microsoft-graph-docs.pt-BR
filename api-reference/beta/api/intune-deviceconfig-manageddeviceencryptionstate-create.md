---
title: Criar managedDeviceEncryptionState
description: Criar um novo objeto managedDeviceEncryptionState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9aeb439c6cd456a992e5485772c2ebd19357c045
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50154575"
---
# <a name="create-manageddeviceencryptionstate"></a><span data-ttu-id="cbdea-103">Criar managedDeviceEncryptionState</span><span class="sxs-lookup"><span data-stu-id="cbdea-103">Create managedDeviceEncryptionState</span></span>

<span data-ttu-id="cbdea-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cbdea-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cbdea-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="cbdea-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cbdea-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cbdea-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cbdea-107">Criar um novo [objeto managedDeviceEncryptionState.](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)</span><span class="sxs-lookup"><span data-stu-id="cbdea-107">Create a new [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cbdea-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="cbdea-108">Prerequisites</span></span>
<span data-ttu-id="cbdea-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cbdea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cbdea-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cbdea-111">Permission type</span></span>|<span data-ttu-id="cbdea-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="cbdea-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cbdea-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cbdea-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cbdea-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cbdea-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="cbdea-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cbdea-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cbdea-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cbdea-116">Not supported.</span></span>|
|<span data-ttu-id="cbdea-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cbdea-117">Application</span></span>|<span data-ttu-id="cbdea-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cbdea-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cbdea-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cbdea-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDeviceEncryptionStates
```

## <a name="request-headers"></a><span data-ttu-id="cbdea-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cbdea-120">Request headers</span></span>
|<span data-ttu-id="cbdea-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cbdea-121">Header</span></span>|<span data-ttu-id="cbdea-122">Valor</span><span class="sxs-lookup"><span data-stu-id="cbdea-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cbdea-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="cbdea-123">Authorization</span></span>|<span data-ttu-id="cbdea-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cbdea-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cbdea-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="cbdea-125">Accept</span></span>|<span data-ttu-id="cbdea-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cbdea-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cbdea-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cbdea-127">Request body</span></span>
<span data-ttu-id="cbdea-128">No corpo da solicitação, fornece uma representação JSON do objeto managedDeviceEncryptionState.</span><span class="sxs-lookup"><span data-stu-id="cbdea-128">In the request body, supply a JSON representation for the managedDeviceEncryptionState object.</span></span>

<span data-ttu-id="cbdea-129">A tabela a seguir mostra as propriedades que são necessárias ao criar managedDeviceEncryptionState.</span><span class="sxs-lookup"><span data-stu-id="cbdea-129">The following table shows the properties that are required when you create the managedDeviceEncryptionState.</span></span>

|<span data-ttu-id="cbdea-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cbdea-130">Property</span></span>|<span data-ttu-id="cbdea-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="cbdea-131">Type</span></span>|<span data-ttu-id="cbdea-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="cbdea-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cbdea-133">id</span><span class="sxs-lookup"><span data-stu-id="cbdea-133">id</span></span>|<span data-ttu-id="cbdea-134">String</span><span class="sxs-lookup"><span data-stu-id="cbdea-134">String</span></span>|<span data-ttu-id="cbdea-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="cbdea-135">Key of the entity.</span></span>|
|<span data-ttu-id="cbdea-136">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="cbdea-136">userPrincipalName</span></span>|<span data-ttu-id="cbdea-137">String</span><span class="sxs-lookup"><span data-stu-id="cbdea-137">String</span></span>|<span data-ttu-id="cbdea-138">Nome de usuário</span><span class="sxs-lookup"><span data-stu-id="cbdea-138">User name</span></span>|
|<span data-ttu-id="cbdea-139">deviceType</span><span class="sxs-lookup"><span data-stu-id="cbdea-139">deviceType</span></span>|[<span data-ttu-id="cbdea-140">deviceTypes</span><span class="sxs-lookup"><span data-stu-id="cbdea-140">deviceTypes</span></span>](../resources/intune-deviceconfig-devicetypes.md)|<span data-ttu-id="cbdea-141">Plataforma do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="cbdea-141">Platform of the device.</span></span> <span data-ttu-id="cbdea-142">Os valores possíveis `desktop` são: `windowsRT` , , , , , , , , `winMO6` , , `nokia` , , `windowsPhone` , , , , `mac` , , `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android` , `iSocConsumer` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `blackberry` `palm` `unknown` .</span><span class="sxs-lookup"><span data-stu-id="cbdea-142">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="cbdea-143">osVersion</span><span class="sxs-lookup"><span data-stu-id="cbdea-143">osVersion</span></span>|<span data-ttu-id="cbdea-144">String</span><span class="sxs-lookup"><span data-stu-id="cbdea-144">String</span></span>|<span data-ttu-id="cbdea-145">Versão do sistema operacional do dispositivo</span><span class="sxs-lookup"><span data-stu-id="cbdea-145">Operating system version of the device</span></span>|
|<span data-ttu-id="cbdea-146">tpmSpecificationVersion</span><span class="sxs-lookup"><span data-stu-id="cbdea-146">tpmSpecificationVersion</span></span>|<span data-ttu-id="cbdea-147">String</span><span class="sxs-lookup"><span data-stu-id="cbdea-147">String</span></span>|<span data-ttu-id="cbdea-148">Versão TPM do dispositivo</span><span class="sxs-lookup"><span data-stu-id="cbdea-148">Device TPM Version</span></span>|
|<span data-ttu-id="cbdea-149">deviceName</span><span class="sxs-lookup"><span data-stu-id="cbdea-149">deviceName</span></span>|<span data-ttu-id="cbdea-150">String</span><span class="sxs-lookup"><span data-stu-id="cbdea-150">String</span></span>|<span data-ttu-id="cbdea-151">Nome do dispositivo</span><span class="sxs-lookup"><span data-stu-id="cbdea-151">Device name</span></span>|
|<span data-ttu-id="cbdea-152">encryptionReadinessState</span><span class="sxs-lookup"><span data-stu-id="cbdea-152">encryptionReadinessState</span></span>|[<span data-ttu-id="cbdea-153">encryptionReadinessState</span><span class="sxs-lookup"><span data-stu-id="cbdea-153">encryptionReadinessState</span></span>](../resources/intune-deviceconfig-encryptionreadinessstate.md)|<span data-ttu-id="cbdea-154">Estado de preparação de criptografia.</span><span class="sxs-lookup"><span data-stu-id="cbdea-154">Encryption readiness state.</span></span> <span data-ttu-id="cbdea-155">Os valores possíveis são: `notReady` e `ready`.</span><span class="sxs-lookup"><span data-stu-id="cbdea-155">Possible values are: `notReady`, `ready`.</span></span>|
|<span data-ttu-id="cbdea-156">encryptionState</span><span class="sxs-lookup"><span data-stu-id="cbdea-156">encryptionState</span></span>|[<span data-ttu-id="cbdea-157">encryptionState</span><span class="sxs-lookup"><span data-stu-id="cbdea-157">encryptionState</span></span>](../resources/intune-deviceconfig-encryptionstate.md)|<span data-ttu-id="cbdea-158">Estado de criptografia do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="cbdea-158">Device encryption state.</span></span> <span data-ttu-id="cbdea-159">Os valores possíveis são: `notEncrypted` e `encrypted`.</span><span class="sxs-lookup"><span data-stu-id="cbdea-159">Possible values are: `notEncrypted`, `encrypted`.</span></span>|
|<span data-ttu-id="cbdea-160">encryptionPolicySettingState</span><span class="sxs-lookup"><span data-stu-id="cbdea-160">encryptionPolicySettingState</span></span>|[<span data-ttu-id="cbdea-161">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="cbdea-161">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="cbdea-162">Estado de configuração da política de criptografia.</span><span class="sxs-lookup"><span data-stu-id="cbdea-162">Encryption policy setting state.</span></span> <span data-ttu-id="cbdea-163">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="cbdea-163">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="cbdea-164">advancedBitLockerStates</span><span class="sxs-lookup"><span data-stu-id="cbdea-164">advancedBitLockerStates</span></span>|[<span data-ttu-id="cbdea-165">advancedBitLockerState</span><span class="sxs-lookup"><span data-stu-id="cbdea-165">advancedBitLockerState</span></span>](../resources/intune-deviceconfig-advancedbitlockerstate.md)|<span data-ttu-id="cbdea-166">Estado avançado do BitLocker.</span><span class="sxs-lookup"><span data-stu-id="cbdea-166">Advanced BitLocker State.</span></span> <span data-ttu-id="cbdea-167">Os valores possíveis `success` são: `noUserConsent` , , , , , , , , `osVolumeUnprotected` , , `osVolumeTpmRequired` , , , `osVolumeTpmOnlyRequired` , `osVolumeTpmPinRequired` `osVolumeTpmStartupKeyRequired` , `osVolumeTpmPinStartupKeyRequired` `osVolumeEncryptionMethodMismatch` `recoveryKeyBackupFailed` `fixedDriveNotEncrypted` `fixedDriveEncryptionMethodMismatch` `loggedOnUserNonAdmin` `windowsRecoveryEnvironmentNotConfigured` `tpmNotAvailable` `tpmNotReady` `networkError` .</span><span class="sxs-lookup"><span data-stu-id="cbdea-167">Possible values are: `success`, `noUserConsent`, `osVolumeUnprotected`, `osVolumeTpmRequired`, `osVolumeTpmOnlyRequired`, `osVolumeTpmPinRequired`, `osVolumeTpmStartupKeyRequired`, `osVolumeTpmPinStartupKeyRequired`, `osVolumeEncryptionMethodMismatch`, `recoveryKeyBackupFailed`, `fixedDriveNotEncrypted`, `fixedDriveEncryptionMethodMismatch`, `loggedOnUserNonAdmin`, `windowsRecoveryEnvironmentNotConfigured`, `tpmNotAvailable`, `tpmNotReady`, `networkError`.</span></span>|
|<span data-ttu-id="cbdea-168">fileVaultStates</span><span class="sxs-lookup"><span data-stu-id="cbdea-168">fileVaultStates</span></span>|[<span data-ttu-id="cbdea-169">fileVaultState</span><span class="sxs-lookup"><span data-stu-id="cbdea-169">fileVaultState</span></span>](../resources/intune-deviceconfig-filevaultstate.md)|<span data-ttu-id="cbdea-170">Estado FileVault.</span><span class="sxs-lookup"><span data-stu-id="cbdea-170">FileVault State.</span></span> <span data-ttu-id="cbdea-171">Os valores possíveis são: `success`, `driveEncryptedByUser`, `userDeferredEncryption`, `escrowNotEnabled`.</span><span class="sxs-lookup"><span data-stu-id="cbdea-171">Possible values are: `success`, `driveEncryptedByUser`, `userDeferredEncryption`, `escrowNotEnabled`.</span></span>|
|<span data-ttu-id="cbdea-172">policyDetails</span><span class="sxs-lookup"><span data-stu-id="cbdea-172">policyDetails</span></span>|<span data-ttu-id="cbdea-173">[Coleção encryptionReportPolicyDetails](../resources/intune-deviceconfig-encryptionreportpolicydetails.md)</span><span class="sxs-lookup"><span data-stu-id="cbdea-173">[encryptionReportPolicyDetails](../resources/intune-deviceconfig-encryptionreportpolicydetails.md) collection</span></span>|<span data-ttu-id="cbdea-174">Detalhes da Política</span><span class="sxs-lookup"><span data-stu-id="cbdea-174">Policy Details</span></span>|



## <a name="response"></a><span data-ttu-id="cbdea-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="cbdea-175">Response</span></span>
<span data-ttu-id="cbdea-176">Se bem-sucedido, este método retorna um código de resposta e um objeto `201 Created` [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cbdea-176">If successful, this method returns a `201 Created` response code and a [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cbdea-177">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cbdea-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="cbdea-178">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cbdea-178">Request</span></span>
<span data-ttu-id="cbdea-179">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cbdea-179">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="cbdea-180">Resposta</span><span class="sxs-lookup"><span data-stu-id="cbdea-180">Response</span></span>
<span data-ttu-id="cbdea-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cbdea-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




