---
title: tipo de recurso workbookChartSeriesFormat
description: Abrange as propriedades de formatação da série do gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 2558d242e18fa8bf7d220ba5bc4dd8aef6cd2865
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519264"
---
# <a name="workbookchartseriesformat-resource-type"></a>tipo de recurso workbookChartSeriesFormat

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Encapsula as propriedades de formato da série do gráfico.


## <a name="methods"></a>Métodos
Nenhum

## <a name="properties"></a>Propriedades
Nenhuma

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|fill|[workbookChartFill](workbookchartfill.md)|Representa o formato de preenchimento de uma série do gráfico, que inclui informações sobre a formatação da tela de fundo. Somente leitura.|
|line|[workbookChartLineFormat](workbookchartlineformat.md)|Representa a formatação de linha. Somente leitura.|


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartSeriesFormat"
}-->

```json
{
  "fill": {"@odata.type": "microsoft.graph.workbookChartFill"},
  "line": {"@odata.type": "microsoft.graph.workbookChartLineFormat"}
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ChartSeriesFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
