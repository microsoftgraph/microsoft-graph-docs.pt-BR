---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: DefaultColumnValue
localization_priority: Normal
description: defaultColumnValue em um recurso columnDefinition especifica o valor padrão dessa coluna.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 4a2ddff8de7efb2bb697ffae63d69376588e6ac9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029509"
---
# <a name="defaultcolumnvalue-resource-type"></a>Tipo de recurso DefaultColumnValue

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
  "tocPath": "Resources/DefaultColumnValue"
} -->
