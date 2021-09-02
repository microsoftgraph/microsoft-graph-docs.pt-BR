---
title: Tipo de recurso deviceManagementConfigurationStringSettingValueTemplate
description: Modelo de valor de configuração de cadeia de caracteres
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0961b4cbb8ff844758a2299d65b60bceb72e2dab
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58805307"
---
# <a name="devicemanagementconfigurationstringsettingvaluetemplate-resource-type"></a>Tipo de recurso deviceManagementConfigurationStringSettingValueTemplate

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Modelo de valor de configuração de cadeia de caracteres


Herda [de deviceManagementConfigurationSimpleSettingValueTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingvaluetemplate.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|settingValueTemplateId|Cadeia de caracteres|Definição da ID do Modelo de Valor Herdada [de deviceManagementConfigurationSimpleSettingValueTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingvaluetemplate.md)|
|defaultValue|[deviceManagementConfigurationStringSettingValueDefaultTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationstringsettingvaluedefaulttemplate.md)|Modelo padrão de valor de configuração de cadeia de caracteres.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationStringSettingValueTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationStringSettingValueTemplate",
  "settingValueTemplateId": "String",
  "defaultValue": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationStringSettingValueConstantDefaultTemplate",
    "constantValue": "String"
  }
}
```



