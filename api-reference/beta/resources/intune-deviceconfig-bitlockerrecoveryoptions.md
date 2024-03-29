---
title: Tipo de recurso bitLockerRecoveryOptions
description: Opções de recuperação do BitLocker.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7c9798225a4d9cb6fe44221a7030e6836803ff51
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59146720"
---
# <a name="bitlockerrecoveryoptions-resource-type"></a>Tipo de recurso bitLockerRecoveryOptions

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Opções de recuperação do BitLocker.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|blockDataRecoveryAgent|Boleano|Indica se o agente de recuperação de dados baseado em certificado deve ser bloqueado.|
|recoveryPasswordUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|Indica se os usuários são permitidos ou necessários para gerar uma senha de recuperação de 48 dígitos para disco fixo ou do sistema. Os valores possíveis são: `blocked`, `required`, `allowed`, `notConfigured`.|
|recoveryKeyUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|Indica se os usuários são permitidos ou necessários para gerar uma chave de recuperação de 256 bits para disco fixo ou do sistema. Os valores possíveis são: `blocked`, `required`, `allowed`, `notConfigured`.|
|hideRecoveryOptions|Boleano|Indica se é possível ou não permitir a exibição de opções de recuperação no Assistente de Instalação do BitLocker para disco fixo ou do sistema.|
|enableRecoveryInformationSaveToStore|Boleano|Indica se as informações de recuperação do BitLocker podem ou não ser armazenadas no AD DS.|
|recoveryInformationToStore|[bitLockerRecoveryInformationType](../resources/intune-deviceconfig-bitlockerrecoveryinformationtype.md)|Configure quais partes das informações de recuperação do BitLocker são armazenadas no AD DS. Os valores possíveis são: `passwordAndKey` e `passwordOnly`.|
|enableBitLockerAfterRecoveryInformationToStore|Boleano|Indica se o BitLocker deve ou não ser habilitado até que as informações de recuperação sejam armazenadas no AD DS.|

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



