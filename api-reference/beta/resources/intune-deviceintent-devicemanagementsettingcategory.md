---
title: Tipo de recurso deviceManagementSettingCategory
description: Entidade que representa uma categoria de configuração
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7dd0e8d84dbe5f55f6c6e24764d5cddabe036174
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59091430"
---
# <a name="devicemanagementsettingcategory-resource-type"></a>Tipo de recurso deviceManagementSettingCategory

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Entidade que representa uma categoria de configuração

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceManagementSettingCategories](../api/intune-deviceintent-devicemanagementsettingcategory-list.md)|[Coleção deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)|Listar propriedades e relações dos [objetos deviceManagementSettingCategory.](../resources/intune-deviceintent-devicemanagementsettingcategory.md)|
|[Obter deviceManagementSettingCategory](../api/intune-deviceintent-devicemanagementsettingcategory-get.md)|[deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)|Leia propriedades e relações do [objeto deviceManagementSettingCategory.](../resources/intune-deviceintent-devicemanagementsettingcategory.md)|
|[Criar deviceManagementSettingCategory](../api/intune-deviceintent-devicemanagementsettingcategory-create.md)|[deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)|Crie um novo [objeto deviceManagementSettingCategory.](../resources/intune-deviceintent-devicemanagementsettingcategory.md)|
|[Excluir deviceManagementSettingCategory](../api/intune-deviceintent-devicemanagementsettingcategory-delete.md)|Nenhum|Exclui um [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md).|
|[Atualizar deviceManagementSettingCategory](../api/intune-deviceintent-devicemanagementsettingcategory-update.md)|[deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)|Atualize as propriedades de [um objeto deviceManagementSettingCategory.](../resources/intune-deviceintent-devicemanagementsettingcategory.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|A ID da categoria|
|displayName|Cadeia de caracteres|O nome da categoria|
|hasRequiredSetting|Boleano|A categoria contém a configuração necessária de nível superior|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|settingDefinitions|[Coleção deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)|As definições de configuração que essa categoria contém|

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



