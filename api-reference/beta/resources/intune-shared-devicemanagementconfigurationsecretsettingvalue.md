---
title: Tipo de recurso deviceManagementConfigurationSecretSettingValue
description: Modelo de grafo para um valor de configuração de segredo
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9e732d13e40fd3c745218c64d0cad9b2af46ee12
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2022
ms.locfileid: "66671462"
---
# <a name="devicemanagementconfigurationsecretsettingvalue-resource-type"></a>Tipo de recurso deviceManagementConfigurationSecretSettingValue

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Modelo de grafo para um valor de configuração de segredo


Herda de [deviceManagementConfigurationSimpleSettingValue](../resources/intune-shared-devicemanagementconfigurationsimplesettingvalue.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|settingValueTemplateReference|[deviceManagementConfigurationSettingValueTemplateReference](../resources/intune-shared-devicemanagementconfigurationsettingvaluetemplatereference.md)|Referência de modelo de valor de configuração Herdada [de deviceManagementConfigurationSettingValue](../resources/intune-shared-devicemanagementconfigurationsettingvalue.md)|
|value|Cadeia de caracteres|Valor da configuração de segredo.|
|valueState|[deviceManagementConfigurationSecretSettingValueState](../resources/intune-shared-devicemanagementconfigurationsecretsettingvaluestate.md)|Obtém ou define um valor que indica o estado de criptografia da propriedade Value. Os valores possíveis são: `invalid`, `notEncrypted`, `encryptedValueToken`.|

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




