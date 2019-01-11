---
title: Tipo de recurso Chart
description: Representa um objeto de gráfico em uma pasta de trabalho.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 4f412894ffaef07908a41f8f7cc15ab3a52331af
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27873399"
---
# <a name="chart-resource-type"></a><span data-ttu-id="e997e-103">Tipo de recurso Chart</span><span class="sxs-lookup"><span data-stu-id="e997e-103">Chart resource type</span></span>

<span data-ttu-id="e997e-104">Representa um objeto de gráfico em uma pasta de trabalho.</span><span class="sxs-lookup"><span data-stu-id="e997e-104">Represents a chart object in a workbook.</span></span>


## <a name="methods"></a><span data-ttu-id="e997e-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="e997e-105">Methods</span></span>

| <span data-ttu-id="e997e-106">Método</span><span class="sxs-lookup"><span data-stu-id="e997e-106">Method</span></span>           | <span data-ttu-id="e997e-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e997e-107">Return Type</span></span>    |<span data-ttu-id="e997e-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="e997e-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e997e-109">Get Chart</span><span class="sxs-lookup"><span data-stu-id="e997e-109">Get Chart</span></span>](../api/chart-get.md) | [<span data-ttu-id="e997e-110">WorkbookChart</span><span class="sxs-lookup"><span data-stu-id="e997e-110">WorkbookChart</span></span>](chart.md) |<span data-ttu-id="e997e-111">Leia as propriedades e os relacionamentos do objeto de gráfico.</span><span class="sxs-lookup"><span data-stu-id="e997e-111">Read properties and relationships of chart object.</span></span>|
|[<span data-ttu-id="e997e-112">Create ChartSeries</span><span class="sxs-lookup"><span data-stu-id="e997e-112">Create ChartSeries</span></span>](../api/chart-post-series.md) |[<span data-ttu-id="e997e-113">WorkbookChartSeries</span><span class="sxs-lookup"><span data-stu-id="e997e-113">WorkbookChartSeries</span></span>](chartseries.md)| <span data-ttu-id="e997e-114">Crie uma nova ChartSeries postando na coleção de séries.</span><span class="sxs-lookup"><span data-stu-id="e997e-114">Create a new ChartSeries by posting to the series collection.</span></span>|
|[<span data-ttu-id="e997e-115">List series</span><span class="sxs-lookup"><span data-stu-id="e997e-115">List series</span></span>](../api/chart-list-series.md) |<span data-ttu-id="e997e-116">Coleção [WorkbookChartSeries](chartseries.md)</span><span class="sxs-lookup"><span data-stu-id="e997e-116">[WorkbookChartSeries](chartseries.md) collection</span></span>| <span data-ttu-id="e997e-117">Obtenha uma coleção de objetos ChartSeries.</span><span class="sxs-lookup"><span data-stu-id="e997e-117">Get a ChartSeries object collection.</span></span>|
|[<span data-ttu-id="e997e-118">Update</span><span class="sxs-lookup"><span data-stu-id="e997e-118">Update</span></span>](../api/chart-update.md) | [<span data-ttu-id="e997e-119">WorkbookChart</span><span class="sxs-lookup"><span data-stu-id="e997e-119">WorkbookChart</span></span>](chart.md)   |<span data-ttu-id="e997e-120">Atualize um objeto Chart.</span><span class="sxs-lookup"><span data-stu-id="e997e-120">Update Chart object.</span></span> |
|[<span data-ttu-id="e997e-121">Image</span><span class="sxs-lookup"><span data-stu-id="e997e-121">Image</span></span>](../api/chart-image.md)|<span data-ttu-id="e997e-122">Cadeia de caracteres de imagem codificada em base64</span><span class="sxs-lookup"><span data-stu-id="e997e-122">Image base64 encoded string</span></span>|<span data-ttu-id="e997e-123">Processa o gráfico como uma imagem codificada em base64, dimensionando o gráfico para se ajustar às dimensões especificadas.</span><span class="sxs-lookup"><span data-stu-id="e997e-123">Renders the chart as a base64-encoded image by scaling the chart to fit the specified dimensions.</span></span>|
|[<span data-ttu-id="e997e-124">Delete</span><span class="sxs-lookup"><span data-stu-id="e997e-124">Delete</span></span>](../api/chart-delete.md)|<span data-ttu-id="e997e-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e997e-125">None</span></span>|<span data-ttu-id="e997e-126">Exclui o objeto de gráfico.</span><span class="sxs-lookup"><span data-stu-id="e997e-126">Deletes the chart object.</span></span>|
|[<span data-ttu-id="e997e-127">SetData</span><span class="sxs-lookup"><span data-stu-id="e997e-127">Setdata</span></span>](../api/chart-setdata.md)|<span data-ttu-id="e997e-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e997e-128">None</span></span>|<span data-ttu-id="e997e-129">Redefine os dados de origem do gráfico.</span><span class="sxs-lookup"><span data-stu-id="e997e-129">Resets the source data for the chart.</span></span>|
|[<span data-ttu-id="e997e-130">Setposition</span><span class="sxs-lookup"><span data-stu-id="e997e-130">Setposition</span></span>](../api/chart-setposition.md)|<span data-ttu-id="e997e-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e997e-131">None</span></span>|<span data-ttu-id="e997e-132">Posiciona o gráfico em relação às células na planilha.</span><span class="sxs-lookup"><span data-stu-id="e997e-132">Positions the chart relative to cells on the worksheet.</span></span>|
|[<span data-ttu-id="e997e-133">List</span><span class="sxs-lookup"><span data-stu-id="e997e-133">List</span></span>](../api/chart-list.md) | <span data-ttu-id="e997e-134">Coleção [WorkbookChart](chart.md)</span><span class="sxs-lookup"><span data-stu-id="e997e-134">[WorkbookChart](chart.md) collection</span></span> |<span data-ttu-id="e997e-135">Obtenha a coleção de objetos do gráfico.</span><span class="sxs-lookup"><span data-stu-id="e997e-135">Get chart object collection.</span></span> |
|[<span data-ttu-id="e997e-136">Itemat</span><span class="sxs-lookup"><span data-stu-id="e997e-136">Itemat</span></span>](../api/chartcollection-itemat.md)|[<span data-ttu-id="e997e-137">WorkbookChart</span><span class="sxs-lookup"><span data-stu-id="e997e-137">WorkbookChart</span></span>](chart.md)|<span data-ttu-id="e997e-138">Obtém um gráfico com base em sua posição na coleção.</span><span class="sxs-lookup"><span data-stu-id="e997e-138">Gets a chart based on its position in the collection.</span></span>|
|[<span data-ttu-id="e997e-139">Add</span><span class="sxs-lookup"><span data-stu-id="e997e-139">Add</span></span>](../api/chartcollection-add.md)|[<span data-ttu-id="e997e-140">WorkbookChart</span><span class="sxs-lookup"><span data-stu-id="e997e-140">WorkbookChart</span></span>](chart.md)|<span data-ttu-id="e997e-141">Cria um novo gráfico.</span><span class="sxs-lookup"><span data-stu-id="e997e-141">Creates a new chart.</span></span>|

