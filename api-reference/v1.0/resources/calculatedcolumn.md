---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: CalculatedColumn
ms.openlocfilehash: 44700ba7606243002798ec0ec84c3be30d38ef1f
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/28/2017
---
# <a name="calculatedcolumn-resource-type"></a>Tipo de recurso CalculatedColumn

**calculatedColumn** em um recurso [columnDefinition](columnDefinition.md) indica que os dados da coluna são calculados com base em outras colunas do site.

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
  "tocPath": "Resources/CalculatedColumn"
} -->
