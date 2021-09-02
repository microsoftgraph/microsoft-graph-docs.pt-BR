---
title: Tipo de recurso deviceManagementIntentSettingCategory
description: Entidade que representa uma categoria de configuração de intenção
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ea9a9b63a30e0de8ad8fadf167cdbb51ce5df6a5
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58803508"
---
# <a name="devicemanagementintentsettingcategory-resource-type"></a>Tipo de recurso deviceManagementIntentSettingCategory

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Entidade que representa uma categoria de configuração de intenção


Herda [de deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceManagementIntentSettingCategories](../api/intune-deviceintent-devicemanagementintentsettingcategory-list.md)|[Coleção deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md)|Listar propriedades e relações dos [objetos deviceManagementIntentSettingCategory.](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md)|
|[Obter deviceManagementIntentSettingCategory](../api/intune-deviceintent-devicemanagementintentsettingcategory-get.md)|[deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md)|Leia propriedades e relações do [objeto deviceManagementIntentSettingCategory.](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md)|
|[Criar deviceManagementIntentSettingCategory](../api/intune-deviceintent-devicemanagementintentsettingcategory-create.md)|[deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md)|Crie um novo [objeto deviceManagementIntentSettingCategory.](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md)|
|[Excluir deviceManagementIntentSettingCategory](../api/intune-deviceintent-devicemanagementintentsettingcategory-delete.md)|Nenhum(a)|Exclui um [deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md).|
|[Atualizar deviceManagementIntentSettingCategory](../api/intune-deviceintent-devicemanagementintentsettingcategory-update.md)|[deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md)|Atualize as propriedades de [um objeto deviceManagementIntentSettingCategory.](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|A ID da categoria Herdada [de deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)|
|displayName|Cadeia de caracteres|O nome da categoria Herdado [de deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)|
|hasRequiredSetting|Boleano|A categoria contém a configuração de nível superior necessária Herdada [de deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|settingDefinitions|[Coleção deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)|As definições de configuração dessa categoria contêm Herdado de [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)|
|settings|[Coleção deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|As configurações que essa categoria contém|

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



