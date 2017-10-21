---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: NumberColumn
ms.openlocfilehash: 8aa366e3c4f59fc5d22f945c863bab4f91373b67
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/28/2017
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
| **decimalPlaces**  | string | Quantas casas decimais exibir. Consulte abaixo para saber mais sobre os valores possíveis.
| **displayAs**      | string | Como o valor deve ser apresentado na experiência do usuário. Deve ser `number` ou `percentage`. Se não for especificado, é tratado como `number`.
| **maximum**        | double | O valor máximo permitido.
| **minimum**        | double | O valor mínimo permitido.

## <a name="decimalplaces-values"></a>Valores de DecimalPlaces

| Valor          | Descrição
|:---------------|:--------------------------------------------------------------
| **automatic**  | Padrão. Exibir casas decimais automaticamente conforme necessário.
| **none**       | Não exibir casas decimais.
| **one**        | Exibir sempre uma casa decimal.
| **two**        | Exibir sempre duas casas decimais.
| **three**      | Exibir sempre três casas decimais.
| **four**       | Exibir sempre quatro casas decimais.
| **five**       | Exibir sempre cinco casas decimais.

Observação: **decimalPlaces** e **displayAs** aplicam-se a como os números são processados, não armazenados.
Essas propriedades podem ser atualizadas.

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/NumberColumn"
} -->
