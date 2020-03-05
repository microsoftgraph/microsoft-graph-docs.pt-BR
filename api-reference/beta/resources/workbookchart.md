---
title: tipo de recurso workbookChart
description: Representa um objeto chart em uma pasta de trabalho.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: f28e89ae20d5675da303f11dc67b6e4b562b5340
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519404"
---
# <a name="workbookchart-resource-type"></a><span data-ttu-id="6a075-103">tipo de recurso workbookChart</span><span class="sxs-lookup"><span data-stu-id="6a075-103">workbookChart resource type</span></span>

<span data-ttu-id="6a075-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="6a075-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6a075-105">Representa um objeto chart em uma pasta de trabalho.</span><span class="sxs-lookup"><span data-stu-id="6a075-105">Represents a chart object in a workbook.</span></span>


## <a name="methods"></a><span data-ttu-id="6a075-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="6a075-106">Methods</span></span>

| <span data-ttu-id="6a075-107">Método</span><span class="sxs-lookup"><span data-stu-id="6a075-107">Method</span></span>           | <span data-ttu-id="6a075-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="6a075-108">Return Type</span></span>    |<span data-ttu-id="6a075-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="6a075-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6a075-110">Get Chart</span><span class="sxs-lookup"><span data-stu-id="6a075-110">Get Chart</span></span>](../api/chart-get.md) | [<span data-ttu-id="6a075-111">workbookChart</span><span class="sxs-lookup"><span data-stu-id="6a075-111">workbookChart</span></span>](workbookchart.md) |<span data-ttu-id="6a075-112">Leia as propriedades e os relacionamentos do objeto de gráfico.</span><span class="sxs-lookup"><span data-stu-id="6a075-112">Read properties and relationships of chart object.</span></span>|
|[<span data-ttu-id="6a075-113">Create ChartSeries</span><span class="sxs-lookup"><span data-stu-id="6a075-113">Create ChartSeries</span></span>](../api/chart-post-series.md) |[<span data-ttu-id="6a075-114">workbookChartSeries</span><span class="sxs-lookup"><span data-stu-id="6a075-114">workbookChartSeries</span></span>](workbookchartseries.md)| <span data-ttu-id="6a075-115">Crie uma nova ChartSeries postando na coleção de séries.</span><span class="sxs-lookup"><span data-stu-id="6a075-115">Create a new ChartSeries by posting to the series collection.</span></span>|
|[<span data-ttu-id="6a075-116">List series</span><span class="sxs-lookup"><span data-stu-id="6a075-116">List series</span></span>](../api/chart-list-series.md) |<span data-ttu-id="6a075-117">coleção [workbookChartSeries](workbookchartseries.md)</span><span class="sxs-lookup"><span data-stu-id="6a075-117">[workbookChartSeries](workbookchartseries.md) collection</span></span>| <span data-ttu-id="6a075-118">Obtenha uma coleção de objetos ChartSeries.</span><span class="sxs-lookup"><span data-stu-id="6a075-118">Get a ChartSeries object collection.</span></span>|
|[<span data-ttu-id="6a075-119">Update</span><span class="sxs-lookup"><span data-stu-id="6a075-119">Update</span></span>](../api/chart-update.md) | [<span data-ttu-id="6a075-120">workbookChart</span><span class="sxs-lookup"><span data-stu-id="6a075-120">workbookChart</span></span>](workbookchart.md)   |<span data-ttu-id="6a075-121">Atualize um objeto Chart.</span><span class="sxs-lookup"><span data-stu-id="6a075-121">Update Chart object.</span></span> |
|[<span data-ttu-id="6a075-122">Image</span><span class="sxs-lookup"><span data-stu-id="6a075-122">Image</span></span>](../api/chart-image.md)|<span data-ttu-id="6a075-123">Cadeia de caracteres de imagem codificada em base64</span><span class="sxs-lookup"><span data-stu-id="6a075-123">Image base64 encoded string</span></span>|<span data-ttu-id="6a075-124">Processa o gráfico como uma imagem codificada em base64, dimensionando o gráfico para se ajustar às dimensões especificadas.</span><span class="sxs-lookup"><span data-stu-id="6a075-124">Renders the chart as a base64-encoded image by scaling the chart to fit the specified dimensions.</span></span>|
|[<span data-ttu-id="6a075-125">Delete</span><span class="sxs-lookup"><span data-stu-id="6a075-125">Delete</span></span>](../api/chart-delete.md)|<span data-ttu-id="6a075-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6a075-126">None</span></span>|<span data-ttu-id="6a075-127">Exclui o objeto de gráfico.</span><span class="sxs-lookup"><span data-stu-id="6a075-127">Deletes the chart object.</span></span>|
|[<span data-ttu-id="6a075-128">SetData</span><span class="sxs-lookup"><span data-stu-id="6a075-128">Setdata</span></span>](../api/chart-setdata.md)|<span data-ttu-id="6a075-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6a075-129">None</span></span>|<span data-ttu-id="6a075-130">Redefine os dados de origem do gráfico.</span><span class="sxs-lookup"><span data-stu-id="6a075-130">Resets the source data for the chart.</span></span>|
|[<span data-ttu-id="6a075-131">Setposition</span><span class="sxs-lookup"><span data-stu-id="6a075-131">Setposition</span></span>](../api/chart-setposition.md)|<span data-ttu-id="6a075-132">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6a075-132">None</span></span>|<span data-ttu-id="6a075-133">Posiciona o gráfico em relação às células na planilha.</span><span class="sxs-lookup"><span data-stu-id="6a075-133">Positions the chart relative to cells on the worksheet.</span></span>|
|[<span data-ttu-id="6a075-134">List</span><span class="sxs-lookup"><span data-stu-id="6a075-134">List</span></span>](../api/chart-list.md) | <span data-ttu-id="6a075-135">coleção [workbookChart](workbookchart.md)</span><span class="sxs-lookup"><span data-stu-id="6a075-135">[workbookChart](workbookchart.md) collection</span></span> |<span data-ttu-id="6a075-136">Obtenha a coleção de objetos do gráfico.</span><span class="sxs-lookup"><span data-stu-id="6a075-136">Get chart object collection.</span></span> |
|[<span data-ttu-id="6a075-137">Itemat</span><span class="sxs-lookup"><span data-stu-id="6a075-137">Itemat</span></span>](../api/chartcollection-itemat.md)|[<span data-ttu-id="6a075-138">workbookChart</span><span class="sxs-lookup"><span data-stu-id="6a075-138">workbookChart</span></span>](workbookchart.md)|<span data-ttu-id="6a075-139">Obtém um gráfico com base em sua posição na coleção.</span><span class="sxs-lookup"><span data-stu-id="6a075-139">Gets a chart based on its position in the collection.</span></span>|
|[<span data-ttu-id="6a075-140">Add</span><span class="sxs-lookup"><span data-stu-id="6a075-140">Add</span></span>](../api/chartcollection-add.md)|[<span data-ttu-id="6a075-141">workbookChart</span><span class="sxs-lookup"><span data-stu-id="6a075-141">workbookChart</span></span>](workbookchart.md)|<span data-ttu-id="6a075-142">Cria um novo gráfico.</span><span class="sxs-lookup"><span data-stu-id="6a075-142">Creates a new chart.</span></span>|

