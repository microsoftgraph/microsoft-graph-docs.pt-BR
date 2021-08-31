---
title: Tipo de recurso deviceManagementSettingDefinition
description: Entidade que representa a definição de uma determinada configuração
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 67349cd190321d26dddd6e8ef0397c707b39fd12
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58806226"
---
# <a name="devicemanagementsettingdefinition-resource-type"></a>Tipo de recurso deviceManagementSettingDefinition

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Entidade que representa a definição de uma determinada configuração

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceManagementSettingDefinitions](../api/intune-deviceintent-devicemanagementsettingdefinition-list.md)|[Coleção deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)|Listar propriedades e relações dos [objetos deviceManagementSettingDefinition.](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)|
|[Obter deviceManagementSettingDefinition](../api/intune-deviceintent-devicemanagementsettingdefinition-get.md)|[deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)|Leia propriedades e relações do [objeto deviceManagementSettingDefinition.](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)|
|[Criar deviceManagementSettingDefinition](../api/intune-deviceintent-devicemanagementsettingdefinition-create.md)|[deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)|Crie um novo [objeto deviceManagementSettingDefinition.](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)|
|[Excluir deviceManagementSettingDefinition](../api/intune-deviceintent-devicemanagementsettingdefinition-delete.md)|Nenhum(a)|Exclui um [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md).|
|[Atualizar deviceManagementSettingDefinition](../api/intune-deviceintent-devicemanagementsettingdefinition-update.md)|[deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)|Atualize as propriedades de [um objeto deviceManagementSettingDefinition.](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|A ID da definição de configuração|
|valueType|[deviceManangementIntentValueType](../resources/intune-deviceintent-devicemanangementintentvaluetype.md)|O tipo de dados do valor. Os possíveis valores são: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.|
|displayName|Cadeia de caracteres|O nome de exibição da configuração|
|isTopLevel|Booliano|Se a configuração for de nível superior, ela poderá ser configurada sem a necessidade de ser empacotada em uma coleção ou configuração complexa|
|descrição|Cadeia de caracteres|Descrição da configuração|
|placeholderText|Cadeia de caracteres|Texto de espaço reservado como exemplo de entrada válida|
|documentationUrl|Cadeia de caracteres|Url para a documentação de configuração|
|headerTitle|Cadeia de caracteres|título do header de configuração representa uma categoria/seção de uma configuração/configurações|
|headerSubtitle|Cadeia de caracteres|subtítulo do header de configuração para obter mais detalhes sobre a categoria/seção|
|palavras-chave|Coleção de cadeias de caracteres|Palavras-chave associadas à configuração|
|restrições|[Coleção deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)|Coleção de restrições para o valor de configuração|
|dependencies|[Coleção deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md)|Coleção de dependências em outras configurações|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementSettingDefinition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingDefinition",
  "id": "String (identifier)",
  "valueType": "String",
  "displayName": "String",
  "isTopLevel": true,
  "description": "String",
  "placeholderText": "String",
  "documentationUrl": "String",
  "headerTitle": "String",
  "headerSubtitle": "String",
  "keywords": [
    "String"
  ],
  "constraints": [
    {
      "@odata.type": "microsoft.graph.deviceManagementSettingAppConstraint",
      "supportedTypes": [
        "String"
      ]
    }
  ],
  "dependencies": [
    {
      "@odata.type": "microsoft.graph.deviceManagementSettingDependency",
      "definitionId": "String",
      "constraints": [
        {
          "@odata.type": "microsoft.graph.deviceManagementSettingAppConstraint",
          "supportedTypes": [
            "String"
          ]
        }
      ]
    }
  ]
}
```



