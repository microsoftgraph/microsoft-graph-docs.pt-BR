---
title: Tipo de recurso identityUserFlowAttributeAssignment
description: identityUserFlowAttributeAssignments são usadas para coletar identityUserFlowAttributes específicas em um fluxo de usuário.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 65859cb0d235454577e236761064f4597f5c68d8
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158783"
---
# <a name="identityuserflowattributeassignment-resource-type"></a>Tipo de recurso identityUserFlowAttributeAssignment

Namespace: microsoft.graph

identityUserFlowAttributeAssignments são usadas para coletar identityUserFlowAttributes específicas em um fluxo de usuário. Isso permite o controle sobre os atributos que são coletados em um fluxo de usuário e fornece opções de personalização sobre como coletar o atributo dentro do fluxo do usuário. Você pode ter vários identityUserFlowAttributeAssignments dentro de um único fluxo de usuário que cria a experiência que o usuário final vê durante a assinatura quando solicitado a fornecer as informações necessárias pelo fluxo do usuário para concluir a assinatura.

## <a name="methods"></a>Métodos

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter identityUserFlowAttributeAssignment](../api/identityuserflowattributeassignment-get.md)|[identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md)|Leia as propriedades e os relacionamentos de um objeto identityUserFlowAttributeAssignment.|
|[Atualizar identityUserFlowAttributeAssignment](../api/identityuserflowattributeassignment-update.md)|Nenhum(a)|Atualizar as propriedades de um objeto identityUserFlowAttributeAssignment.|
|[Excluir identityUserFlowAttributeAssignment](../api/identityuserflowattributeassignment-delete.md)|Nenhum(a)|Exclua um objeto identityUserFlowAttributeAssignment específico.|
|[getOrder](../api/identityuserflowattributeassignment-getorder.md)|[assignmentOrder](../resources/assignmentorder.md)|Obtém a ordem dos identityUserFlowAttributes que estão sendo coletados em um fluxo de usuário.|
|[setOrder](../api/identityuserflowattributeassignment-setorder.md)|Nenhum(a)|Define a ordem dos identityUserFlowAttributes que estão sendo coletados em um fluxo de usuário.|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O identificador do identityUserFlowAttributeAssignment. Esse identificador é imutável depois de criado. Esta é uma propriedade somente leitura.|
|displayName|String|O nome de exibição do identityUserFlowAttribute dentro de um fluxo de usuário.|
|isOptional|Boolean|Determina se a identityUserFlowAttribute é opcional. `true` significa que o usuário não precisa fornecer um valor. `false` significa que o usuário não pode concluir a assinatura sem fornecer um valor.|
|requiresVerification|Boolean|Determina se a identityUserFlowAttribute exige verificação. Isso é usado somente para verificar o número de telefone ou endereço de email do usuário.|
|userAttributeValues|[Coleção userAttributeValuesItem](../resources/userattributevaluesitem.md)|As opções de entrada para o atributo de fluxo do usuário. Aplicável somente quando userInputType for `radioSingleSelect` `dropdownSingleSelect` , ou `checkboxMultiSelect` .|
|userInputType|identityUserFlowAttributeInputType|O tipo de entrada do atributo de fluxo do usuário. Os possíveis valores são: `textBox`, `dateTimeDropdown`, `radioSingleSelect`, `dropdownSingleSelect`, `emailBox`, `checkboxMultiSelect`.|

## <a name="relationships"></a>Relações

|Relação|Tipo|Descrição|
|:---|:---|:---|
|userAttribute|[identityUserFlowAttribute](../resources/identityuserflowattribute.md)|O atributo de usuário que você deseja adicionar ao seu fluxo de usuário.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.identityUserFlowAttributeAssignment",
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
