---
title: Tipo de recurso Chart
description: Representa um objeto chart em uma pasta de trabalho.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: a6f11cad32e48b259f3754ed08e4bad769f9a4c6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531922"
---
# <a name="chart-resource-type"></a><span data-ttu-id="40acb-103">Tipo de recurso Chart</span><span class="sxs-lookup"><span data-stu-id="40acb-103">Chart resource type</span></span>

<span data-ttu-id="40acb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="40acb-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="40acb-105">Representa um objeto chart em uma pasta de trabalho.</span><span class="sxs-lookup"><span data-stu-id="40acb-105">Represents a chart object in a workbook.</span></span>


## <a name="methods"></a><span data-ttu-id="40acb-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="40acb-106">Methods</span></span>

| <span data-ttu-id="40acb-107">Método</span><span class="sxs-lookup"><span data-stu-id="40acb-107">Method</span></span>           | <span data-ttu-id="40acb-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="40acb-108">Return Type</span></span>    |<span data-ttu-id="40acb-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="40acb-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="40acb-110">Get Chart</span><span class="sxs-lookup"><span data-stu-id="40acb-110">Get Chart</span></span>](../api/chart-get.md) | [<span data-ttu-id="40acb-111">WorkbookChart</span><span class="sxs-lookup"><span data-stu-id="40acb-111">WorkbookChart</span></span>](chart.md) |<span data-ttu-id="40acb-112">Leia as propriedades e os relacionamentos do objeto de gráfico.</span><span class="sxs-lookup"><span data-stu-id="40acb-112">Read properties and relationships of chart object.</span></span>|
|[<span data-ttu-id="40acb-113">Create ChartSeries</span><span class="sxs-lookup"><span data-stu-id="40acb-113">Create ChartSeries</span></span>](../api/chart-post-series.md) |[<span data-ttu-id="40acb-114">WorkbookChartSeries</span><span class="sxs-lookup"><span data-stu-id="40acb-114">WorkbookChartSeries</span></span>](chartseries.md)| <span data-ttu-id="40acb-115">Crie uma nova ChartSeries postando na coleção de séries.</span><span class="sxs-lookup"><span data-stu-id="40acb-115">Create a new ChartSeries by posting to the series collection.</span></span>|
|[<span data-ttu-id="40acb-116">List series</span><span class="sxs-lookup"><span data-stu-id="40acb-116">List series</span></span>](../api/chart-list-series.md) |<span data-ttu-id="40acb-117">Coleção [WorkbookChartSeries](chartseries.md)</span><span class="sxs-lookup"><span data-stu-id="40acb-117">[WorkbookChartSeries](chartseries.md) collection</span></span>| <span data-ttu-id="40acb-118">Obtenha uma coleção de objetos ChartSeries.</span><span class="sxs-lookup"><span data-stu-id="40acb-118">Get a ChartSeries object collection.</span></span>|
|[<span data-ttu-id="40acb-119">Update</span><span class="sxs-lookup"><span data-stu-id="40acb-119">Update</span></span>](../api/chart-update.md) | [<span data-ttu-id="40acb-120">WorkbookChart</span><span class="sxs-lookup"><span data-stu-id="40acb-120">WorkbookChart</span></span>](chart.md)   |<span data-ttu-id="40acb-121">Atualize um objeto Chart.</span><span class="sxs-lookup"><span data-stu-id="40acb-121">Update Chart object.</span></span> |
|[<span data-ttu-id="40acb-122">Image</span><span class="sxs-lookup"><span data-stu-id="40acb-122">Image</span></span>](../api/chart-image.md)|<span data-ttu-id="40acb-123">Cadeia de caracteres de imagem codificada em base64</span><span class="sxs-lookup"><span data-stu-id="40acb-123">Image base64 encoded string</span></span>|<span data-ttu-id="40acb-124">Processa o gráfico como uma imagem codificada em base64, dimensionando o gráfico para se ajustar às dimensões especificadas.</span><span class="sxs-lookup"><span data-stu-id="40acb-124">Renders the chart as a base64-encoded image by scaling the chart to fit the specified dimensions.</span></span>|
|[<span data-ttu-id="40acb-125">Excluir</span><span class="sxs-lookup"><span data-stu-id="40acb-125">Delete</span></span>](../api/chart-delete.md)|<span data-ttu-id="40acb-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="40acb-126">None</span></span>|<span data-ttu-id="40acb-127">Exclui o objeto de gráfico.</span><span class="sxs-lookup"><span data-stu-id="40acb-127">Deletes the chart object.</span></span>|
|[<span data-ttu-id="40acb-128">SetData</span><span class="sxs-lookup"><span data-stu-id="40acb-128">Setdata</span></span>](../api/chart-setdata.md)|<span data-ttu-id="40acb-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="40acb-129">None</span></span>|<span data-ttu-id="40acb-130">Redefine os dados de origem do gráfico.</span><span class="sxs-lookup"><span data-stu-id="40acb-130">Resets the source data for the chart.</span></span>|
|[<span data-ttu-id="40acb-131">Setposition</span><span class="sxs-lookup"><span data-stu-id="40acb-131">Setposition</span></span>](../api/chart-setposition.md)|<span data-ttu-id="40acb-132">Nenhum</span><span class="sxs-lookup"><span data-stu-id="40acb-132">None</span></span>|<span data-ttu-id="40acb-133">Posiciona o gráfico em relação às células na planilha.</span><span class="sxs-lookup"><span data-stu-id="40acb-133">Positions the chart relative to cells on the worksheet.</span></span>|
|[<span data-ttu-id="40acb-134">List</span><span class="sxs-lookup"><span data-stu-id="40acb-134">List</span></span>](../api/chart-list.md) | <span data-ttu-id="40acb-135">Conjunto [WorkbookChart](chart.md) </span><span class="sxs-lookup"><span data-stu-id="40acb-135">[WorkbookChart](chart.md) collection</span></span> |<span data-ttu-id="40acb-136">Obtenha a coleção de objetos do gráfico.</span><span class="sxs-lookup"><span data-stu-id="40acb-136">Get chart object collection.</span></span> |
|[<span data-ttu-id="40acb-137">Itemat</span><span class="sxs-lookup"><span data-stu-id="40acb-137">Itemat</span></span>](../api/chartcollection-itemat.md)|[<span data-ttu-id="40acb-138">WorkbookChart</span><span class="sxs-lookup"><span data-stu-id="40acb-138">WorkbookChart</span></span>](chart.md)|<span data-ttu-id="40acb-139">Obtém um gráfico com base em sua posição na coleção.</span><span class="sxs-lookup"><span data-stu-id="40acb-139">Gets a chart based on its position in the collection.</span></span>|
|[<span data-ttu-id="40acb-140">Add</span><span class="sxs-lookup"><span data-stu-id="40acb-140">Add</span></span>](../api/chartcollection-add.md)|[<span data-ttu-id="40acb-141">WorkbookChart</span><span class="sxs-lookup"><span data-stu-id="40acb-141">WorkbookChart</span></span>](chart.md)|<span data-ttu-id="40acb-142">Cria um novo gráfico.</span><span class="sxs-lookup"><span data-stu-id="40acb-142">Creates a new chart.</span></span>|

