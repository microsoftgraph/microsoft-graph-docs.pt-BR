---
title: tipo de recurso workbookChartPoint
description: Representa o ponto de uma série do gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: db0037e91f1ee9279a131c5a318c4425e7878aed
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007253"
---
# <a name="workbookchartpoint-resource-type"></a>tipo de recurso workbookChartPoint

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o ponto de uma série do gráfico.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter workbookChartPoint](../api/chartpoint-get.md) | [workbookChartPoint](workbookchartpoint.md) |Leia as propriedades e os relacionamentos do objeto chartPoint.|
|[List](../api/chartpoint-list.md) | coleção [workbookChartPoint](workbookchartpoint.md) |Obtenha a coleção de objetos chartPoint. |
|[ItemAt](../api/chartpointscollection-itemat.md)|[workbookChartPoint](workbookchartpoint.md)|Recupera um ponto com base na respectiva posição dentro da série.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|valor|Json|Retorna o valor de um ponto do gráfico. Somente leitura.|
|id|string|identificador exclusivo|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|formato|[workbookChartPointFormat](workbookchartpointformat.md)|Encapsula as propriedades de formato de um ponto do gráfico. Somente leitura.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "format"
    ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartPoint"
}-->

```json
{
  "value": "string",
  "id": "string",
  "format": {"@odata.type": "microsoft.graph.workbookChartPointFormat"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ChartPoint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
