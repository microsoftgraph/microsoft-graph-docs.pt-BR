---
title: Tipo de recurso deviceManagementConfigurationChoiceSettingInstanceTemplate
description: Modelo de instância de configuração de opção
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f8448978899a254b66d2494eb09e9fa8b08b8293
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58786646"
---
# <a name="devicemanagementconfigurationchoicesettinginstancetemplate-resource-type"></a>Tipo de recurso deviceManagementConfigurationChoiceSettingInstanceTemplate

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Modelo de instância de configuração de opção


Herda de [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|settingInstanceTemplateId|Cadeia de caracteres|Id do modelo de instância de configuração Herdada [de deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)|
|settingDefinitionId|Cadeia de caracteres|Definição Id De definição Herdada [de deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)|
|isRequired|Booliano|Indica se uma política deve especificar essa configuração. Herdado [de deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)|
|choiceSettingValueTemplate|[deviceManagementConfigurationChoiceSettingValueTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingvaluetemplate.md)|Modelo de valor de configuração de opção|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstanceTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationChoiceSettingInstanceTemplate",
  "settingInstanceTemplateId": "String",
  "settingDefinitionId": "String",
  "isRequired": true,
  "choiceSettingValueTemplate": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValueTemplate",
    "defaultValue": {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValueConstantDefaultTemplate",
      "settingDefinitionOptionId": "String",
      "children": [
        {
          "@odata.type": "microsoft.graph.deviceManagementConfigurationSimpleSettingInstanceTemplate",
          "settingInstanceTemplateId": "String",
          "settingDefinitionId": "String",
          "isRequired": true,
          "simpleSettingValueTemplate": {
            "@odata.type": "microsoft.graph.deviceManagementConfigurationStringSettingValueTemplate",
            "settingValueTemplateId": "String",
            "defaultValue": {
              "@odata.type": "microsoft.graph.deviceManagementConfigurationStringSettingValueConstantDefaultTemplate",
              "constantValue": "String"
            }
          }
        }
      ]
    },
    "recommendedValueDefinition": {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValueDefinitionTemplate",
      "allowedOptions": [
        {
          "@odata.type": "microsoft.graph.deviceManagementConfigurationOptionDefinitionTemplate",
          "itemId": "String",
          "children": [
            {
              "@odata.type": "microsoft.graph.deviceManagementConfigurationSimpleSettingInstanceTemplate",
              "settingInstanceTemplateId": "String",
              "settingDefinitionId": "String",
              "isRequired": true,
              "simpleSettingValueTemplate": {
                "@odata.type": "microsoft.graph.deviceManagementConfigurationStringSettingValueTemplate",
                "settingValueTemplateId": "String",
                "defaultValue": {
                  "@odata.type": "microsoft.graph.deviceManagementConfigurationStringSettingValueConstantDefaultTemplate",
                  "constantValue": "String"
                }
              }
            }
          ]
        }
      ]
    },
    "requiredValueDefinition": {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValueDefinitionTemplate",
      "allowedOptions": [
        {
          "@odata.type": "microsoft.graph.deviceManagementConfigurationOptionDefinitionTemplate",
          "itemId": "String",
          "children": [
            {
              "@odata.type": "microsoft.graph.deviceManagementConfigurationSimpleSettingInstanceTemplate",
              "settingInstanceTemplateId": "String",
              "settingDefinitionId": "String",
              "isRequired": true,
              "simpleSettingValueTemplate": {
                "@odata.type": "microsoft.graph.deviceManagementConfigurationStringSettingValueTemplate",
                "settingValueTemplateId": "String",
                "defaultValue": {
                  "@odata.type": "microsoft.graph.deviceManagementConfigurationStringSettingValueConstantDefaultTemplate",
                  "constantValue": "String"
                }
              }
            }
          ]
        }
      ]
    },
    "settingValueTemplateId": "String"
  }
}
```



