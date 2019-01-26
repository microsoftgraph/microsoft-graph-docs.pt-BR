---
title: Tipo de recurso ChartSeries
description: Representa uma série em um gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: eccd0d970ffeff7b41ceb0f9af810bb7a420d663
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29570656"
---
# <a name="chartseries-resource-type"></a>Tipo de recurso ChartSeries

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma série em um gráfico.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Get ChartSeries](../api/chartseries-get.md) | [workbookChartSeries](chartseries.md) |Leia as propriedades e os relacionamentos do objeto chartSeries.|
|[Create ChartPoints](../api/chartseries-post-points.md) |[chartPoints](chartpoint.md)| Crie um novo ChartPoints postando na coleção de pontos.|
|[List points](../api/chartseries-list-points.md) |coleção [chartPoints](chartpoint.md)| Obtenha uma coleção de objetos ChartPoints.|
|[Update](../api/chartseries-update.md) | [workbookChartSeries](chartseries.md) |Atualize o objeto ChartSeries. |
|[List](../api/chartseries-list.md) | coleção [workbookChartSeries](chartseries.md) |Obtenha uma coleção de objetos chartSeries. |
|[ItemAt](../api/chartseriescollection-itemat.md)|[workbookChartSeries](chartseries.md)|Recupera uma série com base na respectiva posição na coleção.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|name|string|Representa o nome de uma série em um gráfico.|

## <a name="relationships"></a>Relacionamentos
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|formato|[workbookChartSeriesFormat](chartseriesformat.md)|Representa a formatação de uma série do gráfico, que inclui a formatação de linha e de preenchimento. Somente leitura.|
|points|coleção [workbookChartPoint](chartpoint.md)|Representa uma coleção de todos os pontos da série. Somente leitura.|

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
  "suppressions": [
    "Error: /api-reference/beta/resources/chartseries.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
