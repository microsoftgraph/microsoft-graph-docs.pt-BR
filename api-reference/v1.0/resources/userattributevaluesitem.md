---
title: Tipo de recurso userAttributeValuesItem
description: Representa valores de atributo de fluxo do usuário dentro de um fluxo de usuário.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 367f5d835f3790c589a8d7d28b7994484fd9613c
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882382"
---
# <a name="userattributevaluesitem-resource-type"></a>Tipo de recurso userAttributeValuesItem

Namespace: microsoft.graph

Representa valores de atributo de fluxo do usuário em um fluxo de usuário quando há várias seleções para escolher.  O userAttributeValuesItem é aplicável ao userInputTypes de , e a `radioSingleSelect` `dropdownSingleSelect` uma `checkboxMultiSelect` [identityUserFlowAttributeAssignment](..\resources\identityuserflowattributeassignment.md).

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|isDefault|Booliano|Determina se o valor é definido como padrão.|
|nome|Cadeia de caracteres|O nome de exibição da propriedade exibida para o usuário no fluxo do usuário.|
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
