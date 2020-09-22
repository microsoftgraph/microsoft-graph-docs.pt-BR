---
title: tipo de recurso workbookChartSeries
description: Representa uma série de um gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 22ce2138da7ae8163304978370ada1f71abe7026
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47979228"
---
# <a name="workbookchartseries-resource-type"></a>tipo de recurso workbookChartSeries

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma série de um gráfico.


## <a name="methods"></a>Methods

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Get ChartSeries](../api/chartseries-get.md) | [workbookChartSeries](workbookchartseries.md) |Leia as propriedades e os relacionamentos do objeto chartSeries.|
|[Criar ChartPoint](../api/chartseries-post-points.md) |[chartPoints](workbookchartpoint.md)| Crie um novo chartPoint postando na coleção Points.|
|[List points](../api/chartseries-list-points.md) |coleção [workbookChartPoints](workbookchartpoint.md)| Obtenha uma coleção de objetos chartPoints.|
|[Atualização](../api/chartseries-update.md) | [workbookChartSeries](workbookchartseries.md) |Atualize o objeto chartSeries. |
|[List](../api/chartseries-list.md) | coleção [workbookChartSeries](workbookchartseries.md) |Obtenha uma coleção de objetos chartSeries. |
|[ItemAt](../api/chartseriescollection-itemat.md)|[workbookChartSeries](workbookchartseries.md)|Recupera uma série com base na respectiva posição na coleção|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|nome|string|Representa o nome de uma série do gráfico.|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|formato|[workbookChartSeriesFormat](workbookchartseriesformat.md)|Representa a formatação de uma série do gráfico, que inclui a formatação de linha e de preenchimento. Somente leitura.|
|points|coleção [workbookChartPoint](workbookchartpoint.md)|Representa uma coleção de todos os pontos da série. Somente leitura.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookChartSeries"
}-->

```json
{
  "name": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ChartSeries resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


