---
title: Tipo de recurso Chart
description: Representa um objeto de gráfico em uma pasta de trabalho.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: d274b8ec505d15ea985af22627232dbe11dc3263
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27856046"
---
# <a name="chart-resource-type"></a><span data-ttu-id="7d74b-103">Tipo de recurso Chart</span><span class="sxs-lookup"><span data-stu-id="7d74b-103">Chart resource type</span></span>

> <span data-ttu-id="7d74b-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="7d74b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7d74b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="7d74b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7d74b-106">Representa um objeto de gráfico em uma pasta de trabalho.</span><span class="sxs-lookup"><span data-stu-id="7d74b-106">Represents a chart object in a workbook.</span></span>


## <a name="methods"></a><span data-ttu-id="7d74b-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="7d74b-107">Methods</span></span>

| <span data-ttu-id="7d74b-108">Método</span><span class="sxs-lookup"><span data-stu-id="7d74b-108">Method</span></span>           | <span data-ttu-id="7d74b-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="7d74b-109">Return Type</span></span>    |<span data-ttu-id="7d74b-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="7d74b-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7d74b-111">Get Chart</span><span class="sxs-lookup"><span data-stu-id="7d74b-111">Get Chart</span></span>](../api/chart-get.md) | [<span data-ttu-id="7d74b-112">Chart</span><span class="sxs-lookup"><span data-stu-id="7d74b-112">Chart</span></span>](chart.md) |<span data-ttu-id="7d74b-113">Leia as propriedades e os relacionamentos do objeto de gráfico.</span><span class="sxs-lookup"><span data-stu-id="7d74b-113">Read properties and relationships of chart object.</span></span>|
|[<span data-ttu-id="7d74b-114">Create ChartSeries</span><span class="sxs-lookup"><span data-stu-id="7d74b-114">Create ChartSeries</span></span>](../api/chart-post-series.md) |[<span data-ttu-id="7d74b-115">ChartSeries</span><span class="sxs-lookup"><span data-stu-id="7d74b-115">ChartSeries</span></span>](chartseries.md)| <span data-ttu-id="7d74b-116">Crie uma nova ChartSeries postando na coleção de séries.</span><span class="sxs-lookup"><span data-stu-id="7d74b-116">Create a new ChartSeries by posting to the series collection.</span></span>|
|[<span data-ttu-id="7d74b-117">List series</span><span class="sxs-lookup"><span data-stu-id="7d74b-117">List series</span></span>](../api/chart-list-series.md) |<span data-ttu-id="7d74b-118">Coleção [ChartSeries](chartseries.md)</span><span class="sxs-lookup"><span data-stu-id="7d74b-118">[ChartSeries](chartseries.md) collection</span></span>| <span data-ttu-id="7d74b-119">Obtenha uma coleção de objetos ChartSeries.</span><span class="sxs-lookup"><span data-stu-id="7d74b-119">Get a ChartSeries object collection.</span></span>|
|[<span data-ttu-id="7d74b-120">Update</span><span class="sxs-lookup"><span data-stu-id="7d74b-120">Update</span></span>](../api/chart-update.md) | [<span data-ttu-id="7d74b-121">Chart</span><span class="sxs-lookup"><span data-stu-id="7d74b-121">Chart</span></span>](chart.md)   |<span data-ttu-id="7d74b-122">Atualize um objeto Chart.</span><span class="sxs-lookup"><span data-stu-id="7d74b-122">Update Chart object.</span></span> |
|[<span data-ttu-id="7d74b-123">Image</span><span class="sxs-lookup"><span data-stu-id="7d74b-123">Image</span></span>](../api/chart-image.md)|<span data-ttu-id="7d74b-124">Cadeia de caracteres de imagem codificada em base64</span><span class="sxs-lookup"><span data-stu-id="7d74b-124">Image base64 encoded string</span></span>|<span data-ttu-id="7d74b-125">Processa o gráfico como uma imagem codificada em base64, dimensionando o gráfico para se ajustar às dimensões especificadas.</span><span class="sxs-lookup"><span data-stu-id="7d74b-125">Renders the chart as a base64-encoded image by scaling the chart to fit the specified dimensions.</span></span>|
|[<span data-ttu-id="7d74b-126">Delete</span><span class="sxs-lookup"><span data-stu-id="7d74b-126">Delete</span></span>](../api/chart-delete.md)|<span data-ttu-id="7d74b-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7d74b-127">None</span></span>|<span data-ttu-id="7d74b-128">Exclui o objeto de gráfico.</span><span class="sxs-lookup"><span data-stu-id="7d74b-128">Deletes the chart object.</span></span>|
|[<span data-ttu-id="7d74b-129">SetData</span><span class="sxs-lookup"><span data-stu-id="7d74b-129">Setdata</span></span>](../api/chart-setdata.md)|<span data-ttu-id="7d74b-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7d74b-130">None</span></span>|<span data-ttu-id="7d74b-131">Redefine os dados de origem do gráfico.</span><span class="sxs-lookup"><span data-stu-id="7d74b-131">Resets the source data for the chart.</span></span>|
|[<span data-ttu-id="7d74b-132">Setposition</span><span class="sxs-lookup"><span data-stu-id="7d74b-132">Setposition</span></span>](../api/chart-setposition.md)|<span data-ttu-id="7d74b-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7d74b-133">None</span></span>|<span data-ttu-id="7d74b-134">Posiciona o gráfico em relação às células na planilha.</span><span class="sxs-lookup"><span data-stu-id="7d74b-134">Positions the chart relative to cells on the worksheet.</span></span>|
|[<span data-ttu-id="7d74b-135">List</span><span class="sxs-lookup"><span data-stu-id="7d74b-135">List</span></span>](../api/chart-list.md) | <span data-ttu-id="7d74b-136">Coleção [Chart](chart.md)</span><span class="sxs-lookup"><span data-stu-id="7d74b-136">[Chart](chart.md) collection</span></span> |<span data-ttu-id="7d74b-137">Obtenha a coleção de objetos do gráfico.</span><span class="sxs-lookup"><span data-stu-id="7d74b-137">Get chart object collection.</span></span> |
|[<span data-ttu-id="7d74b-138">Itemat</span><span class="sxs-lookup"><span data-stu-id="7d74b-138">Itemat</span></span>](../api/chartcollection-itemat.md)|[<span data-ttu-id="7d74b-139">Chart</span><span class="sxs-lookup"><span data-stu-id="7d74b-139">Chart</span></span>](chart.md)|<span data-ttu-id="7d74b-140">Obtém um gráfico com base em sua posição na coleção.</span><span class="sxs-lookup"><span data-stu-id="7d74b-140">Gets a chart based on its position in the collection.</span></span>|
|[<span data-ttu-id="7d74b-141">Add</span><span class="sxs-lookup"><span data-stu-id="7d74b-141">Add</span></span>](../api/chartcollection-add.md)|[<span data-ttu-id="7d74b-142">Chart</span><span class="sxs-lookup"><span data-stu-id="7d74b-142">Chart</span></span>](chart.md)|<span data-ttu-id="7d74b-143">Cria um novo gráfico.</span><span class="sxs-lookup"><span data-stu-id="7d74b-143">Creates a new chart.</span></span>|

