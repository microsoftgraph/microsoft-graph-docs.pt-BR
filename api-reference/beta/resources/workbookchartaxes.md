---
title: tipo de recurso workbookChartAxes
description: Representa os eixos de um gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 89d9a45f0f9e992ac8a93cde6114fc8c9f073359
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519383"
---
# <a name="workbookchartaxes-resource-type"></a>tipo de recurso workbookChartAxes

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os eixos de um gráfico.


## <a name="methods"></a>Métodos
Nenhum

## <a name="properties"></a>Propriedades
Nenhuma

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|categoryAxis|[workbookChartAxis](workbookchartaxis.md)|Representa o eixo de categoria em um gráfico. Somente leitura.|
|seriesAxis|[workbookChartAxis](workbookchartaxis.md)|Representa o eixo das séries de um gráfico 3D. Somente leitura.|
|valueAxis|[workbookChartAxis](workbookchartaxis.md)|Representa o eixo dos valores em um eixo. Somente leitura.|

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
<!--
{
  "type": "#page.annotation",
  "description": "ChartAxes resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
