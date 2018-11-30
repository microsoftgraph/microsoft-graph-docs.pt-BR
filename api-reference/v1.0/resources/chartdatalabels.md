---
title: Tipo de recurso ChartDataLabels
description: Representa uma coleção de todos os rótulos de dados em um ponto do gráfico.
ms.openlocfilehash: f8cb4310ab9ca2e59325fbc4bd255ae161cc7892
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27003768"
---
# <a name="chartdatalabels-resource-type"></a><span data-ttu-id="2f825-103">Tipo de recurso ChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="2f825-103">ChartDataLabels resource type</span></span>

<span data-ttu-id="2f825-104">Representa uma coleção de todos os rótulos de dados em um ponto do gráfico.</span><span class="sxs-lookup"><span data-stu-id="2f825-104">Represents a collection of all the data labels on a chart point.</span></span>


## <a name="methods"></a><span data-ttu-id="2f825-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="2f825-105">Methods</span></span>

| <span data-ttu-id="2f825-106">Método</span><span class="sxs-lookup"><span data-stu-id="2f825-106">Method</span></span>           | <span data-ttu-id="2f825-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="2f825-107">Return Type</span></span>    |<span data-ttu-id="2f825-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="2f825-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2f825-109">Get ChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="2f825-109">Get ChartDataLabels</span></span>](../api/chartdatalabels-get.md) | [<span data-ttu-id="2f825-110">WorkbookChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="2f825-110">WorkbookChartDataLabels</span></span>](chartdatalabels.md) |<span data-ttu-id="2f825-111">Leia as propriedades e os relacionamentos do objeto chartDataLabels.</span><span class="sxs-lookup"><span data-stu-id="2f825-111">Read properties and relationships of chartDataLabels object.</span></span>|
|[<span data-ttu-id="2f825-112">Update</span><span class="sxs-lookup"><span data-stu-id="2f825-112">Update</span></span>](../api/chartdatalabels-update.md) | [<span data-ttu-id="2f825-113">WorkbookChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="2f825-113">WorkbookChartDataLabels</span></span>](chartdatalabels.md) |<span data-ttu-id="2f825-114">Atualize o objeto ChartDataLabels.</span><span class="sxs-lookup"><span data-stu-id="2f825-114">Update ChartDataLabels object.</span></span> |