## <a name="properties"></a><span data-ttu-id="7d74b-144">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7d74b-144">Properties</span></span>
| <span data-ttu-id="7d74b-145">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7d74b-145">Property</span></span>     | <span data-ttu-id="7d74b-146">Tipo</span><span class="sxs-lookup"><span data-stu-id="7d74b-146">Type</span></span>   |<span data-ttu-id="7d74b-147">Descrição</span><span class="sxs-lookup"><span data-stu-id="7d74b-147">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7d74b-148">height</span><span class="sxs-lookup"><span data-stu-id="7d74b-148">height</span></span>|<span data-ttu-id="7d74b-149">Double</span><span class="sxs-lookup"><span data-stu-id="7d74b-149">double</span></span>|<span data-ttu-id="7d74b-150">Representa a altura, em pontos, do objeto Chart.</span><span class="sxs-lookup"><span data-stu-id="7d74b-150">Represents the height, in points, of the chart object.</span></span>|
|<span data-ttu-id="7d74b-151">id</span><span class="sxs-lookup"><span data-stu-id="7d74b-151">id</span></span>|<span data-ttu-id="7d74b-152">string</span><span class="sxs-lookup"><span data-stu-id="7d74b-152">string</span></span>|<span data-ttu-id="7d74b-p102">Obtém um gráfico com base em sua posição no conjunto. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7d74b-p102">Gets a chart based on its position in the collection. Read-only.</span></span>|
|<span data-ttu-id="7d74b-155">left</span><span class="sxs-lookup"><span data-stu-id="7d74b-155">left</span></span>|<span data-ttu-id="7d74b-156">Double</span><span class="sxs-lookup"><span data-stu-id="7d74b-156">double</span></span>|<span data-ttu-id="7d74b-157">A distância, em pontos, da esquerda do gráfico à origem da planilha.</span><span class="sxs-lookup"><span data-stu-id="7d74b-157">The distance, in points, from the left side of the chart to the worksheet origin.</span></span>|
|<span data-ttu-id="7d74b-158">name</span><span class="sxs-lookup"><span data-stu-id="7d74b-158">name</span></span>|<span data-ttu-id="7d74b-159">string</span><span class="sxs-lookup"><span data-stu-id="7d74b-159">string</span></span>|<span data-ttu-id="7d74b-160">Representa o nome de um objeto Chart.</span><span class="sxs-lookup"><span data-stu-id="7d74b-160">Represents the name of a chart object.</span></span>|
|<span data-ttu-id="7d74b-161">top</span><span class="sxs-lookup"><span data-stu-id="7d74b-161">top</span></span>|<span data-ttu-id="7d74b-162">Double</span><span class="sxs-lookup"><span data-stu-id="7d74b-162">double</span></span>|<span data-ttu-id="7d74b-163">Representa a distância, em pontos, da borda superior do objeto à parte superior da primeira linha de uma planilha ou da área de um gráfico.</span><span class="sxs-lookup"><span data-stu-id="7d74b-163">Represents the distance, in points, from the top edge of the object to the top of row 1 (on a worksheet) or the top of the chart area (on a chart).</span></span>|
|<span data-ttu-id="7d74b-164">width</span><span class="sxs-lookup"><span data-stu-id="7d74b-164">width</span></span>|<span data-ttu-id="7d74b-165">Double</span><span class="sxs-lookup"><span data-stu-id="7d74b-165">double</span></span>|<span data-ttu-id="7d74b-166">Representa a largura, em pontos, do objeto de gráfico.</span><span class="sxs-lookup"><span data-stu-id="7d74b-166">Represents the width, in points, of the chart object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7d74b-167">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="7d74b-167">Relationships</span></span>
| <span data-ttu-id="7d74b-168">Relação</span><span class="sxs-lookup"><span data-stu-id="7d74b-168">Relationship</span></span> | <span data-ttu-id="7d74b-169">Tipo</span><span class="sxs-lookup"><span data-stu-id="7d74b-169">Type</span></span>   |<span data-ttu-id="7d74b-170">Descrição</span><span class="sxs-lookup"><span data-stu-id="7d74b-170">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7d74b-171">axes</span><span class="sxs-lookup"><span data-stu-id="7d74b-171">axes</span></span>|[<span data-ttu-id="7d74b-172">ChartAxes</span><span class="sxs-lookup"><span data-stu-id="7d74b-172">ChartAxes</span></span>](chartaxes.md)|<span data-ttu-id="7d74b-p103">Representa os eixos de um gráfico. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7d74b-p103">Represents chart axes. Read-only.</span></span>|
|<span data-ttu-id="7d74b-175">dataLabels</span><span class="sxs-lookup"><span data-stu-id="7d74b-175">dataLabels</span></span>|[<span data-ttu-id="7d74b-176">ChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="7d74b-176">ChartDataLabels</span></span>](chartdatalabels.md)|<span data-ttu-id="7d74b-p104">Representa os rótulos de dados no gráfico. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7d74b-p104">Represents the datalabels on the chart. Read-only.</span></span>|
|<span data-ttu-id="7d74b-179">formato</span><span class="sxs-lookup"><span data-stu-id="7d74b-179">format</span></span>|[<span data-ttu-id="7d74b-180">ChartAreaFormat</span><span class="sxs-lookup"><span data-stu-id="7d74b-180">ChartAreaFormat</span></span>](chartareaformat.md)|<span data-ttu-id="7d74b-p105">Encapsula as propriedades de formato da área do gráfico. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7d74b-p105">Encapsulates the format properties for the chart area. Read-only.</span></span>|
|<span data-ttu-id="7d74b-183">legend</span><span class="sxs-lookup"><span data-stu-id="7d74b-183">legend</span></span>|[<span data-ttu-id="7d74b-184">ChartLegend</span><span class="sxs-lookup"><span data-stu-id="7d74b-184">ChartLegend</span></span>](chartlegend.md)|<span data-ttu-id="7d74b-p106">Representa a legenda do gráfico. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7d74b-p106">Represents the legend for the chart. Read-only.</span></span>|
|<span data-ttu-id="7d74b-187">series</span><span class="sxs-lookup"><span data-stu-id="7d74b-187">series</span></span>|<span data-ttu-id="7d74b-188">Coleção [ChartSeries](chartseries.md)</span><span class="sxs-lookup"><span data-stu-id="7d74b-188">[ChartSeries](chartseries.md) collection</span></span>|<span data-ttu-id="7d74b-p107">Representa uma única série ou uma coleção de séries no gráfico. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7d74b-p107">Represents either a single series or collection of series in the chart. Read-only.</span></span>|
|<span data-ttu-id="7d74b-191">título</span><span class="sxs-lookup"><span data-stu-id="7d74b-191">title</span></span>|[<span data-ttu-id="7d74b-192">ChartTitle</span><span class="sxs-lookup"><span data-stu-id="7d74b-192">ChartTitle</span></span>](charttitle.md)|<span data-ttu-id="7d74b-p108">Representa o título do gráfico especificado, incluindo o texto, a visibilidade, a posição e a formatação. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7d74b-p108">Represents the title of the specified chart, including the text, visibility, position and formating of the title. Read-only.</span></span>|
|<span data-ttu-id="7d74b-195">planilha</span><span class="sxs-lookup"><span data-stu-id="7d74b-195">worksheet</span></span>|[<span data-ttu-id="7d74b-196">Worksheet</span><span class="sxs-lookup"><span data-stu-id="7d74b-196">Worksheet</span></span>](worksheet.md)|<span data-ttu-id="7d74b-p109">A planilha que contém o gráfico atual. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7d74b-p109">The worksheet containing the current chart. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7d74b-199">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7d74b-199">JSON representation</span></span>

<span data-ttu-id="7d74b-200">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7d74b-200">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Chart resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
