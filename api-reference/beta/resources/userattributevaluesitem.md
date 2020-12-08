---
title: tipo de recurso userAttributeValuesItem
description: Usado para preencher os valores de um atributo de fluxo de usuário dentro de um fluxo de usuário quando há várias seleções para escolher.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 6fd0d582ef4dcdd83dba6947536c5acdbc14a8cb
ms.sourcegitcommit: e68fdfb1124d16265deb8df268d4185d9deacac6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/05/2020
ms.locfileid: "49581286"
---
# <a name="userattributevaluesitem-resource-type"></a>tipo de recurso userAttributeValuesItem

Namespace: Microsoft Graph

Usado para preencher os valores de um atributo de fluxo de usuário dentro de um fluxo de usuário quando há várias seleções para escolher. userAttributeValuesItem é aplicável ao userInputTypes `radioSingleSelect` , `dropdownSingleSelect` e `checkboxMultiSelect` para um [identityUserFlowAttributeAssignment](..\resources\identityuserflowattributeassignment.md).

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|isDefault|Booliano|Usado para definir o valor como o padrão.|
|nome|String|O nome de exibição da propriedade exibida para o usuário final no fluxo do usuário.|
|value|Cadeia de caracteres|O valor definido quando este item é selecionado.|

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
