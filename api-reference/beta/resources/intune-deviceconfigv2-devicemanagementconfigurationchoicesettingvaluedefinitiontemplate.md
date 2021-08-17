---
title: Tipo de recurso deviceManagementConfigurationChoiceSettingValueDefinitionTemplate
description: Modelo de definição de valor de configuração de opção
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f3dfb38c67777344f5489c4593d89dcd140370abf0d77e5a874ae50656ef6f35
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54193724"
---
# <a name="devicemanagementconfigurationchoicesettingvaluedefinitiontemplate-resource-type"></a>Tipo de recurso deviceManagementConfigurationChoiceSettingValueDefinitionTemplate

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Modelo de definição de valor de configuração de opção

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|allowedOptions|[Coleção deviceManagementConfigurationOptionDefinitionTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationoptiondefinitiontemplate.md)|Opções permitidas de configuração de opção|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValueDefinitionTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationChoiceSettingValueDefinitionTemplate",
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
}
```




