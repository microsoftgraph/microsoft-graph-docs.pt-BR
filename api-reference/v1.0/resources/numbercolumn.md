---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: NumberColumn
ms.openlocfilehash: 4aaff6539fc9c7ce77029463562c0f8fca57cac6
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/21/2018
ms.locfileid: "23266503"
---
# <a name="numbercolumn-resource-type"></a>Tipo de recurso NumberColumn

O recurso **numberColumn** em um recurso [columnDefinition](columnDefinition.md) indica que os valores da coluna são números.

## <a name="json-representation"></a>Representação JSON

Aqui está uma representação JSON de um recurso **numberColumn**.
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.numberColumn" } -->

```json
{
  "decimalPlaces": "automatic | none | one | two | three | four | five",
  "displayAs": "number | percentage",
  "maximum": 10.551,
  "minimum": 99.993
}
```

## <a name="properties"></a>Propriedades

| Nome da propriedade      | Tipo   | Descrição
|:-------------------|:-------|:-----------------------------------------------
| **decimalPlaces**  | sequência de caracteres | Quantas casas decimais exibir. Consulte abaixo para saber mais sobre os valores possíveis.
| **displayAs**      | sequência de caracteres | Como o valor deve ser apresentado na experiência do usuário. Deve ser `number` ou `percentage`. Se não for especificado, é tratado como `number`.
| **máximo**        | double | O valor máximo permitido.
| **mínimo**        | double | O valor mínimo permitido.

## <a name="decimalplaces"></a>DecimalPlaces

| Valor          | Descrição
|:---------------|:--------------------------------------------------------------
| **automático**  | Padrão. Exibir casas decimais automaticamente conforme necessário.
| **nenhum**       | Não exibir casas decimais.
| **um**        | Exibir sempre uma casa decimal.
| **dois**        | Exibir sempre duas casas decimais.
| **três**      | Exibir sempre três casas decimais.
| **quatro**       | Exibir sempre quatro casas decimais.
| **cinco**       | Exibir sempre cinco casas decimais.

Observação: **decimalPlaces** e **displayAs** aplicam-se a como os números são processados, não armazenados.
Essas propriedades podem ser atualizadas.

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/numbercolumn.md:
      Found potential enums in resource example that weren't defined in a table:(automatic,none,one,two,three,four,five) are in resource, but () are in table",
    "Warning: /api-reference/v1.0/resources/numbercolumn.md:
      Found potential enums in resource example that weren't defined in a table:(number,percentage) are in resource, but () are in table"
  ],
  "tocPath": "Resources/NumberColumn"
} -->
