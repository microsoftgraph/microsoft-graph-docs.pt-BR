---
title: Tipo de recurso userAttributeValuesItem
description: Usado para preencher os valores de um atributo de fluxo de usuário dentro de um fluxo de usuário quando há várias seleções para escolher.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 1780e37b8be9952d314f2a95a89975814ffac3483199ae72eb608d1426aa84cd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54145072"
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
