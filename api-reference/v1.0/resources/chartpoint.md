---
title: Tipo de recurso ChartPoint
description: Representa o ponto de uma série do gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 870f29df417e401e2c69500f2677b9c5da95c88bb5dd57ede33aa26e125e0869
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54202536"
---
# <a name="chartpoint-resource-type"></a>Tipo de recurso ChartPoint

Namespace: microsoft.graph

Representa o ponto de uma série do gráfico.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Get ChartPoint](../api/chartpoint-get.md) | [WorkbookChartPoint](chartpoint.md) |Leia as propriedades e os relacionamentos do objeto chartPoint.|
|[List](../api/chartpoint-list.md) | [Coleção WorkbookChartPoint](chartpoint.md) |Obtenha a coleção de objetos chartPoint. |
|[ItemAt](../api/chartpointscollection-itemat.md)|[WorkbookChartPoint](chartpoint.md)|Recupera um ponto com base na respectiva posição dentro da série.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|valor|Json|Retorna o valor de um ponto do gráfico. Somente leitura.|
|id|string|identificador exclusivo|

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

