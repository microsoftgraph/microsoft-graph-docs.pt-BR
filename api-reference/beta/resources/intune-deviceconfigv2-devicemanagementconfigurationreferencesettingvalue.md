---
title: Tipo de recurso deviceManagementConfigurationReferenceSettingValue
description: Modelo para ReferenceSettingValue
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1656b3e50094a55b4f2fe9ad422bbd54bd62bd6b
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666454"
---
# <a name="devicemanagementconfigurationreferencesettingvalue-resource-type"></a>Tipo de recurso deviceManagementConfigurationReferenceSettingValue

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Modelo para ReferenceSettingValue


Herda [de deviceManagementConfigurationStringSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationstringsettingvalue.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|settingValueTemplateReference|[deviceManagementConfigurationSettingValueTemplateReference](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvaluetemplatereference.md)|Referência de modelo de valor de configuração Herdada [de deviceManagementConfigurationSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvalue.md)|
|value|Cadeia de caracteres|Valor da configuração da cadeia de caracteres. Herdado [de deviceManagementConfigurationStringSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationstringsettingvalue.md)|
|observação|String|Uma observação que o administrador pode usar para colocar algumas informações contextuais|

## <a name="relationships"></a>Relações
Nenhuma

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




