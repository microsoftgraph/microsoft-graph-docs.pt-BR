---
title: Tipo de recurso ChartDataLabels
description: Representa uma coleção de todos os rótulos de dados em um ponto do gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 502f18fdf03eb28bde4b6f8620bb274f6f2052dd
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47988433"
---
# <a name="chartdatalabels-resource-type"></a><span data-ttu-id="72eaf-103">Tipo de recurso ChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="72eaf-103">ChartDataLabels resource type</span></span>

<span data-ttu-id="72eaf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="72eaf-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="72eaf-105">Representa uma coleção de todos os rótulos de dados em um ponto do gráfico.</span><span class="sxs-lookup"><span data-stu-id="72eaf-105">Represents a collection of all the data labels on a chart point.</span></span>


## <a name="methods"></a><span data-ttu-id="72eaf-106">Methods</span><span class="sxs-lookup"><span data-stu-id="72eaf-106">Methods</span></span>

| <span data-ttu-id="72eaf-107">Método</span><span class="sxs-lookup"><span data-stu-id="72eaf-107">Method</span></span>           | <span data-ttu-id="72eaf-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="72eaf-108">Return Type</span></span>    |<span data-ttu-id="72eaf-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="72eaf-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="72eaf-110">Get ChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="72eaf-110">Get ChartDataLabels</span></span>](../api/chartdatalabels-get.md) | [<span data-ttu-id="72eaf-111">WorkbookChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="72eaf-111">WorkbookChartDataLabels</span></span>](chartdatalabels.md) |<span data-ttu-id="72eaf-112">Leia as propriedades e os relacionamentos do objeto chartDataLabels.</span><span class="sxs-lookup"><span data-stu-id="72eaf-112">Read properties and relationships of chartDataLabels object.</span></span>|
|[<span data-ttu-id="72eaf-113">Update</span><span class="sxs-lookup"><span data-stu-id="72eaf-113">Update</span></span>](../api/chartdatalabels-update.md) | [<span data-ttu-id="72eaf-114">WorkbookChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="72eaf-114">WorkbookChartDataLabels</span></span>](chartdatalabels.md) |<span data-ttu-id="72eaf-115">Atualize o objeto ChartDataLabels.</span><span class="sxs-lookup"><span data-stu-id="72eaf-115">Update ChartDataLabels object.</span></span> |

