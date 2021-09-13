---
title: Tipo de recurso userAttributeValuesItem
description: Representa valores de atributo de fluxo do usuário dentro de um fluxo de usuário.
author: jkdouglas
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 690b9f53762359ab559fb98534525cad15e5e282
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59083961"
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
