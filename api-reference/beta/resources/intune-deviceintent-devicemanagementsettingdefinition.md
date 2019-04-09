---
title: tipo de recurso deviceManagementSettingDefinition
description: Entidade que representa a definição de uma determinada configuração
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1a37046b80ce51a698ba52f08c2693af821b7e52
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/08/2019
ms.locfileid: "31524481"
---
# <a name="devicemanagementsettingdefinition-resource-type"></a>tipo de recurso deviceManagementSettingDefinition

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Entidade que representa a definição de uma determinada configuração

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceManagementSettingDefinitions](../api/intune-deviceintent-devicemanagementsettingdefinition-list.md)|coleção [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)|Listar Propriedades e relações dos objetos [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) .|
|[Obter deviceManagementSettingDefinition](../api/intune-deviceintent-devicemanagementsettingdefinition-get.md)|[deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)|Leia as propriedades e as relações do objeto [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) .|
|[Criar deviceManagementSettingDefinition](../api/intune-deviceintent-devicemanagementsettingdefinition-create.md)|[deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)|Criar um novo objeto [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) .|
|[Excluir deviceManagementSettingDefinition](../api/intune-deviceintent-devicemanagementsettingdefinition-delete.md)|Nenhum|Exclui [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md).|
|[Atualizar deviceManagementSettingDefinition](../api/intune-deviceintent-devicemanagementsettingdefinition-update.md)|[deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)|Atualiza as propriedades de um objeto [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|A ID da definição de configuração|
|valueType|[deviceManangementIntentValueType](../resources/intune-deviceintent-devicemanangementintentvaluetype.md)|O tipo de dados do valor. Os valores possíveis são: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.|
|displayName|Cadeia de Caracteres|O nome de exibição da configuração|
|isTopLevel|Booliano|Se a configuração for de nível superior, ela poderá ser configurada sem a necessidade de ser encapsulada em uma coleção ou configuração complexa|
|description|String|A descrição da configuração|
|documentationUrl|Cadeia de Caracteres|URL para configurar a documentação|
|palavras-chave|Coleção String|Palavras-chave associadas à configuração|
|as|coleção [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)|Conjunto de restrições para o valor de configuração|
|relação|coleção [deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md)|Coleção de dependências em outras configurações|

## <a name="relationships"></a>Relações
Nenhuma

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
  "documentationUrl": "String",
  "keywords": [
    "String"
  ],
  "constraints": [
    {
      "@odata.type": "microsoft.graph.deviceManagementSettingXmlConstraint"
    }
  ],
  "dependencies": [
    {
      "@odata.type": "microsoft.graph.deviceManagementSettingDependency",
      "definitionId": "String",
      "constraints": [
        {
          "@odata.type": "microsoft.graph.deviceManagementSettingXmlConstraint"
        }
      ]
    }
  ]
}
```







