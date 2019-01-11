---
title: Tipo de recurso ChartSeries
description: Representa uma série em um gráfico.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 6742c30eca55426e54290ae689bfabd8e14ce70f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27842626"
---
# <a name="chartseries-resource-type"></a>Tipo de recurso ChartSeries

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Representa uma série de um gráfico.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Get ChartSeries](../api/chartseries-get.md) | [ChartSeries](chartseries.md) |Leia as propriedades e os relacionamentos do objeto chartSeries.|
|[Create ChartPoints](../api/chartseries-post-points.md) |[ChartPoints](chartpoint.md)| Crie um novo ChartPoints postando na coleção de pontos.|
|[List points](../api/chartseries-list-points.md) |Coleção [ChartPoints](chartpoint.md)| Obtenha uma coleção de objetos ChartPoints.|
|[Update](../api/chartseries-update.md) | [ChartSeries](chartseries.md) |Atualize o objeto ChartSeries. |
|[List](../api/chartseries-list.md) | Coleção [ChartSeries](chartseries.md) |Obtenha uma coleção de objetos chartSeries. |
|[Itemat](../api/chartseriescollection-itemat.md)|[ChartSeries](chartseries.md)|Recupera uma série com base na respectiva posição na coleção.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|name|string|Representa o nome de uma série em um gráfico.|

## <a name="relationships"></a>Relacionamentos
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|formato|[ChartSeriesFormat](chartseriesformat.md)|Representa a formatação de uma série do gráfico, que inclui a formatação de linha e de preenchimento. Somente leitura.|
|points|Coleção [ChartPoints](chartpoint.md)|Representa uma coleção de todos os pontos da série. Somente leitura.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartSeries"
}-->

```json
{
  "name": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartSeries resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