## <a name="properties"></a><span data-ttu-id="e997e-142">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e997e-142">Properties</span></span>
| <span data-ttu-id="e997e-143">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e997e-143">Property</span></span>     | <span data-ttu-id="e997e-144">Tipo</span><span class="sxs-lookup"><span data-stu-id="e997e-144">Type</span></span>   |<span data-ttu-id="e997e-145">Descrição</span><span class="sxs-lookup"><span data-stu-id="e997e-145">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e997e-146">height</span><span class="sxs-lookup"><span data-stu-id="e997e-146">height</span></span>|<span data-ttu-id="e997e-147">Double</span><span class="sxs-lookup"><span data-stu-id="e997e-147">double</span></span>|<span data-ttu-id="e997e-148">Representa a altura, em pontos, do objeto Chart.</span><span class="sxs-lookup"><span data-stu-id="e997e-148">Represents the height, in points, of the chart object.</span></span>|
|<span data-ttu-id="e997e-149">id</span><span class="sxs-lookup"><span data-stu-id="e997e-149">id</span></span>|<span data-ttu-id="e997e-150">string</span><span class="sxs-lookup"><span data-stu-id="e997e-150">string</span></span>|<span data-ttu-id="e997e-p101">Obtém um gráfico com base em sua posição no conjunto. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e997e-p101">Gets a chart based on its position in the collection. Read-only.</span></span>|
|<span data-ttu-id="e997e-153">left</span><span class="sxs-lookup"><span data-stu-id="e997e-153">left</span></span>|<span data-ttu-id="e997e-154">Double</span><span class="sxs-lookup"><span data-stu-id="e997e-154">double</span></span>|<span data-ttu-id="e997e-155">A distância, em pontos, da esquerda do gráfico à origem da planilha.</span><span class="sxs-lookup"><span data-stu-id="e997e-155">The distance, in points, from the left side of the chart to the worksheet origin.</span></span>|
|<span data-ttu-id="e997e-156">name</span><span class="sxs-lookup"><span data-stu-id="e997e-156">name</span></span>|<span data-ttu-id="e997e-157">string</span><span class="sxs-lookup"><span data-stu-id="e997e-157">string</span></span>|<span data-ttu-id="e997e-158">Representa o nome de um objeto Chart.</span><span class="sxs-lookup"><span data-stu-id="e997e-158">Represents the name of a chart object.</span></span>|
|<span data-ttu-id="e997e-159">top</span><span class="sxs-lookup"><span data-stu-id="e997e-159">top</span></span>|<span data-ttu-id="e997e-160">Double</span><span class="sxs-lookup"><span data-stu-id="e997e-160">double</span></span>|<span data-ttu-id="e997e-161">Representa a distância, em pontos, da borda superior do objeto à parte superior da primeira linha de uma planilha ou da área de um gráfico.</span><span class="sxs-lookup"><span data-stu-id="e997e-161">Represents the distance, in points, from the top edge of the object to the top of row 1 (on a worksheet) or the top of the chart area (on a chart).</span></span>|
|<span data-ttu-id="e997e-162">width</span><span class="sxs-lookup"><span data-stu-id="e997e-162">width</span></span>|<span data-ttu-id="e997e-163">Double</span><span class="sxs-lookup"><span data-stu-id="e997e-163">double</span></span>|<span data-ttu-id="e997e-164">Representa a largura, em pontos, do objeto de gráfico.</span><span class="sxs-lookup"><span data-stu-id="e997e-164">Represents the width, in points, of the chart object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e997e-165">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="e997e-165">Relationships</span></span>
| <span data-ttu-id="e997e-166">Relação</span><span class="sxs-lookup"><span data-stu-id="e997e-166">Relationship</span></span> | <span data-ttu-id="e997e-167">Tipo</span><span class="sxs-lookup"><span data-stu-id="e997e-167">Type</span></span>   |<span data-ttu-id="e997e-168">Descrição</span><span class="sxs-lookup"><span data-stu-id="e997e-168">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e997e-169">axes</span><span class="sxs-lookup"><span data-stu-id="e997e-169">axes</span></span>|[<span data-ttu-id="e997e-170">WorkbookChartAxes</span><span class="sxs-lookup"><span data-stu-id="e997e-170">WorkbookChartAxes</span></span>](chartaxes.md)|<span data-ttu-id="e997e-p102">Representa os eixos de um gráfico. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e997e-p102">Represents chart axes. Read-only.</span></span>|
|<span data-ttu-id="e997e-173">dataLabels</span><span class="sxs-lookup"><span data-stu-id="e997e-173">dataLabels</span></span>|[<span data-ttu-id="e997e-174">WorkbookChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="e997e-174">WorkbookChartDataLabels</span></span>](chartdatalabels.md)|<span data-ttu-id="e997e-p103">Representa os rótulos de dados no gráfico. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e997e-p103">Represents the datalabels on the chart. Read-only.</span></span>|
|<span data-ttu-id="e997e-177">formato</span><span class="sxs-lookup"><span data-stu-id="e997e-177">format</span></span>|[<span data-ttu-id="e997e-178">WorkbookChartAreaFormat</span><span class="sxs-lookup"><span data-stu-id="e997e-178">WorkbookChartAreaFormat</span></span>](chartareaformat.md)|<span data-ttu-id="e997e-p104">Encapsula as propriedades de formato da área do gráfico. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e997e-p104">Encapsulates the format properties for the chart area. Read-only.</span></span>|
|<span data-ttu-id="e997e-181">legend</span><span class="sxs-lookup"><span data-stu-id="e997e-181">legend</span></span>|[<span data-ttu-id="e997e-182">WorkbookChartLegend</span><span class="sxs-lookup"><span data-stu-id="e997e-182">WorkbookChartLegend</span></span>](chartlegend.md)|<span data-ttu-id="e997e-p105">Representa a legenda do gráfico. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e997e-p105">Represents the legend for the chart. Read-only.</span></span>|
|<span data-ttu-id="e997e-185">series</span><span class="sxs-lookup"><span data-stu-id="e997e-185">series</span></span>|<span data-ttu-id="e997e-186">Coleção [WorkbookChartSeries](chartseries.md)</span><span class="sxs-lookup"><span data-stu-id="e997e-186">[WorkbookChartSeries](chartseries.md) collection</span></span>|<span data-ttu-id="e997e-p106">Representa uma única série ou uma coleção de séries no gráfico. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e997e-p106">Represents either a single series or collection of series in the chart. Read-only.</span></span>|
|<span data-ttu-id="e997e-189">título</span><span class="sxs-lookup"><span data-stu-id="e997e-189">title</span></span>|[<span data-ttu-id="e997e-190">WorkbookChartTitle</span><span class="sxs-lookup"><span data-stu-id="e997e-190">WorkbookChartTitle</span></span>](charttitle.md)|<span data-ttu-id="e997e-p107">Representa o título do gráfico especificado, incluindo o texto, a visibilidade, a posição e a formatação. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e997e-p107">Represents the title of the specified chart, including the text, visibility, position and formating of the title. Read-only.</span></span>|
|<span data-ttu-id="e997e-193">planilha</span><span class="sxs-lookup"><span data-stu-id="e997e-193">worksheet</span></span>|[<span data-ttu-id="e997e-194">WorkbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="e997e-194">WorkbookWorksheet</span></span>](worksheet.md)|<span data-ttu-id="e997e-p108">A planilha que contém o gráfico atual. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e997e-p108">The worksheet containing the current chart. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e997e-197">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e997e-197">JSON representation</span></span>

<span data-ttu-id="e997e-198">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e997e-198">Here is a JSON representation of the resource.</span></span>

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
