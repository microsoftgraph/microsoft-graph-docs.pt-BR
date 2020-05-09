---
title: tipo de recurso bitLockerRecoveryOptions
description: Opções de recuperação do BitLocker.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9c7a27835025e042d38f0e13c92cb30ccad5eec5
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/09/2020
ms.locfileid: "44179232"
---
# <a name="bitlockerrecoveryoptions-resource-type"></a>tipo de recurso bitLockerRecoveryOptions

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Opções de recuperação do BitLocker.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|blockDataRecoveryAgent|Boolean|Indica se o agente de recuperação de dados baseado em certificado deve ser bloqueado.|
|recoveryPasswordUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|Indica se os usuários são permitidos ou necessários para gerar uma senha de recuperação de 48 dígitos para o disco fixo ou do sistema. Os valores possíveis são: `blocked`, `required`, `allowed`, `notConfigured`.|
|recoveryKeyUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|Indica se os usuários são permitidos ou necessários para gerar uma chave de recuperação de 256 bits para o disco fixo ou do sistema. Os valores possíveis são: `blocked`, `required`, `allowed`, `notConfigured`.|
|hideRecoveryOptions|Boolean|Indica se a exibição das opções de recuperação no assistente de configuração do BitLocker deve ou não ser permitida no disco fixo ou do sistema.|
|enableRecoveryInformationSaveToStore|Boolean|Indica se as informações de recuperação do BitLocker devem ou não ser armazenadas no AD DS.|
|recoveryInformationToStore|[bitLockerRecoveryInformationType](../resources/intune-deviceconfig-bitlockerrecoveryinformationtype.md)|Configure quais partes das informações de recuperação do BitLocker são armazenadas no AD DS. Os valores possíveis são: `passwordAndKey` e `passwordOnly`.|
|enableBitLockerAfterRecoveryInformationToStore|Boolean|Indica se o BitLocker deve ou não ser habilitado até que as informações de recuperação sejam armazenadas no AD DS.|

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



