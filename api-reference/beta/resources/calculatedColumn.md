---
author: JeremyKelley
description: calculatedColumn em um recurso columnDefinition indica que os dados da coluna são calculados com base em outras colunas do site.
ms.date: 09/11/2017
title: CalculatedColumn
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: e647d4d7cdc40929bb81a15ef851e978b411ce4b
ms.sourcegitcommit: e5d5095e26dca6f434354a0970e789e94ee6afb0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/22/2022
ms.locfileid: "63724126"
---
# <a name="calculatedcolumn-resource-type"></a>Tipo de recurso CalculatedColumn

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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

| Propriedade       | Tipo   | Descrição                                                                                                                  |
| :------------- | :----- | :--------------------------------------------------------------------------------------------------------------------------- |
| **format**     | string | Nos tipos de saída `dateTime`, o formato do valor. Deve ser `dateOnly` ou `dateTime`.                               |
| **formula**    | string | A fórmula usada para calcular o valor dessa coluna.                                                                       |
| **outputType** | string | O tipo de saída usado para formatar valores nessa coluna. Deve ser `boolean`, `currency`, `dateTime`, `number` ou `text`. |

As fórmulas do SharePoint usam uma sintaxe semelhante a fórmulas do Excel.
Consulte [Exemplos de fórmulas comuns em listas do SharePoint][SPFormulas] para obter mais informações.

[SPFormulas]: https://support.office.com/article/Examples-of-common-formulas-in-SharePoint-Lists-d81f5f21-2b4e-45ce-b170-bf7ebf6988b3

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/CalculatedColumn",
  "suppressions": []
}
-->
