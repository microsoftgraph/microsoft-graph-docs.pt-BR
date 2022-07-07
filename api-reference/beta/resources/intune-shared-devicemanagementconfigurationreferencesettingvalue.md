---
title: Tipo de recurso deviceManagementConfigurationReferenceSettingValue
description: Modelo para ReferenceSettingValue
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: edc233723cc655b6f0d731bceab9f10a1d92644c
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2022
ms.locfileid: "66671450"
---
# <a name="devicemanagementconfigurationreferencesettingvalue-resource-type"></a>Tipo de recurso deviceManagementConfigurationReferenceSettingValue

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Modelo para ReferenceSettingValue


Herda [de deviceManagementConfigurationStringSettingValue](../resources/intune-shared-devicemanagementconfigurationstringsettingvalue.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|settingValueTemplateReference|[deviceManagementConfigurationSettingValueTemplateReference](../resources/intune-shared-devicemanagementconfigurationsettingvaluetemplatereference.md)|Referência de modelo de valor de configuração Herdada [de deviceManagementConfigurationSettingValue](../resources/intune-shared-devicemanagementconfigurationsettingvalue.md)|
|value|Cadeia de caracteres|Valor da configuração da cadeia de caracteres. Herdado [de deviceManagementConfigurationStringSettingValue](../resources/intune-shared-devicemanagementconfigurationstringsettingvalue.md)|
|Nota|Cadeia de caracteres|Uma observação que o administrador pode usar para colocar algumas informações contextuais|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationReferenceSettingValue"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationReferenceSettingValue",
  "settingValueTemplateReference": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValueTemplateReference",
    "settingValueTemplateId": "String",
    "useTemplateDefault": true
  },
  "value": "String",
  "note": "String"
}
```




