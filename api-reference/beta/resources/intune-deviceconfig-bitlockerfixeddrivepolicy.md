---
title: tipo de recurso bitLockerFixedDrivePolicy
description: Políticas de unidade fixa do BitLocker.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7cc2441e03164787db5374827e0fd4ec153a8819
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562731"
---
# <a name="bitlockerfixeddrivepolicy-resource-type"></a>tipo de recurso bitLockerFixedDrivePolicy

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Políticas de unidade fixa do BitLocker.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|encryptionMethod|[bitLockerEncryptionMethod](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|Selecione o método de criptografia para unidades fixas. Os valores possíveis são: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.|
|requireEncryptionForWriteAccess|Booliano|Essa configuração de política determina se é necessário proteger o BitLocker para unidades de dados fixas em um computador.|
|recoveryOptions|[bitLockerRecoveryOptions](../resources/intune-deviceconfig-bitlockerrecoveryoptions.md)|Essa configuração de política permite controlar como as unidades de dados fixas protegidas por BitLocker são recuperadas na ausência das credenciais necessárias. Essa configuração de política é aplicada quando você ativa o BitLocker.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.bitLockerFixedDrivePolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bitLockerFixedDrivePolicy",
  "encryptionMethod": "String",
  "requireEncryptionForWriteAccess": true,
  "recoveryOptions": {
    "@odata.type": "microsoft.graph.bitLockerRecoveryOptions",
    "blockDataRecoveryAgent": true,
    "recoveryPasswordUsage": "String",
    "recoveryKeyUsage": "String",
    "hideRecoveryOptions": true,
    "enableRecoveryInformationSaveToStore": true,
    "recoveryInformationToStore": "String",
    "enableBitLockerAfterRecoveryInformationToStore": true
  }
}
```





