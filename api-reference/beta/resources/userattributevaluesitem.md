---
title: Tipo de recurso userAttributeValuesItem
description: Usado para preencher os valores de um atributo de fluxo de usuário dentro de um fluxo de usuário quando há várias seleções para escolher.
author: jkdouglas
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 3468ed1545c8be12f906182f34f5260897f461ba
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59056995"
---
# <a name="userattributevaluesitem-resource-type"></a>Tipo de recurso userAttributeValuesItem

Namespace: microsoft.graph

Usado para preencher os valores de um atributo de fluxo de usuário dentro de um fluxo de usuário quando há várias seleções para escolher. userAttributeValuesItem é aplicável ao userInputTypes `radioSingleSelect` , e a uma `dropdownSingleSelect` `checkboxMultiSelect` [identityUserFlowAttributeAssignment](..\resources\identityuserflowattributeassignment.md).

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|isDefault|Booliano|Usado para definir o valor como padrão.|
|nome|Cadeia de caracteres|O nome de exibição da propriedade exibida para o usuário final no fluxo do usuário.|
|value|Cadeia de caracteres|O valor que é definido quando esse item é selecionado.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userAttributeValuesItem"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.userAttributeValuesItem",
  "name": "String",
  "value": "String",
  "isDefault": "Boolean"
}
```
