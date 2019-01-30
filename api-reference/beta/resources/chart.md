---
title: Tipo de recurso Chart
description: Representa um objeto de gráfico em uma pasta de trabalho.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 4bc0ad0d31981e7e84241519e92569ab25c2cf18
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643231"
---
# <a name="chart-resource-type"></a><span data-ttu-id="f54eb-103">Tipo de recurso Chart</span><span class="sxs-lookup"><span data-stu-id="f54eb-103">Chart resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f54eb-104">Representa um objeto de gráfico em uma pasta de trabalho.</span><span class="sxs-lookup"><span data-stu-id="f54eb-104">Represents a chart object in a workbook.</span></span>


## <a name="methods"></a><span data-ttu-id="f54eb-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="f54eb-105">Methods</span></span>

| <span data-ttu-id="f54eb-106">Método</span><span class="sxs-lookup"><span data-stu-id="f54eb-106">Method</span></span>           | <span data-ttu-id="f54eb-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f54eb-107">Return Type</span></span>    |<span data-ttu-id="f54eb-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="f54eb-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f54eb-109">Get Chart</span><span class="sxs-lookup"><span data-stu-id="f54eb-109">Get Chart</span></span>](../api/chart-get.md) | [<span data-ttu-id="f54eb-110">Chart</span><span class="sxs-lookup"><span data-stu-id="f54eb-110">Chart</span></span>](chart.md) |<span data-ttu-id="f54eb-111">Leia as propriedades e os relacionamentos do objeto de gráfico.</span><span class="sxs-lookup"><span data-stu-id="f54eb-111">Read properties and relationships of chart object.</span></span>|
|[<span data-ttu-id="f54eb-112">Create ChartSeries</span><span class="sxs-lookup"><span data-stu-id="f54eb-112">Create ChartSeries</span></span>](../api/chart-post-series.md) |[<span data-ttu-id="f54eb-113">ChartSeries</span><span class="sxs-lookup"><span data-stu-id="f54eb-113">ChartSeries</span></span>](chartseries.md)| <span data-ttu-id="f54eb-114">Crie uma nova ChartSeries postando na coleção de séries.</span><span class="sxs-lookup"><span data-stu-id="f54eb-114">Create a new ChartSeries by posting to the series collection.</span></span>|
|[<span data-ttu-id="f54eb-115">List series</span><span class="sxs-lookup"><span data-stu-id="f54eb-115">List series</span></span>](../api/chart-list-series.md) |<span data-ttu-id="f54eb-116">Coleção [ChartSeries](chartseries.md)</span><span class="sxs-lookup"><span data-stu-id="f54eb-116">[ChartSeries](chartseries.md) collection</span></span>| <span data-ttu-id="f54eb-117">Obtenha uma coleção de objetos ChartSeries.</span><span class="sxs-lookup"><span data-stu-id="f54eb-117">Get a ChartSeries object collection.</span></span>|
|[<span data-ttu-id="f54eb-118">Update</span><span class="sxs-lookup"><span data-stu-id="f54eb-118">Update</span></span>](../api/chart-update.md) | [<span data-ttu-id="f54eb-119">Chart</span><span class="sxs-lookup"><span data-stu-id="f54eb-119">Chart</span></span>](chart.md)   |<span data-ttu-id="f54eb-120">Atualize um objeto Chart.</span><span class="sxs-lookup"><span data-stu-id="f54eb-120">Update Chart object.</span></span> |
|[<span data-ttu-id="f54eb-121">Image</span><span class="sxs-lookup"><span data-stu-id="f54eb-121">Image</span></span>](../api/chart-image.md)|<span data-ttu-id="f54eb-122">Cadeia de caracteres de imagem codificada em base64</span><span class="sxs-lookup"><span data-stu-id="f54eb-122">Image base64 encoded string</span></span>|<span data-ttu-id="f54eb-123">Processa o gráfico como uma imagem codificada em base64, dimensionando o gráfico para se ajustar às dimensões especificadas.</span><span class="sxs-lookup"><span data-stu-id="f54eb-123">Renders the chart as a base64-encoded image by scaling the chart to fit the specified dimensions.</span></span>|
|[<span data-ttu-id="f54eb-124">Delete</span><span class="sxs-lookup"><span data-stu-id="f54eb-124">Delete</span></span>](../api/chart-delete.md)|<span data-ttu-id="f54eb-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f54eb-125">None</span></span>|<span data-ttu-id="f54eb-126">Exclui o objeto de gráfico.</span><span class="sxs-lookup"><span data-stu-id="f54eb-126">Deletes the chart object.</span></span>|
|[<span data-ttu-id="f54eb-127">SetData</span><span class="sxs-lookup"><span data-stu-id="f54eb-127">Setdata</span></span>](../api/chart-setdata.md)|<span data-ttu-id="f54eb-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f54eb-128">None</span></span>|<span data-ttu-id="f54eb-129">Redefine os dados de origem do gráfico.</span><span class="sxs-lookup"><span data-stu-id="f54eb-129">Resets the source data for the chart.</span></span>|
|[<span data-ttu-id="f54eb-130">Setposition</span><span class="sxs-lookup"><span data-stu-id="f54eb-130">Setposition</span></span>](../api/chart-setposition.md)|<span data-ttu-id="f54eb-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f54eb-131">None</span></span>|<span data-ttu-id="f54eb-132">Posiciona o gráfico em relação às células na planilha.</span><span class="sxs-lookup"><span data-stu-id="f54eb-132">Positions the chart relative to cells on the worksheet.</span></span>|
|[<span data-ttu-id="f54eb-133">List</span><span class="sxs-lookup"><span data-stu-id="f54eb-133">List</span></span>](../api/chart-list.md) | <span data-ttu-id="f54eb-134">Coleção [Chart](chart.md)</span><span class="sxs-lookup"><span data-stu-id="f54eb-134">[Chart](chart.md) collection</span></span> |<span data-ttu-id="f54eb-135">Obtenha a coleção de objetos do gráfico.</span><span class="sxs-lookup"><span data-stu-id="f54eb-135">Get chart object collection.</span></span> |
|[<span data-ttu-id="f54eb-136">Itemat</span><span class="sxs-lookup"><span data-stu-id="f54eb-136">Itemat</span></span>](../api/chartcollection-itemat.md)|[<span data-ttu-id="f54eb-137">Chart</span><span class="sxs-lookup"><span data-stu-id="f54eb-137">Chart</span></span>](chart.md)|<span data-ttu-id="f54eb-138">Obtém um gráfico com base em sua posição na coleção.</span><span class="sxs-lookup"><span data-stu-id="f54eb-138">Gets a chart based on its position in the collection.</span></span>|
|[<span data-ttu-id="f54eb-139">Add</span><span class="sxs-lookup"><span data-stu-id="f54eb-139">Add</span></span>](../api/chartcollection-add.md)|[<span data-ttu-id="f54eb-140">Chart</span><span class="sxs-lookup"><span data-stu-id="f54eb-140">Chart</span></span>](chart.md)|<span data-ttu-id="f54eb-141">Cria um novo gráfico.</span><span class="sxs-lookup"><span data-stu-id="f54eb-141">Creates a new chart.</span></span>|

