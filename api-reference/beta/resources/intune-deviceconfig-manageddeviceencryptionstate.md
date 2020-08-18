---
title: tipo de recurso managedDeviceEncryptionState
description: Relatório de criptografia por dispositivo
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 532f252480ca094a6fcbd0b530f3e30f452cf816
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/18/2020
ms.locfileid: "46790144"
---
# <a name="manageddeviceencryptionstate-resource-type"></a>tipo de recurso managedDeviceEncryptionState

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Relatório de criptografia por dispositivo

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar managedDeviceEncryptionStates](../api/intune-deviceconfig-manageddeviceencryptionstate-list.md)|coleção [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)|Listar Propriedades e relações dos objetos [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) .|
|[Obter managedDeviceEncryptionState](../api/intune-deviceconfig-manageddeviceencryptionstate-get.md)|[managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)|Leia as propriedades e as relações do objeto [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) .|
|[Criar managedDeviceEncryptionState](../api/intune-deviceconfig-manageddeviceencryptionstate-create.md)|[managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)|Criar um novo objeto [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) .|
|[Excluir managedDeviceEncryptionState](../api/intune-deviceconfig-manageddeviceencryptionstate-delete.md)|Nenhum|Exclui [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md).|
|[Atualizar managedDeviceEncryptionState](../api/intune-deviceconfig-manageddeviceencryptionstate-update.md)|[managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)|Atualiza as propriedades de um objeto [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade.|
|userPrincipalName|String|Nome de usuário|
|deviceType|[deviceTypes](../resources/intune-shared-devicetype.md)|Plataforma do dispositivo. Os valores possíveis são:,,,,,,,,,,,,,,,,,,,, `desktop` `windowsRT` `winMO6` `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer` , `unix` , `macMDM` ,, `holoLens` `surfaceHub` , `androidForWork` `androidEnterprise` `blackberry` `palm` `unknown` ,,,,,.|
|osVersion|String|Versão do sistema operacional do dispositivo|
|tpmSpecificationVersion|String|Versão do TPM do dispositivo|
|deviceName|String|Nome do dispositivo|
|encryptionReadinessState|[encryptionReadinessState](../resources/intune-deviceconfig-encryptionreadinessstate.md)|Estado de preparação de criptografia. Os valores possíveis são: `notReady` e `ready`.|
|encryptionState|[encryptionState](../resources/intune-deviceconfig-encryptionstate.md)|Estado de criptografia do dispositivo. Os valores possíveis são: `notEncrypted` e `encrypted`.|
|encryptionPolicySettingState|[complianceStatus](../resources/intune-shared-compliancestatus.md)|Estado da configuração da política de criptografia. Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.|
|advancedBitLockerStates|[advancedBitLockerState](../resources/intune-deviceconfig-advancedbitlockerstate.md)|Estado do BitLocker avançado. Os valores possíveis são:, `success` `noUserConsent` , `osVolumeEncryptionMethodMismatch` , `osVolumeTpmRequired` , `osVolumeTpmOnlyRequired` , `osVolumeTpmPinRequired` ,,,,,,,,,,,,,,, `osVolumeTpmStartupKeyRequired` `osVolumeTpmPinStartupKeyRequired` `osVolumeUnprotected` `recoveryKeyBackupFailed` `fixedDriveNotEncrypted` `fixedDriveEncryptionMethodMismatch` `loggedOnUserNonAdmin` , `windowsRecoveryEnvironmentNotConfigured` , `tpmNotAvailable` , `tpmNotReady` , `networkError` .|
|fileVaultStates|[fileVaultState](../resources/intune-deviceconfig-filevaultstate.md)|Estado FileVault. Os valores possíveis são: `success`, `driveEncryptedByUser`, `userDeferredEncryption`, `escrowNotEnabled`.|
|policyDetails|coleção [encryptionReportPolicyDetails](../resources/intune-deviceconfig-encryptionreportpolicydetails.md)|Detalhes da política|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDeviceEncryptionState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceEncryptionState",
  "id": "String (identifier)",
  "userPrincipalName": "String",
  "deviceType": "String",
  "osVersion": "String",
  "tpmSpecificationVersion": "String",
  "deviceName": "String",
  "encryptionReadinessState": "String",
  "encryptionState": "String",
  "encryptionPolicySettingState": "String",
  "advancedBitLockerStates": "String",
  "fileVaultStates": "String",
  "policyDetails": [
    {
      "@odata.type": "microsoft.graph.encryptionReportPolicyDetails",
      "policyId": "String",
      "policyName": "String"
    }
  ]
}
```



