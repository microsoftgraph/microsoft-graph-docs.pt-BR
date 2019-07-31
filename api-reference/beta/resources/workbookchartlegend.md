---
title: tipo de recurso workbookChartLegend
description: Representa a legenda de um gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 42414f0089cf3e33529796ebbeb53b95bc1d4ef2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964016"
---
# <a name="workbookchartlegend-resource-type"></a>tipo de recurso workbookChartLegend

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa a legenda de um gráfico.

## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter workbookChartLegend](../api/chartlegend-get.md) | [workbookChartLegend](workbookchartlegend.md) |Leia as propriedades e os relacionamentos do objeto chartLegend.|
|[Update](../api/chartlegend-update.md) | [workbookChartLegend](workbookchartlegend.md) |Atualize o objeto ChartLegend. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|overlay|booliano|Valor booliano para determinar se a legenda do gráfico deve se sobrepor ao corpo principal do gráfico.|
|position|string|Representa a posição da legenda no gráfico. Os valores possíveis são: `Top`, `Bottom`, `Left`, `Right`, `Corner`, `Custom`.|
|visible|booliano|Um valor booliano que representa a visibilidade de um objeto ChartLegend.|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|formato|[workbookChartLegendFormat](workbookchartlegendformat.md)|Representa a formatação de uma legenda de gráfico, que inclui a formatação de fonte e de preenchimento. Somente leitura.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [
    "format"        
  ],
  "@odata.type": "microsoft.graph.workbookChartLegend"
}-->

```json
{
  "overlay": true,
  "position": "string",
  "visible": true,
  "format": {"@odata.type":"microsoft.graph.workbookChartLegendFormat"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ChartLegend resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
