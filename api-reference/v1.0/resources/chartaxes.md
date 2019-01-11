---
title: Tipo de recurso ChartAxes
description: Representa os eixos de um gráfico.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 53f0e4a7344ddfab89330203f90032266e0c622d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27885901"
---
# <a name="chartaxes-resource-type"></a>Tipo de recurso ChartAxes

Representa os eixos de um gráfico.


## <a name="methods"></a>Métodos
Nenhum

## <a name="properties"></a>Propriedades
Nenhum

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|categoryAxis|[WorkbookChartAxis](chartaxis.md)|Representa o eixo de categoria em um gráfico. Somente leitura.|
|seriesAxis|[WorkbookChartAxis](chartaxis.md)|Representa o eixo das séries de um gráfico 3D. Somente leitura.|
|valueAxis|[WorkbookChartAxis](chartaxis.md)|Representa o eixo dos valores em um eixo. Somente leitura.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartAxes"
}-->

```json
{
  "categoryAxis": {"@odata.type": "microsoft.graph.workbookChartAxis"},
  "seriesAxis": {"@odata.type": "microsoft.graph.workbookChartAxis"},
  "valueAxis": {"@odata.type": "microsoft.graph.workbookChartAxis"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartAxes resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
