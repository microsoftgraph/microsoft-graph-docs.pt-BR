---
title: Tipo de recurso ChartLegendFormat
description: Encapsula as propriedades de formato de uma legenda de gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: d3d7d9a0a74a56a6e0ae99aa7431779dc7164265
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531843"
---
# <a name="chartlegendformat-resource-type"></a>Tipo de recurso ChartLegendFormat

Namespace: microsoft.graph

Encapsula as propriedades de formato de uma legenda de gráfico.


## <a name="methods"></a>Métodos
Nenhum

## <a name="properties"></a>Propriedades
Nenhuma

## <a name="relationships"></a>Relacionamento
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|fill|[WorkbookChartFill](chartfill.md)|Representa o formato de preenchimento de um objeto, que inclui informações sobre a formatação da tela de fundo. Somente leitura.|
|fonte|[WorkbookChartFont](chartfont.md)|Representa os atributos de fonte, como nome da fonte, tamanho da fonte, cor, etc. de uma legenda do gráfico. Somente leitura.|


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartLegendFormat"
}-->

```json
{
  "fill": {"@odata.type": "microsoft.graph.workbookChartFill"},
  "font": {"@odata.type": "microsoft.graph.workbookChartFont"}
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartLegendFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