## <a name="properties"></a><span data-ttu-id="72eaf-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="72eaf-116">Properties</span></span>
| <span data-ttu-id="72eaf-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="72eaf-117">Property</span></span>     | <span data-ttu-id="72eaf-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="72eaf-118">Type</span></span>   |<span data-ttu-id="72eaf-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="72eaf-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="72eaf-120">position</span><span class="sxs-lookup"><span data-stu-id="72eaf-120">position</span></span>|<span data-ttu-id="72eaf-121">string</span><span class="sxs-lookup"><span data-stu-id="72eaf-121">string</span></span>|<span data-ttu-id="72eaf-122">Valor de DataLabelPosition que representa a posição do rótulo de dados.</span><span class="sxs-lookup"><span data-stu-id="72eaf-122">DataLabelPosition value that represents the position of the data label.</span></span> <span data-ttu-id="72eaf-123">Os valores possíveis são: `None` , `Center` , `InsideEnd` , `InsideBase` , `OutsideEnd` , `Left` , `Right` , `Top` , `Bottom` , `BestFit` , `Callout` .</span><span class="sxs-lookup"><span data-stu-id="72eaf-123">The possible values are: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.</span></span>|
|<span data-ttu-id="72eaf-124">separator</span><span class="sxs-lookup"><span data-stu-id="72eaf-124">separator</span></span>|<span data-ttu-id="72eaf-125">string</span><span class="sxs-lookup"><span data-stu-id="72eaf-125">string</span></span>|<span data-ttu-id="72eaf-126">Cadeia de caracteres que representa o separador usado para os rótulos de dados em um gráfico.</span><span class="sxs-lookup"><span data-stu-id="72eaf-126">String representing the separator used for the data labels on a chart.</span></span>|
|<span data-ttu-id="72eaf-127">showBubbleSize</span><span class="sxs-lookup"><span data-stu-id="72eaf-127">showBubbleSize</span></span>|<span data-ttu-id="72eaf-128">booliano</span><span class="sxs-lookup"><span data-stu-id="72eaf-128">boolean</span></span>|<span data-ttu-id="72eaf-129">Valor booliano que determina se o tamanho da bolha do rótulo de dados fica visível ou não.</span><span class="sxs-lookup"><span data-stu-id="72eaf-129">Boolean value representing if the data label bubble size is visible or not.</span></span>|
|<span data-ttu-id="72eaf-130">showCategoryName</span><span class="sxs-lookup"><span data-stu-id="72eaf-130">showCategoryName</span></span>|<span data-ttu-id="72eaf-131">booliano</span><span class="sxs-lookup"><span data-stu-id="72eaf-131">boolean</span></span>|<span data-ttu-id="72eaf-132">Valor booliano que determina se o nome da categoria do rótulo de dados fica visível ou não.</span><span class="sxs-lookup"><span data-stu-id="72eaf-132">Boolean value representing if the data label category name is visible or not.</span></span>|
|<span data-ttu-id="72eaf-133">showLegendKey</span><span class="sxs-lookup"><span data-stu-id="72eaf-133">showLegendKey</span></span>|<span data-ttu-id="72eaf-134">booliano</span><span class="sxs-lookup"><span data-stu-id="72eaf-134">boolean</span></span>|<span data-ttu-id="72eaf-135">Valor booliano que determina se o código de legenda do rótulo de dados fica visível ou não.</span><span class="sxs-lookup"><span data-stu-id="72eaf-135">Boolean value representing if the data label legend key is visible or not.</span></span>|
|<span data-ttu-id="72eaf-136">showPercentage</span><span class="sxs-lookup"><span data-stu-id="72eaf-136">showPercentage</span></span>|<span data-ttu-id="72eaf-137">booliano</span><span class="sxs-lookup"><span data-stu-id="72eaf-137">boolean</span></span>|<span data-ttu-id="72eaf-138">Valor booliano que determina se o percentual do rótulo de dados fica visível ou não.</span><span class="sxs-lookup"><span data-stu-id="72eaf-138">Boolean value representing if the data label percentage is visible or not.</span></span>|
|<span data-ttu-id="72eaf-139">showSeriesName</span><span class="sxs-lookup"><span data-stu-id="72eaf-139">showSeriesName</span></span>|<span data-ttu-id="72eaf-140">booliano</span><span class="sxs-lookup"><span data-stu-id="72eaf-140">boolean</span></span>|<span data-ttu-id="72eaf-141">Valor booliano que determina se o nome da série do rótulo de dados fica visível ou não.</span><span class="sxs-lookup"><span data-stu-id="72eaf-141">Boolean value representing if the data label series name is visible or not.</span></span>|
|<span data-ttu-id="72eaf-142">showValue</span><span class="sxs-lookup"><span data-stu-id="72eaf-142">showValue</span></span>|<span data-ttu-id="72eaf-143">booliano</span><span class="sxs-lookup"><span data-stu-id="72eaf-143">boolean</span></span>|<span data-ttu-id="72eaf-144">Valor booliano que determina se o valor do rótulo de dados fica visível ou não.</span><span class="sxs-lookup"><span data-stu-id="72eaf-144">Boolean value representing if the data label value is visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="72eaf-145">Relações</span><span class="sxs-lookup"><span data-stu-id="72eaf-145">Relationships</span></span>
| <span data-ttu-id="72eaf-146">Relação</span><span class="sxs-lookup"><span data-stu-id="72eaf-146">Relationship</span></span> | <span data-ttu-id="72eaf-147">Tipo</span><span class="sxs-lookup"><span data-stu-id="72eaf-147">Type</span></span>   |<span data-ttu-id="72eaf-148">Descrição</span><span class="sxs-lookup"><span data-stu-id="72eaf-148">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="72eaf-149">formato</span><span class="sxs-lookup"><span data-stu-id="72eaf-149">format</span></span>|[<span data-ttu-id="72eaf-150">WorkbookChartDataLabelFormat</span><span class="sxs-lookup"><span data-stu-id="72eaf-150">WorkbookChartDataLabelFormat</span></span>](chartdatalabelformat.md)|<span data-ttu-id="72eaf-151">Representa o formato dos rótulos de dados do gráfico, que inclui a formatação de fonte e de preenchimento.</span><span class="sxs-lookup"><span data-stu-id="72eaf-151">Represents the format of chart data labels, which includes fill and font formatting.</span></span> <span data-ttu-id="72eaf-152">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="72eaf-152">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="72eaf-153">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="72eaf-153">JSON representation</span></span>

<span data-ttu-id="72eaf-154">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="72eaf-154">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.workbookChartDataLabels"
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
<!-- {
  "type": "#page.annotation",
  "description": "ChartDataLabels resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

