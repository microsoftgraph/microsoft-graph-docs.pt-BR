---
title: Tipo de recurso managedDeviceEncryptionState
description: Relatório de criptografia por dispositivo
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 792b9c0d3e62394b4ea06d389ba3891c133fa63322bb20b157d3803f8afd49e9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54236329"
---
# <a name="manageddeviceencryptionstate-resource-type"></a>Tipo de recurso managedDeviceEncryptionState

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Relatório de criptografia por dispositivo

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar managedDeviceEncryptionStates](../api/intune-deviceconfig-manageddeviceencryptionstate-list.md)|[Coleção managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)|Listar propriedades e relações dos [objetos managedDeviceEncryptionState.](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)|
|[Obter managedDeviceEncryptionState](../api/intune-deviceconfig-manageddeviceencryptionstate-get.md)|[managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)|Leia propriedades e relações do [objeto managedDeviceEncryptionState.](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)|
|[Criar managedDeviceEncryptionState](../api/intune-deviceconfig-manageddeviceencryptionstate-create.md)|[managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)|Crie um novo [objeto managedDeviceEncryptionState.](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)|
|[Excluir managedDeviceEncryptionState](../api/intune-deviceconfig-manageddeviceencryptionstate-delete.md)|Nenhum|Exclui [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md).|
|[Atualizar managedDeviceEncryptionState](../api/intune-deviceconfig-manageddeviceencryptionstate-update.md)|[managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)|Atualize as propriedades de [um objeto managedDeviceEncryptionState.](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)|

## <a name="properties"></a>Propriedades
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




