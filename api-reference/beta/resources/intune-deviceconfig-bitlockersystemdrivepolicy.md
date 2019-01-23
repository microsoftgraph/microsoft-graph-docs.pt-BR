---
title: tipo de recurso de bitLockerSystemDrivePolicy
description: Políticas de Base de criptografia BitLocker.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 9b63d075538508941d012df1e44f7cb563fed20d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425705"
---
# <a name="bitlockersystemdrivepolicy-resource-type"></a>tipo de recurso de bitLockerSystemDrivePolicy

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

Políticas de Base de criptografia BitLocker.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|encryptionMethod|[bitLockerEncryptionMethod](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|Selecione o método de criptografia para unidades do sistema operacional. Os valores possíveis são: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.|
|startupAuthenticationRequired|Boolean|Exigem autenticação adicional na inicialização.|
|startupAuthenticationBlockWithoutTpmChip|Boolean|Indica se você deseja permitir BitLocker sem um TPM compatível (exige uma senha ou uma chave de inicialização em uma unidade flash USB).|
|startupAuthenticationTpmUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|Indica se a inicialização do TPM é permitido/necessário/não permitido. Os valores possíveis são: `blocked`, `required`, `allowed`.|
|startupAuthenticationTpmPinUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|Indica se o pin de inicialização TPM é permitido/necessário/não permitido. Os valores possíveis são: `blocked`, `required`, `allowed`.|
|startupAuthenticationTpmKeyUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|Indica se a chave de inicialização do TPM será permitido/necessário/não permitido. Os valores possíveis são: `blocked`, `required`, `allowed`.|
|startupAuthenticationTpmPinAndKeyUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|Indica se a inicialização do TPM fixar chave e chave são permitidos/necessário/não permitido. Os valores possíveis são: `blocked`, `required`, `allowed`.|
|minimumPinLength|Int32|Indica o tamanho mínimo do pin de inicialização. Valores válidos 4 a 20|
|recoveryOptions|[bitLockerRecoveryOptions](../resources/intune-deviceconfig-bitlockerrecoveryoptions.md)|Permite recuperar BitLocker criptografado unidades do sistema operacional na ausência das informações de chave de inicialização necessários. Essa configuração de política é aplicada quando você ativa o BitLocker.|
|prebootRecoveryEnableMessageAndUrl|Boolean|Habilite a mensagem de recuperação antes da inicialização e a Url. Se requireStartupAuthentication for false, esse valor não afeta.|
|prebootRecoveryMessage|String|Define uma mensagem de recuperação personalizada.|
|prebootRecoveryUrl|String|Define uma URL personalizada de recuperação.|

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




