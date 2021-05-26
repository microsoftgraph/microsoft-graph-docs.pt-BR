---
title: Tipo de recurso deviceManagementConfigurationSettingTemplate
description: Modelo de configuração
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: aa1fc478efa5ab541b572686097275aceb82618f
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666770"
---
# <a name="devicemanagementconfigurationsettingtemplate-resource-type"></a>Tipo de recurso deviceManagementConfigurationSettingTemplate

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Modelo de configuração

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceManagementConfigurationSettingTemplates](../api/intune-deviceconfigv2-devicemanagementconfigurationsettingtemplate-list.md)|[Coleção deviceManagementConfigurationSettingTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingtemplate.md)|Listar propriedades e relações dos [objetos deviceManagementConfigurationSettingTemplate.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingtemplate.md)|
|[Obter deviceManagementConfigurationSettingTemplate](../api/intune-deviceconfigv2-devicemanagementconfigurationsettingtemplate-get.md)|[deviceManagementConfigurationSettingTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingtemplate.md)|Leia propriedades e relações do [objeto deviceManagementConfigurationSettingTemplate.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingtemplate.md)|
|[Criar deviceManagementConfigurationSettingTemplate](../api/intune-deviceconfigv2-devicemanagementconfigurationsettingtemplate-create.md)|[deviceManagementConfigurationSettingTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingtemplate.md)|Crie um novo [objeto deviceManagementConfigurationSettingTemplate.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingtemplate.md)|
|[Excluir deviceManagementConfigurationSettingTemplate](../api/intune-deviceconfigv2-devicemanagementconfigurationsettingtemplate-delete.md)|Nenhuma|Exclui um [deviceManagementConfigurationSettingTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingtemplate.md).|
|[Atualizar deviceManagementConfigurationSettingTemplate](../api/intune-deviceconfigv2-devicemanagementconfigurationsettingtemplate-update.md)|[deviceManagementConfigurationSettingTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingtemplate.md)|Atualize as propriedades de [um objeto deviceManagementConfigurationSettingTemplate.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingtemplate.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave deste modelo de configuração no modelo de política que o contém. Gerado automaticamente.|
|settingInstanceTemplate|[deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)|Modelo de instância de configuração|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|settingDefinitions|[Coleção deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)|Lista de definições de configuração relacionadas|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSettingTemplate",
  "id": "String (identifier)",
  "settingInstanceTemplate": {
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
}
```




