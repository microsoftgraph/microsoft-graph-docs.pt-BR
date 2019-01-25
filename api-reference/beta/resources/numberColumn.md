---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: NumberColumn
localization_priority: Normal
ms.openlocfilehash: cf1f6c6cafd23a5503d645d13e597a8941019fee
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512875"
---
# <a name="numbercolumn-resource-type"></a>Tipo de recurso NumberColumn

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/NumberColumn",
  "suppressions": [
    "Error: /api-reference/beta/resources/numberColumn.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
