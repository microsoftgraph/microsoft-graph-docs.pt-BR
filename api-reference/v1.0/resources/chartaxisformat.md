---
title: Tipo de recurso ChartAxisFormat
description: Encapsula as propriedades de formato do eixo do gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 1d52063e63e179540bcbd5c3b4ec0cd09fb620d7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029852"
---
# <a name="chartaxisformat-resource-type"></a>Tipo de recurso ChartAxisFormat

Encapsula as propriedades de formato do eixo do gráfico.


## <a name="methods"></a>Métodos
Nenhum
## <a name="properties"></a>Propriedades
Nenhuma

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|font|[WorkbookChartFont](chartfont.md)|Representa os atributos de fonte de um elemento do eixo do gráfico, como nome, tamanho, cor, etc. Somente leitura.|
|line|[WorkbookChartLineFormat](chartlineformat.md)|Representa a formatação de linha do gráfico. Somente leitura.|


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartAxisFormat"
}-->

```json
{
  "font": {"@odata.type": "microsoft.graph.workbookChartFont"},
  "line": {"@odata.type": "microsoft.graph.workbookChartLineFormat"}
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartAxisFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