## <a name="properties"></a><span data-ttu-id="f54eb-142">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f54eb-142">Properties</span></span>
| <span data-ttu-id="f54eb-143">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f54eb-143">Property</span></span>     | <span data-ttu-id="f54eb-144">Tipo</span><span class="sxs-lookup"><span data-stu-id="f54eb-144">Type</span></span>   |<span data-ttu-id="f54eb-145">Descrição</span><span class="sxs-lookup"><span data-stu-id="f54eb-145">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f54eb-146">height</span><span class="sxs-lookup"><span data-stu-id="f54eb-146">height</span></span>|<span data-ttu-id="f54eb-147">Double</span><span class="sxs-lookup"><span data-stu-id="f54eb-147">double</span></span>|<span data-ttu-id="f54eb-148">Representa a altura, em pontos, do objeto Chart.</span><span class="sxs-lookup"><span data-stu-id="f54eb-148">Represents the height, in points, of the chart object.</span></span>|
|<span data-ttu-id="f54eb-149">id</span><span class="sxs-lookup"><span data-stu-id="f54eb-149">id</span></span>|<span data-ttu-id="f54eb-150">string</span><span class="sxs-lookup"><span data-stu-id="f54eb-150">string</span></span>|<span data-ttu-id="f54eb-p101">Obtém um gráfico com base em sua posição no conjunto. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f54eb-p101">Gets a chart based on its position in the collection. Read-only.</span></span>|
|<span data-ttu-id="f54eb-153">left</span><span class="sxs-lookup"><span data-stu-id="f54eb-153">left</span></span>|<span data-ttu-id="f54eb-154">Double</span><span class="sxs-lookup"><span data-stu-id="f54eb-154">double</span></span>|<span data-ttu-id="f54eb-155">A distância, em pontos, da esquerda do gráfico à origem da planilha.</span><span class="sxs-lookup"><span data-stu-id="f54eb-155">The distance, in points, from the left side of the chart to the worksheet origin.</span></span>|
|<span data-ttu-id="f54eb-156">name</span><span class="sxs-lookup"><span data-stu-id="f54eb-156">name</span></span>|<span data-ttu-id="f54eb-157">string</span><span class="sxs-lookup"><span data-stu-id="f54eb-157">string</span></span>|<span data-ttu-id="f54eb-158">Representa o nome de um objeto Chart.</span><span class="sxs-lookup"><span data-stu-id="f54eb-158">Represents the name of a chart object.</span></span>|
|<span data-ttu-id="f54eb-159">top</span><span class="sxs-lookup"><span data-stu-id="f54eb-159">top</span></span>|<span data-ttu-id="f54eb-160">Double</span><span class="sxs-lookup"><span data-stu-id="f54eb-160">double</span></span>|<span data-ttu-id="f54eb-161">Representa a distância, em pontos, da borda superior do objeto à parte superior da primeira linha de uma planilha ou da área de um gráfico.</span><span class="sxs-lookup"><span data-stu-id="f54eb-161">Represents the distance, in points, from the top edge of the object to the top of row 1 (on a worksheet) or the top of the chart area (on a chart).</span></span>|
|<span data-ttu-id="f54eb-162">width</span><span class="sxs-lookup"><span data-stu-id="f54eb-162">width</span></span>|<span data-ttu-id="f54eb-163">Double</span><span class="sxs-lookup"><span data-stu-id="f54eb-163">double</span></span>|<span data-ttu-id="f54eb-164">Representa a largura, em pontos, do objeto de gráfico.</span><span class="sxs-lookup"><span data-stu-id="f54eb-164">Represents the width, in points, of the chart object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f54eb-165">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="f54eb-165">Relationships</span></span>
| <span data-ttu-id="f54eb-166">Relação</span><span class="sxs-lookup"><span data-stu-id="f54eb-166">Relationship</span></span> | <span data-ttu-id="f54eb-167">Tipo</span><span class="sxs-lookup"><span data-stu-id="f54eb-167">Type</span></span>   |<span data-ttu-id="f54eb-168">Descrição</span><span class="sxs-lookup"><span data-stu-id="f54eb-168">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f54eb-169">axes</span><span class="sxs-lookup"><span data-stu-id="f54eb-169">axes</span></span>|[<span data-ttu-id="f54eb-170">ChartAxes</span><span class="sxs-lookup"><span data-stu-id="f54eb-170">ChartAxes</span></span>](chartaxes.md)|<span data-ttu-id="f54eb-p102">Representa os eixos de um gráfico. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f54eb-p102">Represents chart axes. Read-only.</span></span>|
|<span data-ttu-id="f54eb-173">dataLabels</span><span class="sxs-lookup"><span data-stu-id="f54eb-173">dataLabels</span></span>|[<span data-ttu-id="f54eb-174">ChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="f54eb-174">ChartDataLabels</span></span>](chartdatalabels.md)|<span data-ttu-id="f54eb-p103">Representa os rótulos de dados no gráfico. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f54eb-p103">Represents the datalabels on the chart. Read-only.</span></span>|
|<span data-ttu-id="f54eb-177">formato</span><span class="sxs-lookup"><span data-stu-id="f54eb-177">format</span></span>|[<span data-ttu-id="f54eb-178">ChartAreaFormat</span><span class="sxs-lookup"><span data-stu-id="f54eb-178">ChartAreaFormat</span></span>](chartareaformat.md)|<span data-ttu-id="f54eb-p104">Encapsula as propriedades de formato da área do gráfico. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f54eb-p104">Encapsulates the format properties for the chart area. Read-only.</span></span>|
|<span data-ttu-id="f54eb-181">legend</span><span class="sxs-lookup"><span data-stu-id="f54eb-181">legend</span></span>|[<span data-ttu-id="f54eb-182">ChartLegend</span><span class="sxs-lookup"><span data-stu-id="f54eb-182">ChartLegend</span></span>](chartlegend.md)|<span data-ttu-id="f54eb-p105">Representa a legenda do gráfico. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f54eb-p105">Represents the legend for the chart. Read-only.</span></span>|
|<span data-ttu-id="f54eb-185">series</span><span class="sxs-lookup"><span data-stu-id="f54eb-185">series</span></span>|<span data-ttu-id="f54eb-186">Coleção [ChartSeries](chartseries.md)</span><span class="sxs-lookup"><span data-stu-id="f54eb-186">[ChartSeries](chartseries.md) collection</span></span>|<span data-ttu-id="f54eb-p106">Representa uma única série ou uma coleção de séries no gráfico. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f54eb-p106">Represents either a single series or collection of series in the chart. Read-only.</span></span>|
|<span data-ttu-id="f54eb-189">title</span><span class="sxs-lookup"><span data-stu-id="f54eb-189">title</span></span>|[<span data-ttu-id="f54eb-190">ChartTitle</span><span class="sxs-lookup"><span data-stu-id="f54eb-190">ChartTitle</span></span>](charttitle.md)|<span data-ttu-id="f54eb-p107">Representa o título do gráfico especificado, incluindo o texto, a visibilidade, a posição e a formatação. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f54eb-p107">Represents the title of the specified chart, including the text, visibility, position and formating of the title. Read-only.</span></span>|
|<span data-ttu-id="f54eb-193">planilha</span><span class="sxs-lookup"><span data-stu-id="f54eb-193">worksheet</span></span>|[<span data-ttu-id="f54eb-194">Worksheet</span><span class="sxs-lookup"><span data-stu-id="f54eb-194">Worksheet</span></span>](worksheet.md)|<span data-ttu-id="f54eb-p108">A planilha que contém o gráfico atual. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f54eb-p108">The worksheet containing the current chart. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f54eb-197">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f54eb-197">JSON representation</span></span>

<span data-ttu-id="f54eb-198">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f54eb-198">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chart"
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
  "description": "Chart resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chart.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
