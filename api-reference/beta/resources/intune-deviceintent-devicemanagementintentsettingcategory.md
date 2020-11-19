---
title: tipo de recurso deviceManagementIntentSettingCategory
description: Entidade que representa uma categoria de configuração de intenção
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 84eaa000bade2b09774d79ce8d4570fb397cd649
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49275703"
---
# <a name="devicemanagementintentsettingcategory-resource-type"></a>tipo de recurso deviceManagementIntentSettingCategory

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Entidade que representa uma categoria de configuração de intenção


Herda de [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceManagementIntentSettingCategories](../api/intune-deviceintent-devicemanagementintentsettingcategory-list.md)|coleção [deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md)|Listar Propriedades e relações dos objetos [deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md) .|
|[Obter deviceManagementIntentSettingCategory](../api/intune-deviceintent-devicemanagementintentsettingcategory-get.md)|[deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md)|Leia as propriedades e as relações do objeto [deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md) .|
|[Criar deviceManagementIntentSettingCategory](../api/intune-deviceintent-devicemanagementintentsettingcategory-create.md)|[deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md)|Criar um novo objeto [deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md) .|
|[Excluir deviceManagementIntentSettingCategory](../api/intune-deviceintent-devicemanagementintentsettingcategory-delete.md)|Nenhum|Exclui [deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md).|
|[Atualizar deviceManagementIntentSettingCategory](../api/intune-deviceintent-devicemanagementintentsettingcategory-update.md)|[deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md)|Atualiza as propriedades de um objeto [deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|A ID de categoria herdada de [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)|
|displayName|String|O nome da categoria herdado de [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)|
|hasRequiredSetting|Booliano|A categoria contém a configuração necessária de nível superior herdada de [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|settingDefinitions|coleção [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)|As definições de configuração desta categoria contêm herdadas de [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)|
|settings|coleção [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|As configurações que esta categoria contém|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementIntentSettingCategory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementIntentSettingCategory",
  "id": "String (identifier)",
  "displayName": "String",
  "hasRequiredSetting": true
}
```