## <a name="properties"></a><span data-ttu-id="40acb-143">Propriedades</span><span class="sxs-lookup"><span data-stu-id="40acb-143">Properties</span></span>
| <span data-ttu-id="40acb-144">Propriedade</span><span class="sxs-lookup"><span data-stu-id="40acb-144">Property</span></span>     | <span data-ttu-id="40acb-145">Tipo</span><span class="sxs-lookup"><span data-stu-id="40acb-145">Type</span></span>   |<span data-ttu-id="40acb-146">Descrição</span><span class="sxs-lookup"><span data-stu-id="40acb-146">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="40acb-147">height</span><span class="sxs-lookup"><span data-stu-id="40acb-147">height</span></span>|<span data-ttu-id="40acb-148">double</span><span class="sxs-lookup"><span data-stu-id="40acb-148">double</span></span>|<span data-ttu-id="40acb-149">Representa a altura, em pontos, do objeto Chart.</span><span class="sxs-lookup"><span data-stu-id="40acb-149">Represents the height, in points, of the chart object.</span></span>|
|<span data-ttu-id="40acb-150">id</span><span class="sxs-lookup"><span data-stu-id="40acb-150">id</span></span>|<span data-ttu-id="40acb-151">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="40acb-151">string</span></span>|<span data-ttu-id="40acb-p101">Obtém um gráfico com base em sua posição no conjunto. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="40acb-p101">Gets a chart based on its position in the collection. Read-only.</span></span>|
|<span data-ttu-id="40acb-154">left</span><span class="sxs-lookup"><span data-stu-id="40acb-154">left</span></span>|<span data-ttu-id="40acb-155">double</span><span class="sxs-lookup"><span data-stu-id="40acb-155">double</span></span>|<span data-ttu-id="40acb-156">A distância, em pontos, da esquerda do gráfico à origem da planilha.</span><span class="sxs-lookup"><span data-stu-id="40acb-156">The distance, in points, from the left side of the chart to the worksheet origin.</span></span>|
|<span data-ttu-id="40acb-157">nome</span><span class="sxs-lookup"><span data-stu-id="40acb-157">name</span></span>|<span data-ttu-id="40acb-158">string</span><span class="sxs-lookup"><span data-stu-id="40acb-158">string</span></span>|<span data-ttu-id="40acb-159">Representa o nome de um objeto Chart.</span><span class="sxs-lookup"><span data-stu-id="40acb-159">Represents the name of a chart object.</span></span>|
|<span data-ttu-id="40acb-160">top</span><span class="sxs-lookup"><span data-stu-id="40acb-160">top</span></span>|<span data-ttu-id="40acb-161">duplo</span><span class="sxs-lookup"><span data-stu-id="40acb-161">double</span></span>|<span data-ttu-id="40acb-162">Representa a distância, em pontos, da borda superior do objeto à parte superior da primeira linha de uma planilha ou da área de um gráfico.</span><span class="sxs-lookup"><span data-stu-id="40acb-162">Represents the distance, in points, from the top edge of the object to the top of row 1 (on a worksheet) or the top of the chart area (on a chart).</span></span>|
|<span data-ttu-id="40acb-163">width</span><span class="sxs-lookup"><span data-stu-id="40acb-163">width</span></span>|<span data-ttu-id="40acb-164">Double</span><span class="sxs-lookup"><span data-stu-id="40acb-164">double</span></span>|<span data-ttu-id="40acb-165">Representa a largura, em pontos, do objeto de gráfico.</span><span class="sxs-lookup"><span data-stu-id="40acb-165">Represents the width, in points, of the chart object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="40acb-166">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="40acb-166">Relationships</span></span>
| <span data-ttu-id="40acb-167">Relação</span><span class="sxs-lookup"><span data-stu-id="40acb-167">Relationship</span></span> | <span data-ttu-id="40acb-168">Tipo</span><span class="sxs-lookup"><span data-stu-id="40acb-168">Type</span></span>   |<span data-ttu-id="40acb-169">Descrição</span><span class="sxs-lookup"><span data-stu-id="40acb-169">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="40acb-170">axes</span><span class="sxs-lookup"><span data-stu-id="40acb-170">axes</span></span>|[<span data-ttu-id="40acb-171">WorkbookChartAxes</span><span class="sxs-lookup"><span data-stu-id="40acb-171">WorkbookChartAxes</span></span>](chartaxes.md)|<span data-ttu-id="40acb-p102">Representa os eixos de um gráfico. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="40acb-p102">Represents chart axes. Read-only.</span></span>|
|<span data-ttu-id="40acb-174">dataLabels</span><span class="sxs-lookup"><span data-stu-id="40acb-174">dataLabels</span></span>|[<span data-ttu-id="40acb-175">WorkbookChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="40acb-175">WorkbookChartDataLabels</span></span>](chartdatalabels.md)|<span data-ttu-id="40acb-p103">Representa os rótulos de dados no gráfico. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="40acb-p103">Represents the datalabels on the chart. Read-only.</span></span>|
|<span data-ttu-id="40acb-178">format</span><span class="sxs-lookup"><span data-stu-id="40acb-178">format</span></span>|[<span data-ttu-id="40acb-179">WorkbookChartAreaFormat</span><span class="sxs-lookup"><span data-stu-id="40acb-179">WorkbookChartAreaFormat</span></span>](chartareaformat.md)|<span data-ttu-id="40acb-p104">Encapsula as propriedades de formato da área do gráfico. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="40acb-p104">Encapsulates the format properties for the chart area. Read-only.</span></span>|
|<span data-ttu-id="40acb-182">legend</span><span class="sxs-lookup"><span data-stu-id="40acb-182">legend</span></span>|[<span data-ttu-id="40acb-183">WorkbookChartLegend</span><span class="sxs-lookup"><span data-stu-id="40acb-183">WorkbookChartLegend</span></span>](chartlegend.md)|<span data-ttu-id="40acb-p105">Representa a legenda do gráfico. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="40acb-p105">Represents the legend for the chart. Read-only.</span></span>|
|<span data-ttu-id="40acb-186">series</span><span class="sxs-lookup"><span data-stu-id="40acb-186">series</span></span>|<span data-ttu-id="40acb-187">Coleção [WorkbookChartSeries](chartseries.md)</span><span class="sxs-lookup"><span data-stu-id="40acb-187">[WorkbookChartSeries](chartseries.md) collection</span></span>|<span data-ttu-id="40acb-p106">Representa uma única série ou uma coleção de séries no gráfico. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="40acb-p106">Represents either a single series or collection of series in the chart. Read-only.</span></span>|
|<span data-ttu-id="40acb-190">title</span><span class="sxs-lookup"><span data-stu-id="40acb-190">title</span></span>|[<span data-ttu-id="40acb-191">WorkbookChartTitle</span><span class="sxs-lookup"><span data-stu-id="40acb-191">WorkbookChartTitle</span></span>](charttitle.md)|<span data-ttu-id="40acb-p107">Representa o título do gráfico especificado, incluindo o texto, a visibilidade, a posição e a formatação. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="40acb-p107">Represents the title of the specified chart, including the text, visibility, position and formating of the title. Read-only.</span></span>|
|<span data-ttu-id="40acb-194">planilha</span><span class="sxs-lookup"><span data-stu-id="40acb-194">worksheet</span></span>|[<span data-ttu-id="40acb-195">WorkbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="40acb-195">WorkbookWorksheet</span></span>](worksheet.md)|<span data-ttu-id="40acb-196">A planilha que contém o gráfico atual.</span><span class="sxs-lookup"><span data-stu-id="40acb-196">The worksheet containing the current chart.</span></span> <span data-ttu-id="40acb-197">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="40acb-197">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="40acb-198">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="40acb-198">JSON representation</span></span>

<span data-ttu-id="40acb-199">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="40acb-199">Here is a JSON representation of the resource.</span></span>

<!--{
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
<!-- {
  "type": "#page.annotation",
  "description": "Chart resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
