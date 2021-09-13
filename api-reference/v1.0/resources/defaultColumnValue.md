---
author: daspek
ms.date: 09/12/2017
title: DefaultColumnValue
ms.localizationpriority: medium
description: defaultColumnValue em um recurso columnDefinition especifica o valor padrão dessa coluna.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 93ba93e33359f17aaad8f5cc9f814f0b67758e3e
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59029056"
---
# <a name="defaultcolumnvalue-resource-type"></a>Tipo de recurso DefaultColumnValue

Namespace: microsoft.graph

**defaultColumnValue** em um recurso [columnDefinition](columndefinition.md) especifica o valor padrão dessa coluna.
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
  "tocPath&quot;: &quot;Resources/DefaultColumnValue"
} -->

