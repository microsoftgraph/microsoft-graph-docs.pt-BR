---
title: Atualizar managedDeviceEncryptionState
description: Atualiza as propriedades de um objeto managedDeviceEncryptionState.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 994cf3a4e0760e9f760856f50ee954eea010f524
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31797071"
---
# <a name="update-manageddeviceencryptionstate"></a><span data-ttu-id="daf61-103">Atualizar managedDeviceEncryptionState</span><span class="sxs-lookup"><span data-stu-id="daf61-103">Update managedDeviceEncryptionState</span></span>

> <span data-ttu-id="daf61-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="daf61-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="daf61-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="daf61-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="daf61-106">Atualiza as propriedades de um objeto [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) .</span><span class="sxs-lookup"><span data-stu-id="daf61-106">Update the properties of a [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="daf61-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="daf61-107">Prerequisites</span></span>
<span data-ttu-id="daf61-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="daf61-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="daf61-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="daf61-110">Permission type</span></span>|<span data-ttu-id="daf61-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="daf61-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="daf61-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="daf61-112">Delegated (work or school account)</span></span>|<span data-ttu-id="daf61-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="daf61-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="daf61-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="daf61-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="daf61-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="daf61-115">Not supported.</span></span>|
|<span data-ttu-id="daf61-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="daf61-116">Application</span></span>|<span data-ttu-id="daf61-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="daf61-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="daf61-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="daf61-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managedDeviceEncryptionStates/{managedDeviceEncryptionStateId}
```

## <a name="request-headers"></a><span data-ttu-id="daf61-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="daf61-119">Request headers</span></span>
|<span data-ttu-id="daf61-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="daf61-120">Header</span></span>|<span data-ttu-id="daf61-121">Valor</span><span class="sxs-lookup"><span data-stu-id="daf61-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="daf61-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="daf61-122">Authorization</span></span>|<span data-ttu-id="daf61-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="daf61-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="daf61-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="daf61-124">Accept</span></span>|<span data-ttu-id="daf61-125">application/json</span><span class="sxs-lookup"><span data-stu-id="daf61-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="daf61-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="daf61-126">Request body</span></span>
<span data-ttu-id="daf61-127">No corpo da solicitação, forneça uma representação JSON do objeto [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) .</span><span class="sxs-lookup"><span data-stu-id="daf61-127">In the request body, supply a JSON representation for the [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) object.</span></span>

<span data-ttu-id="daf61-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md).</span><span class="sxs-lookup"><span data-stu-id="daf61-128">The following table shows the properties that are required when you create the [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md).</span></span>

|<span data-ttu-id="daf61-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="daf61-129">Property</span></span>|<span data-ttu-id="daf61-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="daf61-130">Type</span></span>|<span data-ttu-id="daf61-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="daf61-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="daf61-132">id</span><span class="sxs-lookup"><span data-stu-id="daf61-132">id</span></span>|<span data-ttu-id="daf61-133">String</span><span class="sxs-lookup"><span data-stu-id="daf61-133">String</span></span>|<span data-ttu-id="daf61-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="daf61-134">Key of the entity.</span></span>|
|<span data-ttu-id="daf61-135">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="daf61-135">userPrincipalName</span></span>|<span data-ttu-id="daf61-136">String</span><span class="sxs-lookup"><span data-stu-id="daf61-136">String</span></span>|<span data-ttu-id="daf61-137">Nome de usuário</span><span class="sxs-lookup"><span data-stu-id="daf61-137">User name</span></span>|
|<span data-ttu-id="daf61-138">deviceType</span><span class="sxs-lookup"><span data-stu-id="daf61-138">deviceType</span></span>|[<span data-ttu-id="daf61-139">deviceTypes</span><span class="sxs-lookup"><span data-stu-id="daf61-139">deviceTypes</span></span>](../resources/intune-deviceconfig-devicetypes.md)|<span data-ttu-id="daf61-140">Plataforma do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="daf61-140">Platform of the device.</span></span> <span data-ttu-id="daf61-141">Os valores possíveis são `desktop`: `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad` `iPod` `android`,,, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise` ,,,,,,,, , `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="daf61-141">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="daf61-142">osVersion</span><span class="sxs-lookup"><span data-stu-id="daf61-142">osVersion</span></span>|<span data-ttu-id="daf61-143">String</span><span class="sxs-lookup"><span data-stu-id="daf61-143">String</span></span>|<span data-ttu-id="daf61-144">Versão do sistema operacional do dispositivo</span><span class="sxs-lookup"><span data-stu-id="daf61-144">Operating system version of the device</span></span>|
|<span data-ttu-id="daf61-145">tpmSpecificationVersion</span><span class="sxs-lookup"><span data-stu-id="daf61-145">tpmSpecificationVersion</span></span>|<span data-ttu-id="daf61-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="daf61-146">String</span></span>|<span data-ttu-id="daf61-147">Versão do TPM do dispositivo</span><span class="sxs-lookup"><span data-stu-id="daf61-147">Device TPM Version</span></span>|
|<span data-ttu-id="daf61-148">deviceName</span><span class="sxs-lookup"><span data-stu-id="daf61-148">deviceName</span></span>|<span data-ttu-id="daf61-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="daf61-149">String</span></span>|<span data-ttu-id="daf61-150">Nome do dispositivo</span><span class="sxs-lookup"><span data-stu-id="daf61-150">Device name</span></span>|
|<span data-ttu-id="daf61-151">encryptionReadinessState</span><span class="sxs-lookup"><span data-stu-id="daf61-151">encryptionReadinessState</span></span>|[<span data-ttu-id="daf61-152">encryptionReadinessState</span><span class="sxs-lookup"><span data-stu-id="daf61-152">encryptionReadinessState</span></span>](../resources/intune-deviceconfig-encryptionreadinessstate.md)|<span data-ttu-id="daf61-153">Estado de preparação de criptografia.</span><span class="sxs-lookup"><span data-stu-id="daf61-153">Encryption readiness state.</span></span> <span data-ttu-id="daf61-154">Os valores possíveis são: `notReady` e `ready`.</span><span class="sxs-lookup"><span data-stu-id="daf61-154">Possible values are: `notReady`, `ready`.</span></span>|
|<span data-ttu-id="daf61-155">encryptionState</span><span class="sxs-lookup"><span data-stu-id="daf61-155">encryptionState</span></span>|[<span data-ttu-id="daf61-156">encryptionState</span><span class="sxs-lookup"><span data-stu-id="daf61-156">encryptionState</span></span>](../resources/intune-deviceconfig-encryptionstate.md)|<span data-ttu-id="daf61-157">Estado de criptografia do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="daf61-157">Device encryption state.</span></span> <span data-ttu-id="daf61-158">Os valores possíveis são: `notEncrypted` e `encrypted`.</span><span class="sxs-lookup"><span data-stu-id="daf61-158">Possible values are: `notEncrypted`, `encrypted`.</span></span>|
|<span data-ttu-id="daf61-159">encryptionPolicySettingState</span><span class="sxs-lookup"><span data-stu-id="daf61-159">encryptionPolicySettingState</span></span>|[<span data-ttu-id="daf61-160">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="daf61-160">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="daf61-161">Estado da configuração da política de criptografia.</span><span class="sxs-lookup"><span data-stu-id="daf61-161">Encryption policy setting state.</span></span> <span data-ttu-id="daf61-162">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="daf61-162">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="daf61-163">advancedBitLockerStates</span><span class="sxs-lookup"><span data-stu-id="daf61-163">advancedBitLockerStates</span></span>|[<span data-ttu-id="daf61-164">advancedBitLockerState</span><span class="sxs-lookup"><span data-stu-id="daf61-164">advancedBitLockerState</span></span>](../resources/intune-deviceconfig-advancedbitlockerstate.md)|<span data-ttu-id="daf61-165">Estado do BitLocker avançado.</span><span class="sxs-lookup"><span data-stu-id="daf61-165">Advanced BitLocker State.</span></span> <span data-ttu-id="daf61-166">Os valores possíveis são `success`: `noUserConsent`, `osVolumeEncryptionMethodMismatch`, `osVolumeTpmRequired`, `osVolumeTpmOnlyRequired`, `osVolumeTpmPinRequired`, `osVolumeTpmStartupKeyRequired`, `osVolumeTpmPinStartupKeyRequired`, `osVolumeUnprotected`, `recoveryKeyBackupFailed`, `fixedDriveNotEncrypted`, `fixedDriveEncryptionMethodMismatch`, `loggedOnUserNonAdmin`, `windowsRecoveryEnvironmentNotConfigured`, `tpmNotAvailable`, `tpmNotReady`, `networkError`,,,,,,,,,.</span><span class="sxs-lookup"><span data-stu-id="daf61-166">Possible values are: `success`, `noUserConsent`, `osVolumeEncryptionMethodMismatch`, `osVolumeTpmRequired`, `osVolumeTpmOnlyRequired`, `osVolumeTpmPinRequired`, `osVolumeTpmStartupKeyRequired`, `osVolumeTpmPinStartupKeyRequired`, `osVolumeUnprotected`, `recoveryKeyBackupFailed`, `fixedDriveNotEncrypted`, `fixedDriveEncryptionMethodMismatch`, `loggedOnUserNonAdmin`, `windowsRecoveryEnvironmentNotConfigured`, `tpmNotAvailable`, `tpmNotReady`, `networkError`.</span></span>|
|<span data-ttu-id="daf61-167">policyDetails</span><span class="sxs-lookup"><span data-stu-id="daf61-167">policyDetails</span></span>|<span data-ttu-id="daf61-168">coleção [encryptionReportPolicyDetails](../resources/intune-deviceconfig-encryptionreportpolicydetails.md)</span><span class="sxs-lookup"><span data-stu-id="daf61-168">[encryptionReportPolicyDetails](../resources/intune-deviceconfig-encryptionreportpolicydetails.md) collection</span></span>|<span data-ttu-id="daf61-169">Detalhes da política</span><span class="sxs-lookup"><span data-stu-id="daf61-169">Policy Details</span></span>|



## <a name="response"></a><span data-ttu-id="daf61-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="daf61-170">Response</span></span>
<span data-ttu-id="daf61-171">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="daf61-171">If successful, this method returns a `200 OK` response code and an updated [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="daf61-172">Exemplo</span><span class="sxs-lookup"><span data-stu-id="daf61-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="daf61-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="daf61-173">Request</span></span>
<span data-ttu-id="daf61-174">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="daf61-174">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managedDeviceEncryptionStates/{managedDeviceEncryptionStateId}
Content-type: application/json
Content-length: 658

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
  "policyDetails": [
    {
      "@odata.type": "microsoft.graph.encryptionReportPolicyDetails",
      "policyId": "Policy Id value",
      "policyName": "Policy Name value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="daf61-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="daf61-175">Response</span></span>
<span data-ttu-id="daf61-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="daf61-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 707

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
  "policyDetails": [
    {
      "@odata.type": "microsoft.graph.encryptionReportPolicyDetails",
      "policyId": "Policy Id value",
      "policyName": "Policy Name value"
    }
  ]
}
```





