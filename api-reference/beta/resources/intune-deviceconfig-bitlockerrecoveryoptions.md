---
title: tipo de recurso de bitLockerRecoveryOptions
description: Opções de recuperação do BitLocker.
ms.openlocfilehash: 46af5b52d8305932d0d67ef57d6a1f356182a469
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27035200"
---
# <a name="bitlockerrecoveryoptions-resource-type"></a>tipo de recurso de bitLockerRecoveryOptions

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Opções de recuperação do BitLocker.
## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|blockDataRecoveryAgent|Booliano|Indica se o bloqueio de agente de recuperação de dados baseada em certificado.|
|recoveryPasswordUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|Indica se os usuários são permitidos ou necessárias para gerar uma senha de recuperação de 48 dígitos para fixo ou disco do sistema. Os valores possíveis são: `blocked`, `required`, `allowed`.|
|recoveryKeyUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|Indica se os usuários são permitidos ou necessárias para gerar uma chave de recuperação de 256 bits para fixo ou disco do sistema. Os valores possíveis são: `blocked`, `required`, `allowed`.|
|hideRecoveryOptions|Booliano|Indica se deve ou não permitidas mostrando as opções de recuperação no Assistente de configuração de disco BitLocker para fixo ou disco do sistema.|
|enableRecoveryInformationSaveToStore|Booliano|Indica se deve ou não permitir que as informações de recuperação BitLocker armazenar no AD DS.|
|recoveryInformationToStore|[bitLockerRecoveryInformationType](../resources/intune-deviceconfig-bitlockerrecoveryinformationtype.md)|Configure quais partes de informações de recuperação do BitLocker são armazenadas no AD DS. Os valores possíveis são: `passwordAndKey` e `passwordOnly`.|
|enableBitLockerAfterRecoveryInformationToStore|Booliano|Indica se deseja ou não habilitar o BitLocker até que as informações de recuperação são armazenadas no AD DS.|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.bitLockerRecoveryOptions"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bitLockerRecoveryOptions",
  "blockDataRecoveryAgent": true,
  "recoveryPasswordUsage": "String",
  "recoveryKeyUsage": "String",
  "hideRecoveryOptions": true,
  "enableRecoveryInformationSaveToStore": true,
  "recoveryInformationToStore": "String",
  "enableBitLockerAfterRecoveryInformationToStore": true
}
```





