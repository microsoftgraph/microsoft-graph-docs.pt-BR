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
# <a name="workbookchart-resource-type"></a><span data-ttu-id="2bf25-103">tipo de recurso workbookChart</span><span class="sxs-lookup"><span data-stu-id="2bf25-103">workbookChart resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2bf25-104">Representa um objeto chart em uma pasta de trabalho.</span><span class="sxs-lookup"><span data-stu-id="2bf25-104">Represents a chart object in a workbook.</span></span>


## <a name="methods"></a><span data-ttu-id="2bf25-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="2bf25-105">Methods</span></span>

| <span data-ttu-id="2bf25-106">Método</span><span class="sxs-lookup"><span data-stu-id="2bf25-106">Method</span></span>           | <span data-ttu-id="2bf25-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="2bf25-107">Return Type</span></span>    |<span data-ttu-id="2bf25-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="2bf25-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2bf25-109">Get Chart</span><span class="sxs-lookup"><span data-stu-id="2bf25-109">Get Chart</span></span>](../api/chart-get.md) | [<span data-ttu-id="2bf25-110">workbookChart</span><span class="sxs-lookup"><span data-stu-id="2bf25-110">workbookChart</span></span>](workbookchart.md) |<span data-ttu-id="2bf25-111">Leia as propriedades e os relacionamentos do objeto de gráfico.</span><span class="sxs-lookup"><span data-stu-id="2bf25-111">Read properties and relationships of chart object.</span></span>|
|[<span data-ttu-id="2bf25-112">Create ChartSeries</span><span class="sxs-lookup"><span data-stu-id="2bf25-112">Create ChartSeries</span></span>](../api/chart-post-series.md) |[<span data-ttu-id="2bf25-113">workbookChartSeries</span><span class="sxs-lookup"><span data-stu-id="2bf25-113">workbookChartSeries</span></span>](workbookchartseries.md)| <span data-ttu-id="2bf25-114">Crie uma nova ChartSeries postando na coleção de séries.</span><span class="sxs-lookup"><span data-stu-id="2bf25-114">Create a new ChartSeries by posting to the series collection.</span></span>|
|[<span data-ttu-id="2bf25-115">List series</span><span class="sxs-lookup"><span data-stu-id="2bf25-115">List series</span></span>](../api/chart-list-series.md) |<span data-ttu-id="2bf25-116">coleção [workbookChartSeries](workbookchartseries.md)</span><span class="sxs-lookup"><span data-stu-id="2bf25-116">[workbookChartSeries](workbookchartseries.md) collection</span></span>| <span data-ttu-id="2bf25-117">Obtenha uma coleção de objetos ChartSeries.</span><span class="sxs-lookup"><span data-stu-id="2bf25-117">Get a ChartSeries object collection.</span></span>|
|[<span data-ttu-id="2bf25-118">Update</span><span class="sxs-lookup"><span data-stu-id="2bf25-118">Update</span></span>](../api/chart-update.md) | [<span data-ttu-id="2bf25-119">workbookChart</span><span class="sxs-lookup"><span data-stu-id="2bf25-119">workbookChart</span></span>](workbookchart.md)   |<span data-ttu-id="2bf25-120">Atualize um objeto Chart.</span><span class="sxs-lookup"><span data-stu-id="2bf25-120">Update Chart object.</span></span> |
|[<span data-ttu-id="2bf25-121">Image</span><span class="sxs-lookup"><span data-stu-id="2bf25-121">Image</span></span>](../api/chart-image.md)|<span data-ttu-id="2bf25-122">Cadeia de caracteres de imagem codificada em base64</span><span class="sxs-lookup"><span data-stu-id="2bf25-122">Image base64 encoded string</span></span>|<span data-ttu-id="2bf25-123">Processa o gráfico como uma imagem codificada em base64, dimensionando o gráfico para se ajustar às dimensões especificadas.</span><span class="sxs-lookup"><span data-stu-id="2bf25-123">Renders the chart as a base64-encoded image by scaling the chart to fit the specified dimensions.</span></span>|
|[<span data-ttu-id="2bf25-124">Delete</span><span class="sxs-lookup"><span data-stu-id="2bf25-124">Delete</span></span>](../api/chart-delete.md)|<span data-ttu-id="2bf25-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2bf25-125">None</span></span>|<span data-ttu-id="2bf25-126">Exclui o objeto de gráfico.</span><span class="sxs-lookup"><span data-stu-id="2bf25-126">Deletes the chart object.</span></span>|
|[<span data-ttu-id="2bf25-127">SetData</span><span class="sxs-lookup"><span data-stu-id="2bf25-127">Setdata</span></span>](../api/chart-setdata.md)|<span data-ttu-id="2bf25-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2bf25-128">None</span></span>|<span data-ttu-id="2bf25-129">Redefine os dados de origem do gráfico.</span><span class="sxs-lookup"><span data-stu-id="2bf25-129">Resets the source data for the chart.</span></span>|
|[<span data-ttu-id="2bf25-130">Setposition</span><span class="sxs-lookup"><span data-stu-id="2bf25-130">Setposition</span></span>](../api/chart-setposition.md)|<span data-ttu-id="2bf25-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2bf25-131">None</span></span>|<span data-ttu-id="2bf25-132">Posiciona o gráfico em relação às células na planilha.</span><span class="sxs-lookup"><span data-stu-id="2bf25-132">Positions the chart relative to cells on the worksheet.</span></span>|
|[<span data-ttu-id="2bf25-133">List</span><span class="sxs-lookup"><span data-stu-id="2bf25-133">List</span></span>](../api/chart-list.md) | <span data-ttu-id="2bf25-134">coleção [workbookChart](workbookchart.md)</span><span class="sxs-lookup"><span data-stu-id="2bf25-134">[workbookChart](workbookchart.md) collection</span></span> |<span data-ttu-id="2bf25-135">Obtenha a coleção de objetos do gráfico.</span><span class="sxs-lookup"><span data-stu-id="2bf25-135">Get chart object collection.</span></span> |
|[<span data-ttu-id="2bf25-136">Itemat</span><span class="sxs-lookup"><span data-stu-id="2bf25-136">Itemat</span></span>](../api/chartcollection-itemat.md)|[<span data-ttu-id="2bf25-137">workbookChart</span><span class="sxs-lookup"><span data-stu-id="2bf25-137">workbookChart</span></span>](workbookchart.md)|<span data-ttu-id="2bf25-138">Obtém um gráfico com base em sua posição na coleção.</span><span class="sxs-lookup"><span data-stu-id="2bf25-138">Gets a chart based on its position in the collection.</span></span>|
|[<span data-ttu-id="2bf25-139">Add</span><span class="sxs-lookup"><span data-stu-id="2bf25-139">Add</span></span>](../api/chartcollection-add.md)|[<span data-ttu-id="2bf25-140">workbookChart</span><span class="sxs-lookup"><span data-stu-id="2bf25-140">workbookChart</span></span>](workbookchart.md)|<span data-ttu-id="2bf25-141">Cria um novo gráfico.</span><span class="sxs-lookup"><span data-stu-id="2bf25-141">Creates a new chart.</span></span>|

