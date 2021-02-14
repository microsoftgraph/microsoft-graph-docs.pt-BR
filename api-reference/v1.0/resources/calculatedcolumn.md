---
author: JeremyKelley
ms.date: 09/11/2017
title: CalculatedColumn
localization_priority: Normal
description: calculatedColumn em um recurso columnDefinition indica que os dados da coluna são calculados com base em outras colunas do site.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: a75db3ea7a3973d57a3d09aa6cba2cb85a66ce11
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/14/2021
ms.locfileid: "50239076"
---
# <a name="calculatedcolumn-resource-type"></a>Tipo de recurso CalculatedColumn

Namespace: microsoft.graph

**calculatedColumn** em um recurso [columnDefinition](columndefinition.md) indica que os dados da coluna são calculados com base em outras colunas do site.

## <a name="json-representation"></a>Representação JSON

Aqui está uma representação JSON de um recurso **calculatedColumn**.
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.calculatedColumn" } -->

```json
{
  "format": "dateOnly | dateTime",
  "formula": "=[Column1]+[Column2]+[Column3]",
  "outputType": "boolean | currency | dateTime | number | text",
}
```

## <a name="properties"></a>Propriedades

| Nome da propriedade  | Tipo    | Descrição
|:---------------|:--------|:--------------------------------------------------
| **format**     | string  | Nos tipos de saída `dateTime`, o formato do valor. Deve ser `dateOnly` ou `dateTime`.
| **formula**    | string  | A fórmula usada para calcular o valor dessa coluna.
| **outputType** | string  | O tipo de saída usado para formatar valores nessa coluna. Deve ser `boolean`, `currency`, `dateTime`, `number` ou `text`.

As fórmulas do SharePoint usam uma sintaxe semelhante a fórmulas do Excel.
Consulte [Exemplos de fórmulas comuns em listas do SharePoint][SPFormulas] para obter mais informações.

[SPFormulas]: https://support.office.com/en-us/article/Examples-of-common-formulas-in-SharePoint-Lists-d81f5f21-2b4e-45ce-b170-bf7ebf6988b3

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/calculatedcolumn.md:
      Found potential enums in resource example that weren't defined in a table:(dateOnly,dateTime) are in resource, but () are in table",
    "Warning: /api-reference/v1.0/resources/calculatedcolumn.md:
      Found potential enums in resource example that weren't defined in a table:(boolean,currency,dateTime,number,text) are in resource, but () are in table"
  ],
  "tocPath": "Resources/CalculatedColumn"
} -->

