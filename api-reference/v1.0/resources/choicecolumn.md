---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: ChoiceColumn
localization_priority: Normal
ms.openlocfilehash: 1dddbd4cfa4f26ecc0fd79a430c9d7f725bebbf9
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2019
ms.locfileid: "30481101"
---
# <a name="choicecolumn-resource-type"></a>Tipo de recurso ChoiceColumn

O **choiceColumn** em um recurso [columnDefinition](columndefinition.md) indica que os valores da coluna podem ser selecionados em uma lista de opções.

## <a name="json-representation"></a>Representação JSON

Aqui está uma representação JSON de um recurso **choiceColumn**.
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.choiceColumn" } -->

```json
{
  "allowTextEntry": true,
  "choices": ["red", "blue", "green"],
  "displayAs": "checkBoxes | dropDownMenu | radioButtons"
}
```

## <a name="properties"></a>Propriedades

| Nome da propriedade      | Tipo               | Descrição
|:-------------------|:-------------------|:----------------------------------------------
| **allowTextEntry** | booliano            | Se verdadeiro, permite valores personalizados que não estão em opções configuradas.
| **choices**        | collection(string) | A lista de valores disponíveis para essa coluna.
| **displayAs**      | string             | Como as opções devem ser apresentadas na UX. Deve ser `checkBoxes`, `dropDownMenu` ou `radioButtons`


<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/choicecolumn.md:
      Found potential enums in resource example that weren't defined in a table:(checkBoxes,dropDownMenu,radioButtons) are in resource, but () are in table"
  ],
  "tocPath": "Resources/ChoiceColumn"
} -->
