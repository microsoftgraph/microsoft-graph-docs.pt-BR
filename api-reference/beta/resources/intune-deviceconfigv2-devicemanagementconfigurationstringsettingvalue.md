---
title: Tipo de recurso deviceManagementConfigurationStringSettingValue
description: Valor de configuração simples
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 70a61ec3525d5aa778f80b8f127eea09d8956830
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59075288"
---
# <a name="devicemanagementconfigurationstringsettingvalue-resource-type"></a>Tipo de recurso deviceManagementConfigurationStringSettingValue

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Valor de configuração simples


Herda de [deviceManagementConfigurationSimpleSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingvalue.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|settingValueTemplateReference|[deviceManagementConfigurationSettingValueTemplateReference](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvaluetemplatereference.md)|Referência de modelo de valor de configuração Herdada [de deviceManagementConfigurationSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvalue.md)|
|value|Cadeia de caracteres|Valor da configuração da cadeia de caracteres.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationStringSettingValue"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationStringSettingValue",
  "settingValueTemplateReference": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValueTemplateReference",
    "settingValueTemplateId": "String",
    "useTemplateDefault": true
  },
  "value": "String"
}
```



