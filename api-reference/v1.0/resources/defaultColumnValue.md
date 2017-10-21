---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: DefaultColumnValue
ms.openlocfilehash: 73761e224a59b3a9a4206d5e1cfb058294b7f53b
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/28/2017
---
# <a name="defaultcolumnvalue-resource-type"></a>Tipo de recurso DefaultColumnValue

**defaultColumnValue** em um recurso [columnDefinition](columnDefinition.md) especifica o valor padrão dessa coluna.
O valor padrão pode ser especificado tanto diretamente ou como uma fórmula.

## <a name="json-representation"></a>Representação JSON

Aqui está uma representação JSON de um recurso **defaultColumnValue**.
<!-- { "blockType": "resource", "@type": "microsoft.graph.defaultColumnValue" } -->

```json
{
  "formula": "=[Column1]+[Column2]+[Column3]",
  "value": "defaultValueString"
}
```

## <a name="properties"></a>Propriedades

| Nome da propriedade | Tipo   | Descrição
|:--------------|:-------|:----------------------------------------------------
| **formula**   | string | A fórmula usada para calcular o valor padrão dessa coluna.
| **value**     | string | O valor direto para usar como o valor padrão dessa coluna.

Somente uma **fórmula** ou um **valor** pode ser especificado por vez.

As fórmulas do SharePoint usam uma sintaxe semelhante a fórmulas do Excel.
Consulte [Exemplos de fórmulas comuns em listas do SharePoint][SPFormulas] para obter mais informações.

[SPFormulas]: https://support.office.com/en-us/article/Examples-of-common-formulas-in-SharePoint-Lists-d81f5f21-2b4e-45ce-b170-bf7ebf6988b3


<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/DefaultColumnValue"
} -->
