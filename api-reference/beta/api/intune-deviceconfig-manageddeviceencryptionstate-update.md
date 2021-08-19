---
title: Atualizar managedDeviceEncryptionState
description: Atualize as propriedades de um objeto managedDeviceEncryptionState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e9ebfa7253ae6f30a6f3fb27add96e20b69a2733558091bc6926f040d1c0e83b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54134026"
---
# <a name="update-manageddeviceencryptionstate"></a>Atualizar managedDeviceEncryptionState

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Atualize as propriedades de [um objeto managedDeviceEncryptionState.](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)|DeviceManagementConfiguration.ReadWrite.All|
|Delegada (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managedDeviceEncryptionStates/{managedDeviceEncryptionStateId}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON para o [objeto managedDeviceEncryptionState.](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)

A tabela a seguir mostra as propriedades que são necessárias ao criar [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade.|
|userPrincipalName|Cadeia de caracteres|Nome de usuário|
|deviceType|[deviceTypes](../resources/intune-deviceconfig-devicetypes.md)|Plataforma do dispositivo. Os valores possíveis são: `desktop` , , , , , , , , `windowsRT` `winMO6` , , , `nokia` `windowsPhone` `mac` , `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer` `unix` `macMDM` `holoLens` `surfaceHub` , `androidForWork` `androidEnterprise` `blackberry` `palm` `unknown` , .|
|osVersion|String|Versão do sistema operacional do dispositivo|
|tpmSpecificationVersion|Cadeia de caracteres|Versão TPM do dispositivo|
|deviceName|String|Nome do dispositivo|
|encryptionReadinessState|[encryptionReadinessState](../resources/intune-deviceconfig-encryptionreadinessstate.md)|Estado de preparação da criptografia. Os valores possíveis são: `notReady` e `ready`.|
|encryptionState|[encryptionState](../resources/intune-deviceconfig-encryptionstate.md)|Estado de criptografia de dispositivo. Os valores possíveis são: `notEncrypted` e `encrypted`.|
|encryptionPolicySettingState|[complianceStatus](../resources/intune-shared-compliancestatus.md)|Estado de configuração da política de criptografia. Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.|
|advancedBitLockerStates|[advancedBitLockerState](../resources/intune-deviceconfig-advancedbitlockerstate.md)|Estado avançado do BitLocker. Os valores possíveis são: `success` , , , , , , , , `noUserConsent` , , , `osVolumeUnprotected` , , `osVolumeTpmRequired` , , , `osVolumeTpmOnlyRequired` `osVolumeTpmPinRequired` `osVolumeTpmStartupKeyRequired` , `osVolumeTpmPinStartupKeyRequired` `osVolumeEncryptionMethodMismatch` `recoveryKeyBackupFailed` `fixedDriveNotEncrypted` `fixedDriveEncryptionMethodMismatch` `loggedOnUserNonAdmin` `windowsRecoveryEnvironmentNotConfigured` `tpmNotAvailable` `tpmNotReady` `networkError` .|
|fileVaultStates|[fileVaultState](../resources/intune-deviceconfig-filevaultstate.md)|Estado FileVault. Os valores possíveis são: `success`, `driveEncryptedByUser`, `userDeferredEncryption`, `escrowNotEnabled`.|
|policyDetails|[Coleção encryptionReportPolicyDetails](../resources/intune-deviceconfig-encryptionreportpolicydetails.md)|Detalhes da política|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) atualizado no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
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

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
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




