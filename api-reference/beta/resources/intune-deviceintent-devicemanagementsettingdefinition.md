---
title: Tipo de recurso deviceManagementSettingDefinition
description: Entidade que representa a definição de uma determinada configuração
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a424a11e5a86b175a405e405253d776166b9b9ab
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59134952"
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
|[Excluir deviceManagementSettingDefinition](../api/intune-deviceintent-devicemanagementsettingdefinition-delete.md)|Nenhum|Exclui um [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md).|
|[Atualizar deviceManagementSettingDefinition](../api/intune-deviceintent-devicemanagementsettingdefinition-update.md)|[deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)|Atualize as propriedades de [um objeto deviceManagementSettingDefinition.](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|A ID da definição de configuração|
|valueType|[deviceManangementIntentValueType](../resources/intune-deviceintent-devicemanangementintentvaluetype.md)|O tipo de dados do valor. Os possíveis valores são: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.|
|displayName|Cadeia de caracteres|O nome de exibição da configuração|
|isTopLevel|Boleano|Se a configuração for de nível superior, ela poderá ser configurada sem a necessidade de ser empacotada em uma coleção ou configuração complexa|
|description|Cadeia de caracteres|Descrição da configuração|
|placeholderText|Cadeia de Caracteres|Texto de espaço reservado como exemplo de entrada válida|
|documentationUrl|Cadeia de Caracteres|Url para a documentação de configuração|
|headerTitle|Cadeia de Caracteres|título do header de configuração representa uma categoria/seção de uma configuração/configurações|
|headerSubtitle|Cadeia de Caracteres|subtítulo do header de configuração para obter mais detalhes sobre a categoria/seção|
|palavras-chave|String collection|Palavras-chave associadas à configuração|
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



