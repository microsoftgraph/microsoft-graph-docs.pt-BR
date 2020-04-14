---
title: Atualizar managedDeviceEncryptionState
description: Atualiza as propriedades de um objeto managedDeviceEncryptionState.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: de8657e8996f3b0e82712c5be56d12bd36430a68
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43431867"
---
# <a name="update-manageddeviceencryptionstate"></a><span data-ttu-id="5e1ec-103">Atualizar managedDeviceEncryptionState</span><span class="sxs-lookup"><span data-stu-id="5e1ec-103">Update managedDeviceEncryptionState</span></span>

<span data-ttu-id="5e1ec-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5e1ec-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5e1ec-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5e1ec-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5e1ec-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5e1ec-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5e1ec-107">Atualiza as propriedades de um objeto [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) .</span><span class="sxs-lookup"><span data-stu-id="5e1ec-107">Update the properties of a [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5e1ec-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5e1ec-108">Prerequisites</span></span>
<span data-ttu-id="5e1ec-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5e1ec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5e1ec-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5e1ec-111">Permission type</span></span>|<span data-ttu-id="5e1ec-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5e1ec-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5e1ec-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5e1ec-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5e1ec-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5e1ec-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5e1ec-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5e1ec-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5e1ec-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5e1ec-116">Not supported.</span></span>|
|<span data-ttu-id="5e1ec-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5e1ec-117">Application</span></span>|<span data-ttu-id="5e1ec-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5e1ec-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5e1ec-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5e1ec-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managedDeviceEncryptionStates/{managedDeviceEncryptionStateId}
```

## <a name="request-headers"></a><span data-ttu-id="5e1ec-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5e1ec-120">Request headers</span></span>
|<span data-ttu-id="5e1ec-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5e1ec-121">Header</span></span>|<span data-ttu-id="5e1ec-122">Valor</span><span class="sxs-lookup"><span data-stu-id="5e1ec-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5e1ec-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="5e1ec-123">Authorization</span></span>|<span data-ttu-id="5e1ec-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5e1ec-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5e1ec-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5e1ec-125">Accept</span></span>|<span data-ttu-id="5e1ec-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5e1ec-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5e1ec-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5e1ec-127">Request body</span></span>
<span data-ttu-id="5e1ec-128">No corpo da solicitação, forneça uma representação JSON do objeto [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) .</span><span class="sxs-lookup"><span data-stu-id="5e1ec-128">In the request body, supply a JSON representation for the [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) object.</span></span>

<span data-ttu-id="5e1ec-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md).</span><span class="sxs-lookup"><span data-stu-id="5e1ec-129">The following table shows the properties that are required when you create the [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md).</span></span>

|<span data-ttu-id="5e1ec-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5e1ec-130">Property</span></span>|<span data-ttu-id="5e1ec-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="5e1ec-131">Type</span></span>|<span data-ttu-id="5e1ec-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="5e1ec-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5e1ec-133">id</span><span class="sxs-lookup"><span data-stu-id="5e1ec-133">id</span></span>|<span data-ttu-id="5e1ec-134">String</span><span class="sxs-lookup"><span data-stu-id="5e1ec-134">String</span></span>|<span data-ttu-id="5e1ec-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="5e1ec-135">Key of the entity.</span></span>|
|<span data-ttu-id="5e1ec-136">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="5e1ec-136">userPrincipalName</span></span>|<span data-ttu-id="5e1ec-137">String</span><span class="sxs-lookup"><span data-stu-id="5e1ec-137">String</span></span>|<span data-ttu-id="5e1ec-138">Nome de usuário</span><span class="sxs-lookup"><span data-stu-id="5e1ec-138">User name</span></span>|
|<span data-ttu-id="5e1ec-139">deviceType</span><span class="sxs-lookup"><span data-stu-id="5e1ec-139">deviceType</span></span>|[<span data-ttu-id="5e1ec-140">deviceTypes</span><span class="sxs-lookup"><span data-stu-id="5e1ec-140">deviceTypes</span></span>](../resources/intune-deviceconfig-devicetypes.md)|<span data-ttu-id="5e1ec-141">Plataforma do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5e1ec-141">Platform of the device.</span></span> <span data-ttu-id="5e1ec-142">Os valores possíveis são `desktop`: `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad` `iPod` `android`,,, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`,,,,,,,,,,.</span><span class="sxs-lookup"><span data-stu-id="5e1ec-142">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="5e1ec-143">osVersion</span><span class="sxs-lookup"><span data-stu-id="5e1ec-143">osVersion</span></span>|<span data-ttu-id="5e1ec-144">String</span><span class="sxs-lookup"><span data-stu-id="5e1ec-144">String</span></span>|<span data-ttu-id="5e1ec-145">Versão do sistema operacional do dispositivo</span><span class="sxs-lookup"><span data-stu-id="5e1ec-145">Operating system version of the device</span></span>|
|<span data-ttu-id="5e1ec-146">tpmSpecificationVersion</span><span class="sxs-lookup"><span data-stu-id="5e1ec-146">tpmSpecificationVersion</span></span>|<span data-ttu-id="5e1ec-147">String</span><span class="sxs-lookup"><span data-stu-id="5e1ec-147">String</span></span>|<span data-ttu-id="5e1ec-148">Versão do TPM do dispositivo</span><span class="sxs-lookup"><span data-stu-id="5e1ec-148">Device TPM Version</span></span>|
|<span data-ttu-id="5e1ec-149">deviceName</span><span class="sxs-lookup"><span data-stu-id="5e1ec-149">deviceName</span></span>|<span data-ttu-id="5e1ec-150">String</span><span class="sxs-lookup"><span data-stu-id="5e1ec-150">String</span></span>|<span data-ttu-id="5e1ec-151">Nome do dispositivo</span><span class="sxs-lookup"><span data-stu-id="5e1ec-151">Device name</span></span>|
|<span data-ttu-id="5e1ec-152">encryptionReadinessState</span><span class="sxs-lookup"><span data-stu-id="5e1ec-152">encryptionReadinessState</span></span>|[<span data-ttu-id="5e1ec-153">encryptionReadinessState</span><span class="sxs-lookup"><span data-stu-id="5e1ec-153">encryptionReadinessState</span></span>](../resources/intune-deviceconfig-encryptionreadinessstate.md)|<span data-ttu-id="5e1ec-154">Estado de preparação de criptografia.</span><span class="sxs-lookup"><span data-stu-id="5e1ec-154">Encryption readiness state.</span></span> <span data-ttu-id="5e1ec-155">Os valores possíveis são: `notReady` e `ready`.</span><span class="sxs-lookup"><span data-stu-id="5e1ec-155">Possible values are: `notReady`, `ready`.</span></span>|
|<span data-ttu-id="5e1ec-156">encryptionState</span><span class="sxs-lookup"><span data-stu-id="5e1ec-156">encryptionState</span></span>|[<span data-ttu-id="5e1ec-157">encryptionState</span><span class="sxs-lookup"><span data-stu-id="5e1ec-157">encryptionState</span></span>](../resources/intune-deviceconfig-encryptionstate.md)|<span data-ttu-id="5e1ec-158">Estado de criptografia do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5e1ec-158">Device encryption state.</span></span> <span data-ttu-id="5e1ec-159">Os valores possíveis são: `notEncrypted` e `encrypted`.</span><span class="sxs-lookup"><span data-stu-id="5e1ec-159">Possible values are: `notEncrypted`, `encrypted`.</span></span>|
|<span data-ttu-id="5e1ec-160">encryptionPolicySettingState</span><span class="sxs-lookup"><span data-stu-id="5e1ec-160">encryptionPolicySettingState</span></span>|[<span data-ttu-id="5e1ec-161">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="5e1ec-161">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="5e1ec-162">Estado da configuração da política de criptografia.</span><span class="sxs-lookup"><span data-stu-id="5e1ec-162">Encryption policy setting state.</span></span> <span data-ttu-id="5e1ec-163">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="5e1ec-163">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="5e1ec-164">advancedBitLockerStates</span><span class="sxs-lookup"><span data-stu-id="5e1ec-164">advancedBitLockerStates</span></span>|[<span data-ttu-id="5e1ec-165">advancedBitLockerState</span><span class="sxs-lookup"><span data-stu-id="5e1ec-165">advancedBitLockerState</span></span>](../resources/intune-deviceconfig-advancedbitlockerstate.md)|<span data-ttu-id="5e1ec-166">Estado do BitLocker avançado.</span><span class="sxs-lookup"><span data-stu-id="5e1ec-166">Advanced BitLocker State.</span></span> <span data-ttu-id="5e1ec-167">Os valores possíveis são `success`: `noUserConsent`, `osVolumeEncryptionMethodMismatch`, `osVolumeTpmRequired`, `osVolumeTpmOnlyRequired`, `osVolumeTpmPinRequired`, `osVolumeTpmStartupKeyRequired`, `osVolumeTpmPinStartupKeyRequired`, `osVolumeUnprotected`, `recoveryKeyBackupFailed`, `fixedDriveNotEncrypted`, `fixedDriveEncryptionMethodMismatch`, `loggedOnUserNonAdmin`, `windowsRecoveryEnvironmentNotConfigured`, `tpmNotAvailable`, `tpmNotReady`, `networkError`,,,,,,,,,.</span><span class="sxs-lookup"><span data-stu-id="5e1ec-167">Possible values are: `success`, `noUserConsent`, `osVolumeEncryptionMethodMismatch`, `osVolumeTpmRequired`, `osVolumeTpmOnlyRequired`, `osVolumeTpmPinRequired`, `osVolumeTpmStartupKeyRequired`, `osVolumeTpmPinStartupKeyRequired`, `osVolumeUnprotected`, `recoveryKeyBackupFailed`, `fixedDriveNotEncrypted`, `fixedDriveEncryptionMethodMismatch`, `loggedOnUserNonAdmin`, `windowsRecoveryEnvironmentNotConfigured`, `tpmNotAvailable`, `tpmNotReady`, `networkError`.</span></span>|
|<span data-ttu-id="5e1ec-168">fileVaultStates</span><span class="sxs-lookup"><span data-stu-id="5e1ec-168">fileVaultStates</span></span>|[<span data-ttu-id="5e1ec-169">fileVaultState</span><span class="sxs-lookup"><span data-stu-id="5e1ec-169">fileVaultState</span></span>](../resources/intune-deviceconfig-filevaultstate.md)|<span data-ttu-id="5e1ec-170">Estado FileVault.</span><span class="sxs-lookup"><span data-stu-id="5e1ec-170">FileVault State.</span></span> <span data-ttu-id="5e1ec-171">Os valores possíveis são: `success`, `driveEncryptedByUser`, `userDeferredEncryption`, `escrowNotEnabled`.</span><span class="sxs-lookup"><span data-stu-id="5e1ec-171">Possible values are: `success`, `driveEncryptedByUser`, `userDeferredEncryption`, `escrowNotEnabled`.</span></span>|
|<span data-ttu-id="5e1ec-172">policyDetails</span><span class="sxs-lookup"><span data-stu-id="5e1ec-172">policyDetails</span></span>|<span data-ttu-id="5e1ec-173">coleção [encryptionReportPolicyDetails](../resources/intune-deviceconfig-encryptionreportpolicydetails.md)</span><span class="sxs-lookup"><span data-stu-id="5e1ec-173">[encryptionReportPolicyDetails](../resources/intune-deviceconfig-encryptionreportpolicydetails.md) collection</span></span>|<span data-ttu-id="5e1ec-174">Detalhes da política</span><span class="sxs-lookup"><span data-stu-id="5e1ec-174">Policy Details</span></span>|



## <a name="response"></a><span data-ttu-id="5e1ec-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="5e1ec-175">Response</span></span>
<span data-ttu-id="5e1ec-176">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5e1ec-176">If successful, this method returns a `200 OK` response code and an updated [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5e1ec-177">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5e1ec-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="5e1ec-178">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5e1ec-178">Request</span></span>
<span data-ttu-id="5e1ec-179">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5e1ec-179">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5e1ec-180">Resposta</span><span class="sxs-lookup"><span data-stu-id="5e1ec-180">Response</span></span>
<span data-ttu-id="5e1ec-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5e1ec-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



