---
title: Tipo de recurso Chart
description: Representa um objeto de gráfico em uma pasta de trabalho.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 09d5fd376cfdcd03517cc989708bbf17bcf49a72
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27970672"
---
# <a name="chart-resource-type"></a><span data-ttu-id="a6962-103">Tipo de recurso Chart</span><span class="sxs-lookup"><span data-stu-id="a6962-103">Chart resource type</span></span>

> <span data-ttu-id="a6962-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a6962-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a6962-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a6962-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a6962-106">Representa um objeto de gráfico em uma pasta de trabalho.</span><span class="sxs-lookup"><span data-stu-id="a6962-106">Represents a chart object in a workbook.</span></span>


## <a name="methods"></a><span data-ttu-id="a6962-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="a6962-107">Methods</span></span>

| <span data-ttu-id="a6962-108">Método</span><span class="sxs-lookup"><span data-stu-id="a6962-108">Method</span></span>           | <span data-ttu-id="a6962-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="a6962-109">Return Type</span></span>    |<span data-ttu-id="a6962-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a6962-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a6962-111">Get Chart</span><span class="sxs-lookup"><span data-stu-id="a6962-111">Get Chart</span></span>](../api/chart-get.md) | [<span data-ttu-id="a6962-112">Chart</span><span class="sxs-lookup"><span data-stu-id="a6962-112">Chart</span></span>](chart.md) |<span data-ttu-id="a6962-113">Leia as propriedades e os relacionamentos do objeto de gráfico.</span><span class="sxs-lookup"><span data-stu-id="a6962-113">Read properties and relationships of chart object.</span></span>|
|[<span data-ttu-id="a6962-114">Create ChartSeries</span><span class="sxs-lookup"><span data-stu-id="a6962-114">Create ChartSeries</span></span>](../api/chart-post-series.md) |[<span data-ttu-id="a6962-115">ChartSeries</span><span class="sxs-lookup"><span data-stu-id="a6962-115">ChartSeries</span></span>](chartseries.md)| <span data-ttu-id="a6962-116">Crie uma nova ChartSeries postando na coleção de séries.</span><span class="sxs-lookup"><span data-stu-id="a6962-116">Create a new ChartSeries by posting to the series collection.</span></span>|
|[<span data-ttu-id="a6962-117">List series</span><span class="sxs-lookup"><span data-stu-id="a6962-117">List series</span></span>](../api/chart-list-series.md) |<span data-ttu-id="a6962-118">Coleção [ChartSeries](chartseries.md)</span><span class="sxs-lookup"><span data-stu-id="a6962-118">[ChartSeries](chartseries.md) collection</span></span>| <span data-ttu-id="a6962-119">Obtenha uma coleção de objetos ChartSeries.</span><span class="sxs-lookup"><span data-stu-id="a6962-119">Get a ChartSeries object collection.</span></span>|
|[<span data-ttu-id="a6962-120">Update</span><span class="sxs-lookup"><span data-stu-id="a6962-120">Update</span></span>](../api/chart-update.md) | [<span data-ttu-id="a6962-121">Chart</span><span class="sxs-lookup"><span data-stu-id="a6962-121">Chart</span></span>](chart.md)   |<span data-ttu-id="a6962-122">Atualize um objeto Chart.</span><span class="sxs-lookup"><span data-stu-id="a6962-122">Update Chart object.</span></span> |
|[<span data-ttu-id="a6962-123">Image</span><span class="sxs-lookup"><span data-stu-id="a6962-123">Image</span></span>](../api/chart-image.md)|<span data-ttu-id="a6962-124">Cadeia de caracteres de imagem codificada em base64</span><span class="sxs-lookup"><span data-stu-id="a6962-124">Image base64 encoded string</span></span>|<span data-ttu-id="a6962-125">Processa o gráfico como uma imagem codificada em base64, dimensionando o gráfico para se ajustar às dimensões especificadas.</span><span class="sxs-lookup"><span data-stu-id="a6962-125">Renders the chart as a base64-encoded image by scaling the chart to fit the specified dimensions.</span></span>|
|[<span data-ttu-id="a6962-126">Delete</span><span class="sxs-lookup"><span data-stu-id="a6962-126">Delete</span></span>](../api/chart-delete.md)|<span data-ttu-id="a6962-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a6962-127">None</span></span>|<span data-ttu-id="a6962-128">Exclui o objeto de gráfico.</span><span class="sxs-lookup"><span data-stu-id="a6962-128">Deletes the chart object.</span></span>|
|[<span data-ttu-id="a6962-129">SetData</span><span class="sxs-lookup"><span data-stu-id="a6962-129">Setdata</span></span>](../api/chart-setdata.md)|<span data-ttu-id="a6962-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a6962-130">None</span></span>|<span data-ttu-id="a6962-131">Redefine os dados de origem do gráfico.</span><span class="sxs-lookup"><span data-stu-id="a6962-131">Resets the source data for the chart.</span></span>|
|[<span data-ttu-id="a6962-132">Setposition</span><span class="sxs-lookup"><span data-stu-id="a6962-132">Setposition</span></span>](../api/chart-setposition.md)|<span data-ttu-id="a6962-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a6962-133">None</span></span>|<span data-ttu-id="a6962-134">Posiciona o gráfico em relação às células na planilha.</span><span class="sxs-lookup"><span data-stu-id="a6962-134">Positions the chart relative to cells on the worksheet.</span></span>|
|[<span data-ttu-id="a6962-135">List</span><span class="sxs-lookup"><span data-stu-id="a6962-135">List</span></span>](../api/chart-list.md) | <span data-ttu-id="a6962-136">Coleção [Chart](chart.md)</span><span class="sxs-lookup"><span data-stu-id="a6962-136">[Chart](chart.md) collection</span></span> |<span data-ttu-id="a6962-137">Obtenha a coleção de objetos do gráfico.</span><span class="sxs-lookup"><span data-stu-id="a6962-137">Get chart object collection.</span></span> |
|[<span data-ttu-id="a6962-138">Itemat</span><span class="sxs-lookup"><span data-stu-id="a6962-138">Itemat</span></span>](../api/chartcollection-itemat.md)|[<span data-ttu-id="a6962-139">Chart</span><span class="sxs-lookup"><span data-stu-id="a6962-139">Chart</span></span>](chart.md)|<span data-ttu-id="a6962-140">Obtém um gráfico com base em sua posição na coleção.</span><span class="sxs-lookup"><span data-stu-id="a6962-140">Gets a chart based on its position in the collection.</span></span>|
|[<span data-ttu-id="a6962-141">Add</span><span class="sxs-lookup"><span data-stu-id="a6962-141">Add</span></span>](../api/chartcollection-add.md)|[<span data-ttu-id="a6962-142">Chart</span><span class="sxs-lookup"><span data-stu-id="a6962-142">Chart</span></span>](chart.md)|<span data-ttu-id="a6962-143">Cria um novo gráfico.</span><span class="sxs-lookup"><span data-stu-id="a6962-143">Creates a new chart.</span></span>|

