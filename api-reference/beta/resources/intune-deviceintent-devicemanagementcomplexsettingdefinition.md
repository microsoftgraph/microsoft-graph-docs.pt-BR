---
title: tipo de recurso deviceManagementComplexSettingDefinition
description: Entidade que representa a definição de uma configuração complexa
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d4a8017a4ca95d51a3568c53c4197de663b75c2a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43462464"
---
# <a name="devicemanagementcomplexsettingdefinition-resource-type"></a>tipo de recurso deviceManagementComplexSettingDefinition

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Entidade que representa a definição de uma configuração complexa


Herda de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceManagementComplexSettingDefinitions](../api/intune-deviceintent-devicemanagementcomplexsettingdefinition-list.md)|coleção [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md)|Listar Propriedades e relações dos objetos [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) .|
|[Obter deviceManagementComplexSettingDefinition](../api/intune-deviceintent-devicemanagementcomplexsettingdefinition-get.md)|[deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md)|Leia as propriedades e as relações do objeto [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) .|
|[Criar deviceManagementComplexSettingDefinition](../api/intune-deviceintent-devicemanagementcomplexsettingdefinition-create.md)|[deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md)|Criar um novo objeto [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) .|
|[Excluir deviceManagementComplexSettingDefinition](../api/intune-deviceintent-devicemanagementcomplexsettingdefinition-delete.md)|Nenhum|Exclui [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md).|
|[Atualizar deviceManagementComplexSettingDefinition](../api/intune-deviceintent-devicemanagementcomplexsettingdefinition-update.md)|[deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md)|Atualiza as propriedades de um objeto [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|A ID da definição de configuração herdada de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)|
|valueType|[deviceManangementIntentValueType](../resources/intune-deviceintent-devicemanangementintentvaluetype.md)|O tipo de dados do valor herdado de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md). Os possíveis valores são: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.|
|displayName|Cadeia de caracteres|O nome de exibição da configuração herdado de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)|
|isTopLevel|Booliano|Se a configuração for de nível superior, ela poderá ser configurada sem a necessidade de ser encapsulada em uma coleção ou configuração complexa herdada de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)|
|description|String|A descrição da configuração herdada de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)|
|placeholderText|String|Texto do espaço reservado como um exemplo de entrada válida herdada de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)|
|documentationUrl|String|URL para definir a documentação herdada de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)|
|palavras-chave|Coleção de cadeias de caracteres|Palavras-chave associadas à configuração herdadas de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)|
|as|coleção [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)|Conjunto de restrições para o valor de configuração herdado de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)|
|relação|coleção [deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md)|Coleção de dependências em outras configurações herdadas de [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)|
|propertyDefinitionIds|Coleção de cadeias de caracteres|As definições de cada propriedade da configuração complexa|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementComplexSettingDefinition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementComplexSettingDefinition",
  "id": "String (identifier)",
  "valueType": "String",
  "displayName": "String",
  "isTopLevel": true,
  "description": "String",
  "placeholderText": "String",
  "documentationUrl": "String",
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
  ],
  "propertyDefinitionIds": [
    "String"
  ]
}
```



