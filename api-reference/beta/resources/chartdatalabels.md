---
title: Tipo de recurso ChartDataLabels
description: Representa uma coleção de todos os rótulos de dados em um ponto do gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: bda2c1849f154435608f311671026e224b0c7e3c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543721"
---
# <a name="chartdatalabels-resource-type"></a>Tipo de recurso ChartDataLabels

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma coleção de todos os rótulos de dados em um ponto do gráfico.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Get ChartDataLabels](../api/chartdatalabels-get.md) | [ChartDataLabels](chartdatalabels.md) |Leia as propriedades e os relacionamentos do objeto chartDataLabels.|
|[Update](../api/chartdatalabels-update.md) | [ChartDataLabels](chartdatalabels.md) |Atualize o objeto ChartDataLabels. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|position|cadeia de caracteres|Valor de DataLabelPosition que representa a posição do rótulo de dados. Os valores possíveis são: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit` e `Callout`.|
|separador|string|Cadeia de caracteres que representa o separador usado para os rótulos de dados em um gráfico.|
|showBubbleSize|booliano|Valor booliano que determina se o tamanho da bolha do rótulo de dados fica visível ou não.|
|showCategoryName|booliano|Valor booliano que determina se o nome da categoria do rótulo de dados fica visível ou não.|
|showLegendKey|booliano|Valor booliano que determina se o código de legenda do rótulo de dados fica visível ou não.|
|showPercentage|booliano|Valor booliano que determina se o percentual do rótulo de dados fica visível ou não.|
|showSeriesName|booliano|Valor booliano que determina se o nome da série do rótulo de dados fica visível ou não.|
|showValue|booliano|Valor booliano que determina se o valor do rótulo de dados fica visível ou não.|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|format|[ChartDataLabelFormat](chartdatalabelformat.md)|Representa o formato dos rótulos de dados do gráfico, que inclui a formatação de fonte e de preenchimento. Somente leitura.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartDataLabels"
}-->

```json
{
  "position": "string",
  "separator": "string",
  "showBubbleSize": true,
  "showCategoryName": true,
  "showLegendKey": true,
  "showPercentage": true,
  "showSeriesName": true,
  "showValue": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ChartDataLabels resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chartdatalabels.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
