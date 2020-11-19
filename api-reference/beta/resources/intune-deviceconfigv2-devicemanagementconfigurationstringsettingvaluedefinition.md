---
title: tipo de recurso deviceManagementConfigurationStringSettingValueDefinition
description: Restrições de cadeia de caracteres
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 03a96252cffabddd2acb613ff365fd16951fd55c
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49241242"
---
# <a name="devicemanagementconfigurationstringsettingvaluedefinition-resource-type"></a>tipo de recurso deviceManagementConfigurationStringSettingValueDefinition

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Restrições de cadeia de caracteres


Herda de [deviceManagementConfigurationSettingValueDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvaluedefinition.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|formato|[deviceManagementConfigurationStringFormat](../resources/intune-deviceconfigv2-devicemanagementconfigurationstringformat.md)|Formato predefinido da cadeia de caracteres. Os valores possíveis são:, `none` `email` , `guid` , `ip` , `base64` , `url` , `version` , `xml` , `date` , `time` , `binary` , `regEx` ,, `json` `dateTime` `surfaceHub` .|
|inputValidationSchema|String|Expressão regular ou qualquer esquema XML ou JSON que a cadeia de caracteres de entrada deve corresponder|
|maximumLength|Int64|Comprimento máximo da cadeia de caracteres. Valores válidos de 0 a 87516|
|minimumLength|Int64|Comprimento mínimo da cadeia de caracteres. Valores válidos de 0 a 87516|
|issecret|Booliano|Especifica se a configuração deve ser tratada como um segredo. As configurações marcadas como Sim serão criptografadas em trânsito e em repouso e serão exibidas como asteriscos quando forem representadas no UX.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationStringSettingValueDefinition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationStringSettingValueDefinition",
  "format": "String",
  "inputValidationSchema": "String",
  "maximumLength": 1024,
  "minimumLength": 1024,
  "isSecret": true
}
```




