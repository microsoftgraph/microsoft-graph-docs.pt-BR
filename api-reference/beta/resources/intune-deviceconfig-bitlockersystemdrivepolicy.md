---
title: tipo de recurso de bitLockerSystemDrivePolicy
description: Políticas de Base de criptografia BitLocker.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 030051faf1405cf15c138384c1b6ab8891fbae95
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27867428"
---
# <a name="bitlockersystemdrivepolicy-resource-type"></a>tipo de recurso de bitLockerSystemDrivePolicy

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Políticas de Base de criptografia BitLocker.
## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|encryptionMethod|[bitLockerEncryptionMethod](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|Selecione o método de criptografia para unidades do sistema operacional. Os valores possíveis são: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.|
|startupAuthenticationRequired|Booliano|Exigem autenticação adicional na inicialização.|
|startupAuthenticationBlockWithoutTpmChip|Booliano|Indica se você deseja permitir BitLocker sem um TPM compatível (exige uma senha ou uma chave de inicialização em uma unidade flash USB).|
|startupAuthenticationTpmUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|Indica se a inicialização do TPM é permitido/necessário/não permitido. Os valores possíveis são: `blocked`, `required`, `allowed`.|
|startupAuthenticationTpmPinUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|Indica se o pin de inicialização TPM é permitido/necessário/não permitido. Os valores possíveis são: `blocked`, `required`, `allowed`.|
|startupAuthenticationTpmKeyUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|Indica se a chave de inicialização do TPM será permitido/necessário/não permitido. Os valores possíveis são: `blocked`, `required`, `allowed`.|
|startupAuthenticationTpmPinAndKeyUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|Indica se a inicialização do TPM fixar chave e chave são permitidos/necessário/não permitido. Os valores possíveis são: `blocked`, `required`, `allowed`.|
|minimumPinLength|Int32|Indica o tamanho mínimo do pin de inicialização. Valores válidos 4 a 20|
|recoveryOptions|[bitLockerRecoveryOptions](../resources/intune-deviceconfig-bitlockerrecoveryoptions.md)|Permite recuperar BitLocker criptografado unidades do sistema operacional na ausência das informações de chave de inicialização necessários. Essa configuração de política é aplicada quando você ativa o BitLocker.|
|prebootRecoveryEnableMessageAndUrl|Booliano|Habilite a mensagem de recuperação antes da inicialização e a Url. Se requireStartupAuthentication for false, esse valor não afeta.|
|prebootRecoveryMessage|Cadeia de caracteres|Define uma mensagem de recuperação personalizada.|
|prebootRecoveryUrl|Cadeia de caracteres|Define uma URL personalizada de recuperação.|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.bitLockerSystemDrivePolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bitLockerSystemDrivePolicy",
  "encryptionMethod": "String",
  "startupAuthenticationRequired": true,
  "startupAuthenticationBlockWithoutTpmChip": true,
  "startupAuthenticationTpmUsage": "String",
  "startupAuthenticationTpmPinUsage": "String",
  "startupAuthenticationTpmKeyUsage": "String",
  "startupAuthenticationTpmPinAndKeyUsage": "String",
  "minimumPinLength": 1024,
  "recoveryOptions": {
    "@odata.type": "microsoft.graph.bitLockerRecoveryOptions",
    "blockDataRecoveryAgent": true,
    "recoveryPasswordUsage": "String",
    "recoveryKeyUsage": "String",
    "hideRecoveryOptions": true,
    "enableRecoveryInformationSaveToStore": true,
    "recoveryInformationToStore": "String",
    "enableBitLockerAfterRecoveryInformationToStore": true
  },
  "prebootRecoveryEnableMessageAndUrl": true,
  "prebootRecoveryMessage": "String",
  "prebootRecoveryUrl": "String"
}
```





