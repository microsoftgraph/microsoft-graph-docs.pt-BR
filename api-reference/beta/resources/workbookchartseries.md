---
title: tipo de recurso workbookChartSeries
description: Representa uma série de um gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: e9ff478a5f7e91c3d116ca2dbd78e20699077aab
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348501"
---
# <a name="workbookchartseries-resource-type"></a>tipo de recurso workbookChartSeries

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma série de um gráfico.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Get ChartSeries](../api/chartseries-get.md) | [workbookChartSeries](workbookchartseries.md) |Leia as propriedades e os relacionamentos do objeto chartSeries.|
|[Criar ChartPoint](../api/chartseries-post-points.md) |[chartPoints](workbookchartpoint.md)| Crie um novo chartPoint postando na coleção Points.|
|[List points](../api/chartseries-list-points.md) |coleção [workbookChartPoints](workbookchartpoint.md)| Obtenha uma coleção de objetos chartPoints.|
|[Update](../api/chartseries-update.md) | [workbookChartSeries](workbookchartseries.md) |Atualize o objeto chartSeries. |
|[Lista](../api/chartseries-list.md) | coleção [workbookChartSeries](workbookchartseries.md) |Obtenha uma coleção de objetos chartSeries. |
|[ItemAt](../api/chartseriescollection-itemat.md)|[workbookChartSeries](workbookchartseries.md)|Recupera uma série com base na respectiva posição na coleção|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|name|string|Representa o nome de uma série do gráfico.|

## <a name="relationships"></a>Relacionamento
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