## <a name="properties"></a><span data-ttu-id="6a075-143">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6a075-143">Properties</span></span>
| <span data-ttu-id="6a075-144">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6a075-144">Property</span></span>     | <span data-ttu-id="6a075-145">Tipo</span><span class="sxs-lookup"><span data-stu-id="6a075-145">Type</span></span>   |<span data-ttu-id="6a075-146">Descrição</span><span class="sxs-lookup"><span data-stu-id="6a075-146">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6a075-147">height</span><span class="sxs-lookup"><span data-stu-id="6a075-147">height</span></span>|<span data-ttu-id="6a075-148">double</span><span class="sxs-lookup"><span data-stu-id="6a075-148">double</span></span>|<span data-ttu-id="6a075-149">Representa a altura, em pontos, do objeto Chart.</span><span class="sxs-lookup"><span data-stu-id="6a075-149">Represents the height, in points, of the chart object.</span></span>|
|<span data-ttu-id="6a075-150">id</span><span class="sxs-lookup"><span data-stu-id="6a075-150">id</span></span>|<span data-ttu-id="6a075-151">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6a075-151">string</span></span>|<span data-ttu-id="6a075-p101">Obtém um gráfico com base em sua posição no conjunto. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6a075-p101">Gets a chart based on its position in the collection. Read-only.</span></span>|
|<span data-ttu-id="6a075-154">left</span><span class="sxs-lookup"><span data-stu-id="6a075-154">left</span></span>|<span data-ttu-id="6a075-155">double</span><span class="sxs-lookup"><span data-stu-id="6a075-155">double</span></span>|<span data-ttu-id="6a075-156">A distância, em pontos, da esquerda do gráfico à origem da planilha.</span><span class="sxs-lookup"><span data-stu-id="6a075-156">The distance, in points, from the left side of the chart to the worksheet origin.</span></span>|
|<span data-ttu-id="6a075-157">nome</span><span class="sxs-lookup"><span data-stu-id="6a075-157">name</span></span>|<span data-ttu-id="6a075-158">string</span><span class="sxs-lookup"><span data-stu-id="6a075-158">string</span></span>|<span data-ttu-id="6a075-159">Representa o nome de um objeto Chart.</span><span class="sxs-lookup"><span data-stu-id="6a075-159">Represents the name of a chart object.</span></span>|
|<span data-ttu-id="6a075-160">top</span><span class="sxs-lookup"><span data-stu-id="6a075-160">top</span></span>|<span data-ttu-id="6a075-161">duplo</span><span class="sxs-lookup"><span data-stu-id="6a075-161">double</span></span>|<span data-ttu-id="6a075-162">Representa a distância, em pontos, da borda superior do objeto à parte superior da primeira linha de uma planilha ou da área de um gráfico.</span><span class="sxs-lookup"><span data-stu-id="6a075-162">Represents the distance, in points, from the top edge of the object to the top of row 1 (on a worksheet) or the top of the chart area (on a chart).</span></span>|
|<span data-ttu-id="6a075-163">width</span><span class="sxs-lookup"><span data-stu-id="6a075-163">width</span></span>|<span data-ttu-id="6a075-164">Double</span><span class="sxs-lookup"><span data-stu-id="6a075-164">double</span></span>|<span data-ttu-id="6a075-165">Representa a largura, em pontos, do objeto de gráfico.</span><span class="sxs-lookup"><span data-stu-id="6a075-165">Represents the width, in points, of the chart object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6a075-166">Relações</span><span class="sxs-lookup"><span data-stu-id="6a075-166">Relationships</span></span>
| <span data-ttu-id="6a075-167">Relação</span><span class="sxs-lookup"><span data-stu-id="6a075-167">Relationship</span></span> | <span data-ttu-id="6a075-168">Tipo</span><span class="sxs-lookup"><span data-stu-id="6a075-168">Type</span></span>   |<span data-ttu-id="6a075-169">Descrição</span><span class="sxs-lookup"><span data-stu-id="6a075-169">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6a075-170">axes</span><span class="sxs-lookup"><span data-stu-id="6a075-170">axes</span></span>|[<span data-ttu-id="6a075-171">workbookChartAxes</span><span class="sxs-lookup"><span data-stu-id="6a075-171">workbookChartAxes</span></span>](workbookchartaxes.md)|<span data-ttu-id="6a075-p102">Representa os eixos de um gráfico. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6a075-p102">Represents chart axes. Read-only.</span></span>|
|<span data-ttu-id="6a075-174">dataLabels</span><span class="sxs-lookup"><span data-stu-id="6a075-174">dataLabels</span></span>|[<span data-ttu-id="6a075-175">workbookChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="6a075-175">workbookChartDataLabels</span></span>](workbookchartdatalabels.md)|<span data-ttu-id="6a075-p103">Representa os rótulos de dados no gráfico. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6a075-p103">Represents the datalabels on the chart. Read-only.</span></span>|
|<span data-ttu-id="6a075-178">format</span><span class="sxs-lookup"><span data-stu-id="6a075-178">format</span></span>|[<span data-ttu-id="6a075-179">workbookChartAreaFormat</span><span class="sxs-lookup"><span data-stu-id="6a075-179">workbookChartAreaFormat</span></span>](workbookchartareaformat.md)|<span data-ttu-id="6a075-p104">Encapsula as propriedades de formato da área do gráfico. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6a075-p104">Encapsulates the format properties for the chart area. Read-only.</span></span>|
|<span data-ttu-id="6a075-182">legend</span><span class="sxs-lookup"><span data-stu-id="6a075-182">legend</span></span>|[<span data-ttu-id="6a075-183">workbookChartLegend</span><span class="sxs-lookup"><span data-stu-id="6a075-183">workbookChartLegend</span></span>](workbookchartlegend.md)|<span data-ttu-id="6a075-p105">Representa a legenda do gráfico. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6a075-p105">Represents the legend for the chart. Read-only.</span></span>|
|<span data-ttu-id="6a075-186">series</span><span class="sxs-lookup"><span data-stu-id="6a075-186">series</span></span>|<span data-ttu-id="6a075-187">coleção [workbookChartSeries](workbookchartseries.md)</span><span class="sxs-lookup"><span data-stu-id="6a075-187">[workbookChartSeries](workbookchartseries.md) collection</span></span>|<span data-ttu-id="6a075-p106">Representa uma única série ou uma coleção de séries no gráfico. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6a075-p106">Represents either a single series or collection of series in the chart. Read-only.</span></span>|
|<span data-ttu-id="6a075-190">title</span><span class="sxs-lookup"><span data-stu-id="6a075-190">title</span></span>|[<span data-ttu-id="6a075-191">workbookChartTitle</span><span class="sxs-lookup"><span data-stu-id="6a075-191">workbookChartTitle</span></span>](workbookcharttitle.md)|<span data-ttu-id="6a075-p107">Representa o título do gráfico especificado, incluindo o texto, a visibilidade, a posição e a formatação. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6a075-p107">Represents the title of the specified chart, including the text, visibility, position and formating of the title. Read-only.</span></span>|
|<span data-ttu-id="6a075-194">planilha</span><span class="sxs-lookup"><span data-stu-id="6a075-194">worksheet</span></span>|[<span data-ttu-id="6a075-195">workbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="6a075-195">workbookWorksheet</span></span>](workbookworksheet.md)|<span data-ttu-id="6a075-196">A planilha que contém o gráfico atual.</span><span class="sxs-lookup"><span data-stu-id="6a075-196">The worksheet containing the current chart.</span></span> <span data-ttu-id="6a075-197">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6a075-197">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6a075-198">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6a075-198">JSON representation</span></span>

<span data-ttu-id="6a075-199">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6a075-199">Here is a JSON representation of the resource.</span></span>

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