## <a name="properties"></a><span data-ttu-id="a6962-144">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a6962-144">Properties</span></span>
| <span data-ttu-id="a6962-145">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a6962-145">Property</span></span>     | <span data-ttu-id="a6962-146">Tipo</span><span class="sxs-lookup"><span data-stu-id="a6962-146">Type</span></span>   |<span data-ttu-id="a6962-147">Descrição</span><span class="sxs-lookup"><span data-stu-id="a6962-147">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a6962-148">height</span><span class="sxs-lookup"><span data-stu-id="a6962-148">height</span></span>|<span data-ttu-id="a6962-149">Double</span><span class="sxs-lookup"><span data-stu-id="a6962-149">double</span></span>|<span data-ttu-id="a6962-150">Representa a altura, em pontos, do objeto Chart.</span><span class="sxs-lookup"><span data-stu-id="a6962-150">Represents the height, in points, of the chart object.</span></span>|
|<span data-ttu-id="a6962-151">id</span><span class="sxs-lookup"><span data-stu-id="a6962-151">id</span></span>|<span data-ttu-id="a6962-152">string</span><span class="sxs-lookup"><span data-stu-id="a6962-152">string</span></span>|<span data-ttu-id="a6962-p102">Obtém um gráfico com base em sua posição no conjunto. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a6962-p102">Gets a chart based on its position in the collection. Read-only.</span></span>|
|<span data-ttu-id="a6962-155">left</span><span class="sxs-lookup"><span data-stu-id="a6962-155">left</span></span>|<span data-ttu-id="a6962-156">Double</span><span class="sxs-lookup"><span data-stu-id="a6962-156">double</span></span>|<span data-ttu-id="a6962-157">A distância, em pontos, da esquerda do gráfico à origem da planilha.</span><span class="sxs-lookup"><span data-stu-id="a6962-157">The distance, in points, from the left side of the chart to the worksheet origin.</span></span>|
|<span data-ttu-id="a6962-158">name</span><span class="sxs-lookup"><span data-stu-id="a6962-158">name</span></span>|<span data-ttu-id="a6962-159">string</span><span class="sxs-lookup"><span data-stu-id="a6962-159">string</span></span>|<span data-ttu-id="a6962-160">Representa o nome de um objeto Chart.</span><span class="sxs-lookup"><span data-stu-id="a6962-160">Represents the name of a chart object.</span></span>|
|<span data-ttu-id="a6962-161">top</span><span class="sxs-lookup"><span data-stu-id="a6962-161">top</span></span>|<span data-ttu-id="a6962-162">Double</span><span class="sxs-lookup"><span data-stu-id="a6962-162">double</span></span>|<span data-ttu-id="a6962-163">Representa a distância, em pontos, da borda superior do objeto à parte superior da primeira linha de uma planilha ou da área de um gráfico.</span><span class="sxs-lookup"><span data-stu-id="a6962-163">Represents the distance, in points, from the top edge of the object to the top of row 1 (on a worksheet) or the top of the chart area (on a chart).</span></span>|
|<span data-ttu-id="a6962-164">width</span><span class="sxs-lookup"><span data-stu-id="a6962-164">width</span></span>|<span data-ttu-id="a6962-165">Double</span><span class="sxs-lookup"><span data-stu-id="a6962-165">double</span></span>|<span data-ttu-id="a6962-166">Representa a largura, em pontos, do objeto de gráfico.</span><span class="sxs-lookup"><span data-stu-id="a6962-166">Represents the width, in points, of the chart object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a6962-167">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="a6962-167">Relationships</span></span>
| <span data-ttu-id="a6962-168">Relação</span><span class="sxs-lookup"><span data-stu-id="a6962-168">Relationship</span></span> | <span data-ttu-id="a6962-169">Tipo</span><span class="sxs-lookup"><span data-stu-id="a6962-169">Type</span></span>   |<span data-ttu-id="a6962-170">Descrição</span><span class="sxs-lookup"><span data-stu-id="a6962-170">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a6962-171">axes</span><span class="sxs-lookup"><span data-stu-id="a6962-171">axes</span></span>|[<span data-ttu-id="a6962-172">ChartAxes</span><span class="sxs-lookup"><span data-stu-id="a6962-172">ChartAxes</span></span>](chartaxes.md)|<span data-ttu-id="a6962-p103">Representa os eixos de um gráfico. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a6962-p103">Represents chart axes. Read-only.</span></span>|
|<span data-ttu-id="a6962-175">dataLabels</span><span class="sxs-lookup"><span data-stu-id="a6962-175">dataLabels</span></span>|[<span data-ttu-id="a6962-176">ChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="a6962-176">ChartDataLabels</span></span>](chartdatalabels.md)|<span data-ttu-id="a6962-p104">Representa os rótulos de dados no gráfico. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a6962-p104">Represents the datalabels on the chart. Read-only.</span></span>|
|<span data-ttu-id="a6962-179">formato</span><span class="sxs-lookup"><span data-stu-id="a6962-179">format</span></span>|[<span data-ttu-id="a6962-180">ChartAreaFormat</span><span class="sxs-lookup"><span data-stu-id="a6962-180">ChartAreaFormat</span></span>](chartareaformat.md)|<span data-ttu-id="a6962-p105">Encapsula as propriedades de formato da área do gráfico. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a6962-p105">Encapsulates the format properties for the chart area. Read-only.</span></span>|
|<span data-ttu-id="a6962-183">legend</span><span class="sxs-lookup"><span data-stu-id="a6962-183">legend</span></span>|[<span data-ttu-id="a6962-184">ChartLegend</span><span class="sxs-lookup"><span data-stu-id="a6962-184">ChartLegend</span></span>](chartlegend.md)|<span data-ttu-id="a6962-p106">Representa a legenda do gráfico. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a6962-p106">Represents the legend for the chart. Read-only.</span></span>|
|<span data-ttu-id="a6962-187">series</span><span class="sxs-lookup"><span data-stu-id="a6962-187">series</span></span>|<span data-ttu-id="a6962-188">Coleção [ChartSeries](chartseries.md)</span><span class="sxs-lookup"><span data-stu-id="a6962-188">[ChartSeries](chartseries.md) collection</span></span>|<span data-ttu-id="a6962-p107">Representa uma única série ou uma coleção de séries no gráfico. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a6962-p107">Represents either a single series or collection of series in the chart. Read-only.</span></span>|
|<span data-ttu-id="a6962-191">título</span><span class="sxs-lookup"><span data-stu-id="a6962-191">title</span></span>|[<span data-ttu-id="a6962-192">ChartTitle</span><span class="sxs-lookup"><span data-stu-id="a6962-192">ChartTitle</span></span>](charttitle.md)|<span data-ttu-id="a6962-p108">Representa o título do gráfico especificado, incluindo o texto, a visibilidade, a posição e a formatação. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a6962-p108">Represents the title of the specified chart, including the text, visibility, position and formating of the title. Read-only.</span></span>|
|<span data-ttu-id="a6962-195">planilha</span><span class="sxs-lookup"><span data-stu-id="a6962-195">worksheet</span></span>|[<span data-ttu-id="a6962-196">Worksheet</span><span class="sxs-lookup"><span data-stu-id="a6962-196">Worksheet</span></span>](worksheet.md)|<span data-ttu-id="a6962-p109">A planilha que contém o gráfico atual. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a6962-p109">The worksheet containing the current chart. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a6962-199">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a6962-199">JSON representation</span></span>

<span data-ttu-id="a6962-200">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a6962-200">Here is a JSON representation of the resource.</span></span>

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
