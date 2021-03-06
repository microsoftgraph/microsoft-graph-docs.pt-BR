---
title: Tipo de recurso deviceManagementConfigurationCategory
description: Política de Configuração de Gerenciamento de Dispositivos
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c3a9bdfceabe13c98ac8c559aa7901336942c5bf
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50433107"
---
# <a name="devicemanagementconfigurationcategory-resource-type"></a>Tipo de recurso deviceManagementConfigurationCategory

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Política de Configuração de Gerenciamento de Dispositivos

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceManagementConfigurationCategories](../api/intune-deviceconfigv2-devicemanagementconfigurationcategory-list.md)|[Coleção deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md)|Listar propriedades e relações dos [objetos deviceManagementConfigurationCategory.](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md)|
|[Obter deviceManagementConfigurationCategory](../api/intune-deviceconfigv2-devicemanagementconfigurationcategory-get.md)|[deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md)|Leia propriedades e relações do [objeto deviceManagementConfigurationCategory.](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md)|
|[Criar deviceManagementConfigurationCategory](../api/intune-deviceconfigv2-devicemanagementconfigurationcategory-create.md)|[deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md)|Crie um novo [objeto deviceManagementConfigurationCategory.](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md)|
|[Excluir deviceManagementConfigurationCategory](../api/intune-deviceconfigv2-devicemanagementconfigurationcategory-delete.md)|Nenhum(a)|Exclui um [deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md).|
|[Atualizar deviceManagementConfigurationCategory](../api/intune-deviceconfigv2-devicemanagementconfigurationcategory-update.md)|[deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md)|Atualize as propriedades de [um objeto deviceManagementConfigurationCategory.](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Identificador de item|
|descrição|String|Descrição do item|
|helpText|String|Texto de ajuda do item|
|nome|String|Nome do item|
|displayName|String|Nome de exibição do item|
|plataformas|[deviceManagementConfigurationPlatforms](../resources/intune-deviceconfigv2-devicemanagementconfigurationplatforms.md)|Tipos de plataformas, que configurações na categoria têm. Os valores possíveis são: `none`, `macOS`, `windows10X`, `windows10`.|
|technologies|[deviceManagementConfigurationTechnologies](../resources/intune-deviceconfigv2-devicemanagementconfigurationtechnologies.md)|Tipos de tecnologias, que configurações na categoria têm. Os valores possíveis são: `none`, `mdm`, `windows10XManagement`, `configManager`.|
|settingUsage|[deviceManagementConfigurationSettingUsage](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingusage.md)|Indica que a categoria contém configurações usadas para Conformidade ou Configuração. Os valores possíveis são: `none` e `configuration`.|
|parentCategoryId|String|ID pai da categoria.|
|rootCategoryId|String|ID raiz da categoria.|
|childCategoryIds|Coleção de cadeias de caracteres|Lista de IDs filho da categoria.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationCategory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationCategory",
  "id": "String (identifier)",
  "description": "String",
  "helpText": "String",
  "name": "String",
  "displayName": "String",
  "platforms": "String",
  "technologies": "String",
  "settingUsage": "String",
  "parentCategoryId": "String",
  "rootCategoryId": "String",
  "childCategoryIds": [
    "String"
  ]
}
```




