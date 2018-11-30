---
title: Tipo de recurso Chart
description: Representa um objeto de gráfico em uma pasta de trabalho.
ms.openlocfilehash: bada94032dcc00e3f6294b20559f44044570f2ec
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27004950"
---
# <a name="chart-resource-type"></a><span data-ttu-id="5b5bd-103">Tipo de recurso Chart</span><span class="sxs-lookup"><span data-stu-id="5b5bd-103">Chart resource type</span></span>

<span data-ttu-id="5b5bd-104">Representa um objeto de gráfico em uma pasta de trabalho.</span><span class="sxs-lookup"><span data-stu-id="5b5bd-104">Represents a chart object in a workbook.</span></span>


## <a name="methods"></a><span data-ttu-id="5b5bd-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="5b5bd-105">Methods</span></span>

| <span data-ttu-id="5b5bd-106">Método</span><span class="sxs-lookup"><span data-stu-id="5b5bd-106">Method</span></span>           | <span data-ttu-id="5b5bd-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="5b5bd-107">Return Type</span></span>    |<span data-ttu-id="5b5bd-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="5b5bd-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5b5bd-109">Get Chart</span><span class="sxs-lookup"><span data-stu-id="5b5bd-109">Get Chart</span></span>](../api/chart-get.md) | [<span data-ttu-id="5b5bd-110">WorkbookChart</span><span class="sxs-lookup"><span data-stu-id="5b5bd-110">WorkbookChart</span></span>](chart.md) |<span data-ttu-id="5b5bd-111">Leia as propriedades e os relacionamentos do objeto de gráfico.</span><span class="sxs-lookup"><span data-stu-id="5b5bd-111">Read properties and relationships of chart object.</span></span>|
|[<span data-ttu-id="5b5bd-112">Create ChartSeries</span><span class="sxs-lookup"><span data-stu-id="5b5bd-112">Create ChartSeries</span></span>](../api/chart-post-series.md) |[<span data-ttu-id="5b5bd-113">WorkbookChartSeries</span><span class="sxs-lookup"><span data-stu-id="5b5bd-113">WorkbookChartSeries</span></span>](chartseries.md)| <span data-ttu-id="5b5bd-114">Crie uma nova ChartSeries postando na coleção de séries.</span><span class="sxs-lookup"><span data-stu-id="5b5bd-114">Create a new ChartSeries by posting to the series collection.</span></span>|
|[<span data-ttu-id="5b5bd-115">List series</span><span class="sxs-lookup"><span data-stu-id="5b5bd-115">List series</span></span>](../api/chart-list-series.md) |<span data-ttu-id="5b5bd-116">Coleção [WorkbookChartSeries](chartseries.md)</span><span class="sxs-lookup"><span data-stu-id="5b5bd-116">[WorkbookChartSeries](chartseries.md) collection</span></span>| <span data-ttu-id="5b5bd-117">Obtenha uma coleção de objetos ChartSeries.</span><span class="sxs-lookup"><span data-stu-id="5b5bd-117">Get a ChartSeries object collection.</span></span>|
|[<span data-ttu-id="5b5bd-118">Update</span><span class="sxs-lookup"><span data-stu-id="5b5bd-118">Update</span></span>](../api/chart-update.md) | [<span data-ttu-id="5b5bd-119">WorkbookChart</span><span class="sxs-lookup"><span data-stu-id="5b5bd-119">WorkbookChart</span></span>](chart.md)   |<span data-ttu-id="5b5bd-120">Atualize um objeto Chart.</span><span class="sxs-lookup"><span data-stu-id="5b5bd-120">Update Chart object.</span></span> |
|[<span data-ttu-id="5b5bd-121">Imagem</span><span class="sxs-lookup"><span data-stu-id="5b5bd-121">Image</span></span>](../api/chart-image.md)|<span data-ttu-id="5b5bd-122">Cadeia de caracteres de imagem codificada em base64</span><span class="sxs-lookup"><span data-stu-id="5b5bd-122">Image base64 encoded string</span></span>|<span data-ttu-id="5b5bd-123">Processa o gráfico como uma imagem codificada em base64, dimensionando o gráfico para se ajustar às dimensões especificadas.</span><span class="sxs-lookup"><span data-stu-id="5b5bd-123">Renders the chart as a base64-encoded image by scaling the chart to fit the specified dimensions.</span></span>|
|[<span data-ttu-id="5b5bd-124">Delete</span><span class="sxs-lookup"><span data-stu-id="5b5bd-124">Delete</span></span>](../api/chart-delete.md)|<span data-ttu-id="5b5bd-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5b5bd-125">None</span></span>|<span data-ttu-id="5b5bd-126">Exclui o objeto de gráfico.</span><span class="sxs-lookup"><span data-stu-id="5b5bd-126">Deletes the chart object.</span></span>|
|[<span data-ttu-id="5b5bd-127">SetData</span><span class="sxs-lookup"><span data-stu-id="5b5bd-127">Setdata</span></span>](../api/chart-setdata.md)|<span data-ttu-id="5b5bd-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5b5bd-128">None</span></span>|<span data-ttu-id="5b5bd-129">Redefine os dados de origem do gráfico.</span><span class="sxs-lookup"><span data-stu-id="5b5bd-129">Resets the source data for the chart.</span></span>|
|[<span data-ttu-id="5b5bd-130">Setposition</span><span class="sxs-lookup"><span data-stu-id="5b5bd-130">Setposition</span></span>](../api/chart-setposition.md)|<span data-ttu-id="5b5bd-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5b5bd-131">None</span></span>|<span data-ttu-id="5b5bd-132">Posiciona o gráfico em relação às células na planilha.</span><span class="sxs-lookup"><span data-stu-id="5b5bd-132">Positions the chart relative to cells on the worksheet.</span></span>|
|[<span data-ttu-id="5b5bd-133">List</span><span class="sxs-lookup"><span data-stu-id="5b5bd-133">List</span></span>](../api/chart-list.md) | <span data-ttu-id="5b5bd-134">Coleção [WorkbookChart](chart.md)</span><span class="sxs-lookup"><span data-stu-id="5b5bd-134">[WorkbookChart](chart.md) collection</span></span> |<span data-ttu-id="5b5bd-135">Obtenha a coleção de objetos do gráfico.</span><span class="sxs-lookup"><span data-stu-id="5b5bd-135">Get chart object collection.</span></span> |
|[<span data-ttu-id="5b5bd-136">Itemat</span><span class="sxs-lookup"><span data-stu-id="5b5bd-136">Itemat</span></span>](../api/chartcollection-itemat.md)|[<span data-ttu-id="5b5bd-137">WorkbookChart</span><span class="sxs-lookup"><span data-stu-id="5b5bd-137">WorkbookChart</span></span>](chart.md)|<span data-ttu-id="5b5bd-138">Obtém um gráfico com base em sua posição na coleção.</span><span class="sxs-lookup"><span data-stu-id="5b5bd-138">Gets a chart based on its position in the collection.</span></span>|
|[<span data-ttu-id="5b5bd-139">Add</span><span class="sxs-lookup"><span data-stu-id="5b5bd-139">Add</span></span>](../api/chartcollection-add.md)|[<span data-ttu-id="5b5bd-140">WorkbookChart</span><span class="sxs-lookup"><span data-stu-id="5b5bd-140">WorkbookChart</span></span>](chart.md)|<span data-ttu-id="5b5bd-141">Cria um novo gráfico.</span><span class="sxs-lookup"><span data-stu-id="5b5bd-141">Creates a new chart.</span></span>|

