---
title: Tipo de recurso deviceManagementConfigurationSettingGroupCollectionInstance
description: Definindo instância dentro da política
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a828c826f96b0c781f845a48c71e4ba3e45bc737
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58820419"
---
# <a name="devicemanagementconfigurationsettinggroupcollectioninstance-resource-type"></a>Tipo de recurso deviceManagementConfigurationSettingGroupCollectionInstance

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Definindo instância dentro da política


Herda [de deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|settingDefinitionId|Cadeia de caracteres|Definição Id de definição Herdada [de deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)|
|settingInstanceTemplateReference|[deviceManagementConfigurationSettingInstanceTemplateReference](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplatereference.md)|Referência do modelo de instância de configuração Herdada [de deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingGroupCollectionInstance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSettingGroupCollectionInstance",
  "settingDefinitionId": "String",
  "settingInstanceTemplateReference": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingInstanceTemplateReference",
    "settingInstanceTemplateId": "String"
  }
}
```