## <a name="properties"></a><span data-ttu-id="2bf25-142">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2bf25-142">Properties</span></span>
| <span data-ttu-id="2bf25-143">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2bf25-143">Property</span></span>     | <span data-ttu-id="2bf25-144">Tipo</span><span class="sxs-lookup"><span data-stu-id="2bf25-144">Type</span></span>   |<span data-ttu-id="2bf25-145">Descrição</span><span class="sxs-lookup"><span data-stu-id="2bf25-145">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2bf25-146">height</span><span class="sxs-lookup"><span data-stu-id="2bf25-146">height</span></span>|<span data-ttu-id="2bf25-147">double</span><span class="sxs-lookup"><span data-stu-id="2bf25-147">double</span></span>|<span data-ttu-id="2bf25-148">Representa a altura, em pontos, do objeto Chart.</span><span class="sxs-lookup"><span data-stu-id="2bf25-148">Represents the height, in points, of the chart object.</span></span>|
|<span data-ttu-id="2bf25-149">id</span><span class="sxs-lookup"><span data-stu-id="2bf25-149">id</span></span>|<span data-ttu-id="2bf25-150">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2bf25-150">string</span></span>|<span data-ttu-id="2bf25-p101">Obtém um gráfico com base em sua posição no conjunto. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2bf25-p101">Gets a chart based on its position in the collection. Read-only.</span></span>|
|<span data-ttu-id="2bf25-153">left</span><span class="sxs-lookup"><span data-stu-id="2bf25-153">left</span></span>|<span data-ttu-id="2bf25-154">double</span><span class="sxs-lookup"><span data-stu-id="2bf25-154">double</span></span>|<span data-ttu-id="2bf25-155">A distância, em pontos, da esquerda do gráfico à origem da planilha.</span><span class="sxs-lookup"><span data-stu-id="2bf25-155">The distance, in points, from the left side of the chart to the worksheet origin.</span></span>|
|<span data-ttu-id="2bf25-156">name</span><span class="sxs-lookup"><span data-stu-id="2bf25-156">name</span></span>|<span data-ttu-id="2bf25-157">string</span><span class="sxs-lookup"><span data-stu-id="2bf25-157">string</span></span>|<span data-ttu-id="2bf25-158">Representa o nome de um objeto Chart.</span><span class="sxs-lookup"><span data-stu-id="2bf25-158">Represents the name of a chart object.</span></span>|
|<span data-ttu-id="2bf25-159">top</span><span class="sxs-lookup"><span data-stu-id="2bf25-159">top</span></span>|<span data-ttu-id="2bf25-160">duplo</span><span class="sxs-lookup"><span data-stu-id="2bf25-160">double</span></span>|<span data-ttu-id="2bf25-161">Representa a distância, em pontos, da borda superior do objeto à parte superior da primeira linha de uma planilha ou da área de um gráfico.</span><span class="sxs-lookup"><span data-stu-id="2bf25-161">Represents the distance, in points, from the top edge of the object to the top of row 1 (on a worksheet) or the top of the chart area (on a chart).</span></span>|
|<span data-ttu-id="2bf25-162">width</span><span class="sxs-lookup"><span data-stu-id="2bf25-162">width</span></span>|<span data-ttu-id="2bf25-163">Double</span><span class="sxs-lookup"><span data-stu-id="2bf25-163">double</span></span>|<span data-ttu-id="2bf25-164">Representa a largura, em pontos, do objeto de gráfico.</span><span class="sxs-lookup"><span data-stu-id="2bf25-164">Represents the width, in points, of the chart object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2bf25-165">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="2bf25-165">Relationships</span></span>
| <span data-ttu-id="2bf25-166">Relação</span><span class="sxs-lookup"><span data-stu-id="2bf25-166">Relationship</span></span> | <span data-ttu-id="2bf25-167">Tipo</span><span class="sxs-lookup"><span data-stu-id="2bf25-167">Type</span></span>   |<span data-ttu-id="2bf25-168">Descrição</span><span class="sxs-lookup"><span data-stu-id="2bf25-168">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2bf25-169">axes</span><span class="sxs-lookup"><span data-stu-id="2bf25-169">axes</span></span>|[<span data-ttu-id="2bf25-170">workbookChartAxes</span><span class="sxs-lookup"><span data-stu-id="2bf25-170">workbookChartAxes</span></span>](workbookchartaxes.md)|<span data-ttu-id="2bf25-p102">Representa os eixos de um gráfico. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2bf25-p102">Represents chart axes. Read-only.</span></span>|
|<span data-ttu-id="2bf25-173">dataLabels</span><span class="sxs-lookup"><span data-stu-id="2bf25-173">dataLabels</span></span>|[<span data-ttu-id="2bf25-174">workbookChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="2bf25-174">workbookChartDataLabels</span></span>](workbookchartdatalabels.md)|<span data-ttu-id="2bf25-p103">Representa os rótulos de dados no gráfico. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2bf25-p103">Represents the datalabels on the chart. Read-only.</span></span>|
|<span data-ttu-id="2bf25-177">format</span><span class="sxs-lookup"><span data-stu-id="2bf25-177">format</span></span>|[<span data-ttu-id="2bf25-178">workbookChartAreaFormat</span><span class="sxs-lookup"><span data-stu-id="2bf25-178">workbookChartAreaFormat</span></span>](workbookchartareaformat.md)|<span data-ttu-id="2bf25-p104">Encapsula as propriedades de formato da área do gráfico. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2bf25-p104">Encapsulates the format properties for the chart area. Read-only.</span></span>|
|<span data-ttu-id="2bf25-181">legend</span><span class="sxs-lookup"><span data-stu-id="2bf25-181">legend</span></span>|[<span data-ttu-id="2bf25-182">workbookChartLegend</span><span class="sxs-lookup"><span data-stu-id="2bf25-182">workbookChartLegend</span></span>](workbookchartlegend.md)|<span data-ttu-id="2bf25-p105">Representa a legenda do gráfico. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2bf25-p105">Represents the legend for the chart. Read-only.</span></span>|
|<span data-ttu-id="2bf25-185">series</span><span class="sxs-lookup"><span data-stu-id="2bf25-185">series</span></span>|<span data-ttu-id="2bf25-186">coleção [workbookChartSeries](workbookchartseries.md)</span><span class="sxs-lookup"><span data-stu-id="2bf25-186">[workbookChartSeries](workbookchartseries.md) collection</span></span>|<span data-ttu-id="2bf25-p106">Representa uma única série ou uma coleção de séries no gráfico. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2bf25-p106">Represents either a single series or collection of series in the chart. Read-only.</span></span>|
|<span data-ttu-id="2bf25-189">title</span><span class="sxs-lookup"><span data-stu-id="2bf25-189">title</span></span>|[<span data-ttu-id="2bf25-190">workbookChartTitle</span><span class="sxs-lookup"><span data-stu-id="2bf25-190">workbookChartTitle</span></span>](workbookcharttitle.md)|<span data-ttu-id="2bf25-p107">Representa o título do gráfico especificado, incluindo o texto, a visibilidade, a posição e a formatação. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2bf25-p107">Represents the title of the specified chart, including the text, visibility, position and formating of the title. Read-only.</span></span>|
|<span data-ttu-id="2bf25-193">planilha</span><span class="sxs-lookup"><span data-stu-id="2bf25-193">worksheet</span></span>|[<span data-ttu-id="2bf25-194">workbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="2bf25-194">workbookWorksheet</span></span>](workbookworksheet.md)|<span data-ttu-id="2bf25-195">A planilha que contém o gráfico atual.</span><span class="sxs-lookup"><span data-stu-id="2bf25-195">The worksheet containing the current chart.</span></span> <span data-ttu-id="2bf25-196">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2bf25-196">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2bf25-197">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2bf25-197">JSON representation</span></span>

<span data-ttu-id="2bf25-198">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2bf25-198">Here is a JSON representation of the resource.</span></span>

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