## <a name="properties"></a><span data-ttu-id="5b5bd-142">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5b5bd-142">Properties</span></span>
| <span data-ttu-id="5b5bd-143">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5b5bd-143">Property</span></span>     | <span data-ttu-id="5b5bd-144">Tipo</span><span class="sxs-lookup"><span data-stu-id="5b5bd-144">Type</span></span>   |<span data-ttu-id="5b5bd-145">Descrição</span><span class="sxs-lookup"><span data-stu-id="5b5bd-145">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5b5bd-146">height</span><span class="sxs-lookup"><span data-stu-id="5b5bd-146">height</span></span>|<span data-ttu-id="5b5bd-147">Double</span><span class="sxs-lookup"><span data-stu-id="5b5bd-147">double</span></span>|<span data-ttu-id="5b5bd-148">Representa a altura, em pontos, do objeto Chart.</span><span class="sxs-lookup"><span data-stu-id="5b5bd-148">Represents the height, in points, of the chart object.</span></span>|
|<span data-ttu-id="5b5bd-149">id</span><span class="sxs-lookup"><span data-stu-id="5b5bd-149">id</span></span>|<span data-ttu-id="5b5bd-150">string</span><span class="sxs-lookup"><span data-stu-id="5b5bd-150">string</span></span>|<span data-ttu-id="5b5bd-p101">Obtém um gráfico com base em sua posição no conjunto. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5b5bd-p101">Gets a chart based on its position in the collection. Read-only.</span></span>|
|<span data-ttu-id="5b5bd-153">left</span><span class="sxs-lookup"><span data-stu-id="5b5bd-153">left</span></span>|<span data-ttu-id="5b5bd-154">Double</span><span class="sxs-lookup"><span data-stu-id="5b5bd-154">double</span></span>|<span data-ttu-id="5b5bd-155">A distância, em pontos, da esquerda do gráfico à origem da planilha.</span><span class="sxs-lookup"><span data-stu-id="5b5bd-155">The distance, in points, from the left side of the chart to the worksheet origin.</span></span>|
|<span data-ttu-id="5b5bd-156">name</span><span class="sxs-lookup"><span data-stu-id="5b5bd-156">name</span></span>|<span data-ttu-id="5b5bd-157">string</span><span class="sxs-lookup"><span data-stu-id="5b5bd-157">string</span></span>|<span data-ttu-id="5b5bd-158">Representa o nome de um objeto Chart.</span><span class="sxs-lookup"><span data-stu-id="5b5bd-158">Represents the name of a chart object.</span></span>|
|<span data-ttu-id="5b5bd-159">top</span><span class="sxs-lookup"><span data-stu-id="5b5bd-159">top</span></span>|<span data-ttu-id="5b5bd-160">Double</span><span class="sxs-lookup"><span data-stu-id="5b5bd-160">double</span></span>|<span data-ttu-id="5b5bd-161">Representa a distância, em pontos, da borda superior do objeto à parte superior da primeira linha de uma planilha ou da área de um gráfico.</span><span class="sxs-lookup"><span data-stu-id="5b5bd-161">Represents the distance, in points, from the top edge of the object to the top of row 1 (on a worksheet) or the top of the chart area (on a chart).</span></span>|
|<span data-ttu-id="5b5bd-162">width</span><span class="sxs-lookup"><span data-stu-id="5b5bd-162">width</span></span>|<span data-ttu-id="5b5bd-163">Double</span><span class="sxs-lookup"><span data-stu-id="5b5bd-163">double</span></span>|<span data-ttu-id="5b5bd-164">Representa a largura, em pontos, do objeto de gráfico.</span><span class="sxs-lookup"><span data-stu-id="5b5bd-164">Represents the width, in points, of the chart object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5b5bd-165">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="5b5bd-165">Relationships</span></span>
| <span data-ttu-id="5b5bd-166">Relação</span><span class="sxs-lookup"><span data-stu-id="5b5bd-166">Relationship</span></span> | <span data-ttu-id="5b5bd-167">Tipo</span><span class="sxs-lookup"><span data-stu-id="5b5bd-167">Type</span></span>   |<span data-ttu-id="5b5bd-168">Descrição</span><span class="sxs-lookup"><span data-stu-id="5b5bd-168">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5b5bd-169">axes</span><span class="sxs-lookup"><span data-stu-id="5b5bd-169">axes</span></span>|[<span data-ttu-id="5b5bd-170">WorkbookChartAxes</span><span class="sxs-lookup"><span data-stu-id="5b5bd-170">WorkbookChartAxes</span></span>](chartaxes.md)|<span data-ttu-id="5b5bd-p102">Representa os eixos de um gráfico. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5b5bd-p102">Represents chart axes. Read-only.</span></span>|
|<span data-ttu-id="5b5bd-173">dataLabels</span><span class="sxs-lookup"><span data-stu-id="5b5bd-173">dataLabels</span></span>|[<span data-ttu-id="5b5bd-174">WorkbookChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="5b5bd-174">WorkbookChartDataLabels</span></span>](chartdatalabels.md)|<span data-ttu-id="5b5bd-p103">Representa os rótulos de dados no gráfico. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5b5bd-p103">Represents the datalabels on the chart. Read-only.</span></span>|
|<span data-ttu-id="5b5bd-177">formato</span><span class="sxs-lookup"><span data-stu-id="5b5bd-177">format</span></span>|[<span data-ttu-id="5b5bd-178">WorkbookChartAreaFormat</span><span class="sxs-lookup"><span data-stu-id="5b5bd-178">WorkbookChartAreaFormat</span></span>](chartareaformat.md)|<span data-ttu-id="5b5bd-p104">Encapsula as propriedades de formato da área do gráfico. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5b5bd-p104">Encapsulates the format properties for the chart area. Read-only.</span></span>|
|<span data-ttu-id="5b5bd-181">legend</span><span class="sxs-lookup"><span data-stu-id="5b5bd-181">legend</span></span>|[<span data-ttu-id="5b5bd-182">WorkbookChartLegend</span><span class="sxs-lookup"><span data-stu-id="5b5bd-182">WorkbookChartLegend</span></span>](chartlegend.md)|<span data-ttu-id="5b5bd-p105">Representa a legenda do gráfico. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5b5bd-p105">Represents the legend for the chart. Read-only.</span></span>|
|<span data-ttu-id="5b5bd-185">series</span><span class="sxs-lookup"><span data-stu-id="5b5bd-185">series</span></span>|<span data-ttu-id="5b5bd-186">Coleção [WorkbookChartSeries](chartseries.md)</span><span class="sxs-lookup"><span data-stu-id="5b5bd-186">[WorkbookChartSeries](chartseries.md) collection</span></span>|<span data-ttu-id="5b5bd-p106">Representa uma única série ou uma coleção de séries no gráfico. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5b5bd-p106">Represents either a single series or collection of series in the chart. Read-only.</span></span>|
|<span data-ttu-id="5b5bd-189">title</span><span class="sxs-lookup"><span data-stu-id="5b5bd-189">title</span></span>|[<span data-ttu-id="5b5bd-190">WorkbookChartTitle</span><span class="sxs-lookup"><span data-stu-id="5b5bd-190">WorkbookChartTitle</span></span>](charttitle.md)|<span data-ttu-id="5b5bd-p107">Representa o título do gráfico especificado, incluindo o texto, a visibilidade, a posição e a formatação. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5b5bd-p107">Represents the title of the specified chart, including the text, visibility, position and formating of the title. Read-only.</span></span>|
|<span data-ttu-id="5b5bd-193">planilha</span><span class="sxs-lookup"><span data-stu-id="5b5bd-193">worksheet</span></span>|[<span data-ttu-id="5b5bd-194">WorkbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="5b5bd-194">WorkbookWorksheet</span></span>](worksheet.md)|<span data-ttu-id="5b5bd-p108">A planilha que contém o gráfico atual. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5b5bd-p108">The worksheet containing the current chart. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5b5bd-197">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5b5bd-197">JSON representation</span></span>

<span data-ttu-id="5b5bd-198">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5b5bd-198">Here is a JSON representation of the resource.</span></span>

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