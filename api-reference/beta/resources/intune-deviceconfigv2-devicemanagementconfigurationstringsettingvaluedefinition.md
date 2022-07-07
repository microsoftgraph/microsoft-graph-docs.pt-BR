---
title: Tipo de recurso deviceManagementConfigurationStringSettingValueDefinition
description: Restrições de cadeia de caracteres
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f9071e3b7e497f65f6a64a623770ec56f68d6fde
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2022
ms.locfileid: "66670566"
---
# <a name="devicemanagementconfigurationstringsettingvaluedefinition-resource-type"></a>Tipo de recurso deviceManagementConfigurationStringSettingValueDefinition

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Restrições de cadeia de caracteres


Herda de [deviceManagementConfigurationSettingValueDefinition](../resources/intune-shared-devicemanagementconfigurationsettingvaluedefinition.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|formato|[deviceManagementConfigurationStringFormat](../resources/intune-shared-devicemanagementconfigurationstringformat.md)|Formato predefinido da cadeia de caracteres. Os valores possíveis são: , , , , , , , `version`, `xml`, `date`, `time`, `binary`, , `regEx`, `json`, , , `dateTime`. `surfaceHub``base64``url``ip``guid``email``none`|
|inputValidationSchema|Cadeia de caracteres|Expressão regular ou qualquer esquema xml ou json que a cadeia de caracteres de entrada deve corresponder|
|maximumLength|Int64|Comprimento máximo da cadeia de caracteres. Valores válidos de 0 a 87516|
|Minimumlength|Int64|Comprimento mínimo da cadeia de caracteres. Valores válidos de 0 a 87516|
|isSecret|Boolean|Especifica se a configuração precisa ser tratada como um segredo. As configurações marcadas como sim serão criptografadas em trânsito e em repouso e serão exibidas como asteriscos quando representadas na experiência do usuário.|
|Filetypes|Conjunto de cadeias de caracteres|Tipos de arquivo com suporte para essa configuração.|

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
  "isSecret": true,
  "fileTypes": [
    "String"
  ]
}
```




