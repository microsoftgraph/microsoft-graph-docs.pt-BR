---
title: tipo de recurso identityUserFlowAttributeAssignment
description: identityUserFlowAttributeAssignments são usados para coletar identidade específicaUserFlowAttributes em um fluxo de usuário.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 0b1b0addc48b96eeb3f19c9acf2a8b01e8891efb
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440224"
---
# <a name="identityuserflowattributeassignment-resource-type"></a>tipo de recurso identityUserFlowAttributeAssignment

Namespace: microsoft.graph

identityUserFlowAttributeAssignments são usados para coletar identidade específicaUserFlowAttributes em um fluxo de usuário. Isso permite o controle sobre os atributos coletados em um fluxo de usuários e fornece opções de personalização sobre como coletar o atributo dentro do fluxo do usuário. Você pode ter várias identidadesUserFlowAttributeAssignments em um único fluxo de usuários que cria a experiência que o usuário final vê durante a assinatura quando solicitado a fornecer as informações necessárias pelo fluxo do usuário para concluir a assinatura.

## <a name="methods"></a>Methods

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter identityUserFlowAttributeAssignment](../api/identityuserflowattributeassignment-get.md)|[identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md)|Leia as propriedades e as relações de um objeto identityUserFlowAttributeAssignment.|
|[Atualizar identityUserFlowAttributeAssignment](../api/identityuserflowattributeassignment-update.md)|Nenhum(a)|Atualize as propriedades de um objeto identityUserFlowAttributeAssignment.|
|[Excluir identityUserFlowAttributeAssignment](../api/identityuserflowattributeassignment-delete.md)|Nenhum(a)|Exclua um objeto identityUserFlowAttributeAssignment específico.|
|[getOrder](../api/identityuserflowattributeassignment-getorder.md)|[assignmentOrder](../resources/assignmentorder.md)|Obtém a ordem da identityUserFlowAttributes sendo coletada dentro de um fluxo de usuário.|
|[setOrder](../api/identityuserflowattributeassignment-setorder.md)|Nenhum(a)|Define a ordem da identidadeUserFlowAttributes sendo coletada dentro de um fluxo de usuários.|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O identificador da identityUserFlowAttributeAssignment. Esse identificador é imutável depois de criado. Esta é uma propriedade somente leitura.|
|displayName|String|O nome de exibição da identityUserFlowAttribute em um fluxo de usuário.|
|isOptional|Booliano|Determina se identityUserFlowAttribute é opcional. `true` significa que o usuário não precisa fornecer um valor. `false` significa que o usuário não pode concluir a assinatura sem fornecer um valor.|
|requiresVerification|Booliano|Determina se identityUserFlowAttribute requer verificação. Isso só é usado para verificar o número de telefone ou o endereço de email do usuário.|
|userAttributeValues|[Coleção userAttributeValuesItem](../resources/userattributevaluesitem.md)|As opções de entrada para o atributo de fluxo do usuário. Aplicável somente quando o userInputType `radioSingleSelect` for `dropdownSingleSelect` , ou `checkboxMultiSelect` .|
|userInputType|identityUserFlowAttributeInputType|O tipo de entrada do atributo de fluxo do usuário. Os possíveis valores são: `textBox`, `dateTimeDropdown`, `radioSingleSelect`, `dropdownSingleSelect`, `emailBox`, `checkboxMultiSelect`.|

## <a name="relationships"></a>Relações

|Relação|Tipo|Descrição|
|:---|:---|:---|
|userAttribute|[identityUserFlowAttribute](../resources/identityuserflowattribute.md)|O atributo do usuário que você deseja adicionar ao seu fluxo de usuários.|

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
