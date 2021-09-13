---
title: Tipo de recurso deviceManagementConfigurationSimpleSettingValue
description: Valor de configuração simples
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 590db3f86684681be483bbeb4ab5e4467f5bf7ce
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59040285"
---
# <a name="devicemanagementconfigurationsimplesettingvalue-resource-type"></a>Tipo de recurso deviceManagementConfigurationSimpleSettingValue

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Valor de configuração simples


Herda de [deviceManagementConfigurationSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvalue.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|settingValueTemplateReference|[deviceManagementConfigurationSettingValueTemplateReference](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvaluetemplatereference.md)|Referência de modelo de valor de configuração Herdada [de deviceManagementConfigurationSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvalue.md)|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationSimpleSettingValue"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSimpleSettingValue",
  "settingValueTemplateReference": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValueTemplateReference",
    "settingValueTemplateId": "String",
    "useTemplateDefault": true
  }
}
```



