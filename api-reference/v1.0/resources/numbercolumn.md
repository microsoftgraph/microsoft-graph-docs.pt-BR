---
author: JeremyKelley
ms.date: 09/11/2017
title: NumberColumn
ms.localizationpriority: medium
description: O recurso numberColumn em um recurso columnDefinition indica que os valores da coluna são números.
ms.prod: sites-and-lists
doc_type: resourcePageType
ms.openlocfilehash: ae1f12b9c5f0f4b21830091c2518e1d66d624fef
ms.sourcegitcommit: 423e698a580c3b902f2816b0216ab9d5b91e6d20
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/12/2022
ms.locfileid: "66034919"
---
# <a name="numbercolumn-resource-type"></a>Tipo de recurso NumberColumn

Namespace: microsoft.graph

O recurso **numberColumn** em um recurso [columnDefinition](columndefinition.md) indica que os valores da coluna são números.

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

## <a name="decimalplaces"></a>DecimalPlaces

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
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/numbercolumn.md:
      Found potential enums in resource example that weren't defined in a table:(automatic,none,one,two,three,four,five) are in resource, but () are in table",
    "Warning: /api-reference/v1.0/resources/numbercolumn.md:
      Found potential enums in resource example that weren't defined in a table:(number,percentage) are in resource, but () are in table"
  ],
  "tocPath": "Resources/NumberColumn"
} -->

