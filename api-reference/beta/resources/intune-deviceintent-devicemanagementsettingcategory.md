---
title: tipo de recurso deviceManagementSettingCategory
description: Entidade que representa uma categoria de configuração
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: bb5402c983588dc53b1654d67bb6955d385e85d3
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49275556"
---
# <a name="devicemanagementsettingcategory-resource-type"></a>tipo de recurso deviceManagementSettingCategory

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Entidade que representa uma categoria de configuração

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceManagementSettingCategories](../api/intune-deviceintent-devicemanagementsettingcategory-list.md)|coleção [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)|Listar Propriedades e relações dos objetos [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) .|
|[Obter deviceManagementSettingCategory](../api/intune-deviceintent-devicemanagementsettingcategory-get.md)|[deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)|Leia as propriedades e as relações do objeto [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) .|
|[Criar deviceManagementSettingCategory](../api/intune-deviceintent-devicemanagementsettingcategory-create.md)|[deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)|Criar um novo objeto [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) .|
|[Excluir deviceManagementSettingCategory](../api/intune-deviceintent-devicemanagementsettingcategory-delete.md)|Nenhum|Exclui [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md).|
|[Atualizar deviceManagementSettingCategory](../api/intune-deviceintent-devicemanagementsettingcategory-update.md)|[deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)|Atualiza as propriedades de um objeto [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|A ID da categoria|
|displayName|String|O nome da categoria|
|hasRequiredSetting|Booliano|A categoria contém a configuração necessária de nível superior|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|settingDefinitions|coleção [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)|As definições de configuração que esta categoria contém|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementSettingCategory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingCategory",
  "id": "String (identifier)",
  "displayName": "String",
  "hasRequiredSetting": true
}
```




