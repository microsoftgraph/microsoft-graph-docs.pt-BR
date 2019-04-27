---
title: tipo de recurso workbookChart
description: Representa um objeto chart em uma pasta de trabalho.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 55d5278c08a63e853383e3f80ff015e97afcb9b6
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348460"
---
# <a name="workbookchart-resource-type"></a>tipo de recurso workbookChart

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um objeto chart em uma pasta de trabalho.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Get Chart](../api/chart-get.md) | [workbookChart](workbookchart.md) |Leia as propriedades e os relacionamentos do objeto de gráfico.|
|[Create ChartSeries](../api/chart-post-series.md) |[workbookChartSeries](workbookchartseries.md)| Crie uma nova ChartSeries postando na coleção de séries.|
|[List series](../api/chart-list-series.md) |coleção [workbookChartSeries](workbookchartseries.md)| Obtenha uma coleção de objetos ChartSeries.|
|[Update](../api/chart-update.md) | [workbookChart](workbookchart.md)   |Atualize um objeto Chart. |
|[Image](../api/chart-image.md)|Cadeia de caracteres de imagem codificada em base64|Processa o gráfico como uma imagem codificada em base64, dimensionando o gráfico para se ajustar às dimensões especificadas.|
|[Delete](../api/chart-delete.md)|Nenhum|Exclui o objeto de gráfico.|
|[SetData](../api/chart-setdata.md)|Nenhum|Redefine os dados de origem do gráfico.|
|[Setposition](../api/chart-setposition.md)|Nenhum|Posiciona o gráfico em relação às células na planilha.|
|[List](../api/chart-list.md) | coleção [workbookChart](workbookchart.md) |Obtenha a coleção de objetos do gráfico. |
|[Itemat](../api/chartcollection-itemat.md)|[workbookChart](workbookchart.md)|Obtém um gráfico com base em sua posição na coleção.|
|[Add](../api/chartcollection-add.md)|[workbookChart](workbookchart.md)|Cria um novo gráfico.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|height|double|Representa a altura, em pontos, do objeto Chart.|
|id|cadeia de caracteres|Obtém um gráfico com base em sua posição no conjunto. Somente leitura.|
|left|double|A distância, em pontos, da esquerda do gráfico à origem da planilha.|
|name|string|Representa o nome de um objeto Chart.|
|top|duplo|Representa a distância, em pontos, da borda superior do objeto à parte superior da primeira linha de uma planilha ou da área de um gráfico.|
|width|Double|Representa a largura, em pontos, do objeto de gráfico.|

## <a name="relationships"></a>Relacionamento
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|axes|[workbookChartAxes](workbookchartaxes.md)|Representa os eixos de um gráfico. Somente leitura.|
|dataLabels|[workbookChartDataLabels](workbookchartdatalabels.md)|Representa os rótulos de dados no gráfico. Somente leitura.|
|format|[workbookChartAreaFormat](workbookchartareaformat.md)|Encapsula as propriedades de formato da área do gráfico. Somente leitura.|
|legend|[workbookChartLegend](workbookchartlegend.md)|Representa a legenda do gráfico. Somente leitura.|
|series|coleção [workbookChartSeries](workbookchartseries.md)|Representa uma única série ou uma coleção de séries no gráfico. Somente leitura.|
|title|[workbookChartTitle](workbookcharttitle.md)|Representa o título do gráfico especificado, incluindo o texto, a visibilidade, a posição e a formatação. Somente leitura.|
|planilha|[workbookWorksheet](workbookworksheet.md)|A planilha que contém o gráfico atual. Somente leitura.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChart"
}-->

```json
{
  "height": 1024,
  "id": "string",
  "left": 1024,
  "name": "string",
  "top": 1024,
  "width": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "workbookChart resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
