---
title: Tipo de recurso deviceManagementConfigurationStringSettingValueDefinition
description: Restrições de cadeia de caracteres
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a497972c8d84781cb5984993389fdb1163514f0d
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59128841"
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
|inputValidationSchema|Cadeia de Caracteres|Expressão regular ou qualquer esquema xml ou json que a cadeia de caracteres de entrada deve corresponder|
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



