---
title: Tipo de recurso ChartPoint
description: Representa um ponto de uma série do gráfico.
author: lumine2008
ms.openlocfilehash: b2d1fab0c76100aae1a5606690772a0aa3854f42
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27316223"
---
# <a name="chartpoint-resource-type"></a>Tipo de recurso ChartPoint

Representa um ponto de uma série do gráfico.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Get ChartPoint](../api/chartpoint-get.md) | [WorkbookChartPoint](chartpoint.md) |Leia as propriedades e os relacionamentos do objeto chartPoint.|
|[List](../api/chartpoint-list.md) | Coleção [WorkbookChartPoint](chartpoint.md) |Obtenha a coleção de objetos chartPoint. |
|[ItemAt](../api/chartpointscollection-itemat.md)|[WorkbookChartPoint](chartpoint.md)|Recupera um ponto com base na respectiva posição dentro da série.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|valor|Json|Retorna o valor de um ponto do gráfico. Somente leitura.|
|id|string|Identificador exclusivo|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|formato|[WorkbookChartPointFormat](chartpointformat.md)|Encapsula as propriedades de formato de um ponto do gráfico. Somente leitura.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartPoint"
}-->

```json
{
  "value": "string",
  "id": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartPoint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->