---
title: tipo de recurso bitLockerSystemDrivePolicy
description: Políticas de base de criptografia BitLocker.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 40eeaa88f2e31901f39edc7b52b1a9358db70396
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/09/2020
ms.locfileid: "44179303"
---
# <a name="bitlockersystemdrivepolicy-resource-type"></a>tipo de recurso bitLockerSystemDrivePolicy

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Políticas de base de criptografia BitLocker.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|encryptionMethod|[bitLockerEncryptionMethod](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|Selecione o método de criptografia para unidades do sistema operacional. Os valores possíveis são: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.|
|startupAuthenticationRequired|Boolean|Exigir autenticação adicional na inicialização.|
|startupAuthenticationBlockWithoutTpmChip|Boolean|Indica se é permitido o BitLocker sem um TPM compatível (requer uma senha ou uma chave de inicialização em uma unidade flash USB).|
|startupAuthenticationTpmUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|Indica se a inicialização do TPM é permitida/obrigatória/não permitida. Os valores possíveis são: `blocked`, `required`, `allowed`, `notConfigured`.|
|startupAuthenticationTpmPinUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|Indica se o PIN de inicialização do TPM é permitido/obrigatório/não permitido. Os valores possíveis são: `blocked`, `required`, `allowed`, `notConfigured`.|
|startupAuthenticationTpmKeyUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|Indica se a chave de inicialização do TPM é permitida/obrigatória/não permitida. Os valores possíveis são: `blocked`, `required`, `allowed`, `notConfigured`.|
|startupAuthenticationTpmPinAndKeyUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|Indica se a chave do PIN de inicialização do TPM e a chave são permitidas/obrigatórias/não permitidas. Os valores possíveis são: `blocked`, `required`, `allowed`, `notConfigured`.|
|minimumPinLength|Int32|Indica o comprimento mínimo do PIN de inicialização. Valores válidos de 4 a 20|
|recoveryOptions|[bitLockerRecoveryOptions](../resources/intune-deviceconfig-bitlockerrecoveryoptions.md)|Permite recuperar as unidades do sistema operacional criptografadas do BitLocker na ausência das informações de chave de inicialização necessárias. Essa configuração de política é aplicada quando você ativa o BitLocker.|
|prebootRecoveryEnableMessageAndUrl|Boolean|Habilitar mensagem e URL de recuperação de pré-inicialização. Se requireStartupAuthentication for false, esse valor não será afetado.|
|prebootRecoveryMessage|Cadeia de Caracteres|Define uma mensagem de recuperação personalizada.|
|prebootRecoveryUrl|Cadeia de Caracteres|Define uma URL de recuperação personalizada.|

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



