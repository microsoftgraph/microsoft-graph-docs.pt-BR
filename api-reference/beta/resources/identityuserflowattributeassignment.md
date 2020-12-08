---
title: tipo de recurso identityUserFlowAttributeAssignment
description: identityUserFlowAttributeAssignments são usados para coletar identityUserFlowAttributes específicos dentro de um fluxo de usuário.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 80bc6547307914e0d206ea9b5c79073f96fce19c
ms.sourcegitcommit: e68fdfb1124d16265deb8df268d4185d9deacac6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/05/2020
ms.locfileid: "49581277"
---
# <a name="identityuserflowattributeassignment-resource-type"></a>tipo de recurso identityUserFlowAttributeAssignment

Namespace: Microsoft Graph

identityUserFlowAttributeAssignments são usados para coletar identityUserFlowAttributes específicos dentro de um fluxo de usuário. Isso permite o controle sobre os atributos coletados em um fluxo de usuário e fornece opções de personalização sobre como coletar o atributo dentro do fluxo do usuário. Você pode ter vários identityUserFlowAttributeAssignments em um único fluxo de usuário que cria a experiência que o usuário final vê durante a inscrição quando solicitado a fornecer as informações exigidas pelo fluxo de usuário para concluir a inscrição.

## <a name="methods"></a>Methods

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter identityUserFlowAttributeAssignment](../api/identityuserflowattributeassignment-get.md)|[identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md)|Leia as propriedades e os relacionamentos de um objeto identityUserFlowAttributeAssignment.|
|[Atualizar identityUserFlowAttributeAssignment](../api/identityuserflowattributeassignment-update.md)|Nenhum|Atualiza as propriedades de um objeto identityUserFlowAttributeAssignment.|
|[Excluir identityUserFlowAttributeAssignment](../api/identityuserflowattributeassignment-delete.md)|Nenhum|Excluir um objeto identityUserFlowAttributeAssignment específico.|
|[GetOrder](../api/identityuserflowattributeassignment-getorder.md)|[assignmentOrder](../resources/assignmentorder.md)|Obtém a ordem do identityUserFlowAttributes que está sendo coletado dentro de um fluxo de usuário.|
|[SetOrder](../api/identityuserflowattributeassignment-setorder.md)|Nenhum|Define a ordem de coleta de identityUserFlowAttributes em um fluxo de usuário.|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O identificador do identityUserFlowAttributeAssignment. Esse identificador é imutável após sua criação. Esta é uma propriedade somente leitura.|
|displayName|String|O nome de exibição do identityUserFlowAttribute dentro de um fluxo de usuário.|
|IsOptional|Boolean|Determina se o identityUserFlowAttribute é opcional. `true` significa que o usuário não precisa fornecer um valor. `false` significa que o usuário não pode concluir a inscrição sem fornecer um valor.|
|requiresVerification|Boolean|Determina se o identityUserFlowAttribute requer verificação. Isso é usado apenas para verificar o número de telefone ou endereço de email do usuário.|
|userAttributeValues|coleção [userAttributeValuesItem](../resources/userattributevaluesitem.md)|As opções de entrada para o atributo de fluxo do usuário. Aplicável somente quando userinputtype é `radioSingleSelect` , `dropdownSingleSelect` , ou `checkboxMultiSelect` .|
|userinputtype|identityUserFlowAttributeInputType|O tipo de entrada do atributo de fluxo do usuário. Os possíveis valores são: `textBox`, `dateTimeDropdown`, `radioSingleSelect`, `dropdownSingleSelect`, `emailBox`, `checkboxMultiSelect`.|

## <a name="relationships"></a>Relações

|Relação|Tipo|Descrição|
|:---|:---|:---|
|userattribute|[identityUserFlowAttribute](../resources/identityuserflowattribute.md)|O atributo de usuário que você deseja adicionar ao seu fluxo de usuário.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.identityUserFlowAttributeAssignment",
  "baseType": "",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.identityUserFlowAttributeAssignment",
  "id": "String (identifier)",
  "isOptional": "Boolean",
  "requiresVerification": "Boolean",
  "userInputType": "String",
  "userAttributeValues": [
    {
      "@odata.type": "microsoft.graph.userAttributeValuesItem"
    }
  ],
  "displayName": "String"
}
```