## <a name="properties"></a><span data-ttu-id="2f825-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2f825-115">Properties</span></span>
| <span data-ttu-id="2f825-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2f825-116">Property</span></span>     | <span data-ttu-id="2f825-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="2f825-117">Type</span></span>   |<span data-ttu-id="2f825-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="2f825-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2f825-119">position</span><span class="sxs-lookup"><span data-stu-id="2f825-119">position</span></span>|<span data-ttu-id="2f825-120">string</span><span class="sxs-lookup"><span data-stu-id="2f825-120">string</span></span>|<span data-ttu-id="2f825-121">Valor de DataLabelPosition que representa a posição do rótulo de dados.</span><span class="sxs-lookup"><span data-stu-id="2f825-121">DataLabelPosition value that represents the position of the data label.</span></span> <span data-ttu-id="2f825-122">Os valores possíveis são: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.</span><span class="sxs-lookup"><span data-stu-id="2f825-122">The possible values are: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.</span></span>|
|<span data-ttu-id="2f825-123">separador</span><span class="sxs-lookup"><span data-stu-id="2f825-123">separator</span></span>|<span data-ttu-id="2f825-124">string</span><span class="sxs-lookup"><span data-stu-id="2f825-124">string</span></span>|<span data-ttu-id="2f825-125">Cadeia de caracteres que representa o separador usado para os rótulos de dados em um gráfico.</span><span class="sxs-lookup"><span data-stu-id="2f825-125">String representing the separator used for the data labels on a chart.</span></span>|
|<span data-ttu-id="2f825-126">showBubbleSize</span><span class="sxs-lookup"><span data-stu-id="2f825-126">showBubbleSize</span></span>|<span data-ttu-id="2f825-127">booliano</span><span class="sxs-lookup"><span data-stu-id="2f825-127">boolean</span></span>|<span data-ttu-id="2f825-128">Valor booliano que determina se o tamanho da bolha do rótulo de dados fica visível ou não.</span><span class="sxs-lookup"><span data-stu-id="2f825-128">Boolean value representing if the data label bubble size is visible or not.</span></span>|
|<span data-ttu-id="2f825-129">showCategoryName</span><span class="sxs-lookup"><span data-stu-id="2f825-129">showCategoryName</span></span>|<span data-ttu-id="2f825-130">booliano</span><span class="sxs-lookup"><span data-stu-id="2f825-130">boolean</span></span>|<span data-ttu-id="2f825-131">Valor booliano que determina se o nome da categoria do rótulo de dados fica visível ou não.</span><span class="sxs-lookup"><span data-stu-id="2f825-131">Boolean value representing if the data label category name is visible or not.</span></span>|
|<span data-ttu-id="2f825-132">showLegendKey</span><span class="sxs-lookup"><span data-stu-id="2f825-132">showLegendKey</span></span>|<span data-ttu-id="2f825-133">booliano</span><span class="sxs-lookup"><span data-stu-id="2f825-133">boolean</span></span>|<span data-ttu-id="2f825-134">Valor booliano que determina se o código de legenda do rótulo de dados fica visível ou não.</span><span class="sxs-lookup"><span data-stu-id="2f825-134">Boolean value representing if the data label legend key is visible or not.</span></span>|
|<span data-ttu-id="2f825-135">showPercentage</span><span class="sxs-lookup"><span data-stu-id="2f825-135">showPercentage</span></span>|<span data-ttu-id="2f825-136">booliano</span><span class="sxs-lookup"><span data-stu-id="2f825-136">boolean</span></span>|<span data-ttu-id="2f825-137">Valor booliano que determina se o percentual do rótulo de dados fica visível ou não.</span><span class="sxs-lookup"><span data-stu-id="2f825-137">Boolean value representing if the data label percentage is visible or not.</span></span>|
|<span data-ttu-id="2f825-138">showSeriesName</span><span class="sxs-lookup"><span data-stu-id="2f825-138">showSeriesName</span></span>|<span data-ttu-id="2f825-139">booliano</span><span class="sxs-lookup"><span data-stu-id="2f825-139">boolean</span></span>|<span data-ttu-id="2f825-140">Valor booliano que determina se o nome da série do rótulo de dados fica visível ou não.</span><span class="sxs-lookup"><span data-stu-id="2f825-140">Boolean value representing if the data label series name is visible or not.</span></span>|
|<span data-ttu-id="2f825-141">showValue</span><span class="sxs-lookup"><span data-stu-id="2f825-141">showValue</span></span>|<span data-ttu-id="2f825-142">booliano</span><span class="sxs-lookup"><span data-stu-id="2f825-142">boolean</span></span>|<span data-ttu-id="2f825-143">Valor booliano que determina se o valor do rótulo de dados fica visível ou não.</span><span class="sxs-lookup"><span data-stu-id="2f825-143">Boolean value representing if the data label value is visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2f825-144">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="2f825-144">Relationships</span></span>
| <span data-ttu-id="2f825-145">Relação</span><span class="sxs-lookup"><span data-stu-id="2f825-145">Relationship</span></span> | <span data-ttu-id="2f825-146">Tipo</span><span class="sxs-lookup"><span data-stu-id="2f825-146">Type</span></span>   |<span data-ttu-id="2f825-147">Descrição</span><span class="sxs-lookup"><span data-stu-id="2f825-147">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2f825-148">formato</span><span class="sxs-lookup"><span data-stu-id="2f825-148">format</span></span>|[<span data-ttu-id="2f825-149">WorkbookChartDataLabelFormat</span><span class="sxs-lookup"><span data-stu-id="2f825-149">WorkbookChartDataLabelFormat</span></span>](chartdatalabelformat.md)|<span data-ttu-id="2f825-p102">Representa o formato dos rótulos de dados do gráfico, que inclui a formatação de fonte e de preenchimento. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2f825-p102">Represents the format of chart data labels, which includes fill and font formatting. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2f825-152">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2f825-152">JSON representation</span></span>

<span data-ttu-id="2f825-153">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2f825-153">Here is a JSON representation of the resource.</span></span>

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