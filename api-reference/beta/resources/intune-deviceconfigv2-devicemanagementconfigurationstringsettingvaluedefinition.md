---
title: Tipo de recurso deviceManagementConfigurationStringSettingValueDefinition
description: Restrições de cadeia de caracteres
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9731c46e9ae80f346bef29d951f4e430d76743f3
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58815075"
---
# <a name="devicemanagementconfigurationstringsettingvaluedefinition-resource-type"></a>Tipo de recurso deviceManagementConfigurationStringSettingValueDefinition

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Restrições de cadeia de caracteres


Herda [de deviceManagementConfigurationSettingValueDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvaluedefinition.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|formato|[deviceManagementConfigurationStringFormat](../resources/intune-deviceconfigv2-devicemanagementconfigurationstringformat.md)|Formato pré-definido da cadeia de caracteres. Os valores possíveis são: `none` , , , , , , , , , `email` , , `guid` , , , `ip` `base64` `url` , `version` `xml` `date` `time` `binary` `regEx` `json` `dateTime` `surfaceHub` .|
|inputValidationSchema|Cadeia de caracteres|Expressão regular ou qualquer esquema xml ou json que a cadeia de caracteres de entrada deve corresponder|
|maximumLength|Int64|Comprimento máximo da cadeia de caracteres. Valores válidos de 0 a 87516|
|minimumLength|Int64|Comprimento mínimo da cadeia de caracteres. Valores válidos de 0 a 87516|
|isSecret|Boleano|Especifica se a configuração precisa ser tratada como um segredo. Configurações marcados como sim serão criptografados em trânsito e em repouso e serão exibidos como asteriscos quando representados no UX.|

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



