---
title: Tipo de recurso userAttributeValuesItem
description: Representa valores de atributo de fluxo do usuário dentro de um fluxo de usuário.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 88e19bfa02876e08df4c3040ff6bcfefae41840278719b83ccc7b57be651f5a0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54205210"
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
