---
title: Tipo de recurso deviceManagementConfigurationSecretSettingValue
description: Graph modelo para um valor de configuração secreto
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4f4b0a332311b99c31070de9cb5dda20837ef2e3
ms.sourcegitcommit: 0076eb6abb89be3dca3575631924a74a5202be30
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/03/2022
ms.locfileid: "64631063"
---
# <a name="devicemanagementconfigurationsecretsettingvalue-resource-type"></a>Tipo de recurso deviceManagementConfigurationSecretSettingValue

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Graph modelo para um valor de configuração secreto


Herda de [deviceManagementConfigurationSimpleSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingvalue.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|settingValueTemplateReference|[deviceManagementConfigurationSettingValueTemplateReference](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvaluetemplatereference.md)|Referência de modelo de valor de configuração Herdada [de deviceManagementConfigurationSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvalue.md)|
|value|Cadeia de caracteres|Valor da configuração secreta.|
|valueState|[deviceManagementConfigurationSecretSettingValueState](../resources/intune-deviceconfigv2-devicemanagementconfigurationsecretsettingvaluestate.md)|Obtém ou define um valor que indica o estado de criptografia da propriedade Value. Os valores possíveis são: `invalid`, `notEncrypted`, `encryptedValueToken`.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationSecretSettingValue"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSecretSettingValue",
  "settingValueTemplateReference": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValueTemplateReference",
    "settingValueTemplateId": "String",
    "useTemplateDefault": true
  },
  "value": "String",
  "valueState": "String"
}
```




