---
title: Tipo de recurso ChartDataLabels
description: Representa uma coleção de todos os rótulos de dados em um ponto do gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: f722dccd84d1861ff47e0aa073fe66f50372ad4f
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29576399"
---
# <a name="chartdatalabels-resource-type"></a><span data-ttu-id="5076d-103">Tipo de recurso ChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="5076d-103">ChartDataLabels resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5076d-104">Representa uma coleção de todos os rótulos de dados em um ponto do gráfico.</span><span class="sxs-lookup"><span data-stu-id="5076d-104">Represents a collection of all the data labels on a chart point.</span></span>


## <a name="methods"></a><span data-ttu-id="5076d-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="5076d-105">Methods</span></span>

| <span data-ttu-id="5076d-106">Método</span><span class="sxs-lookup"><span data-stu-id="5076d-106">Method</span></span>           | <span data-ttu-id="5076d-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="5076d-107">Return Type</span></span>    |<span data-ttu-id="5076d-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="5076d-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5076d-109">Get ChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="5076d-109">Get ChartDataLabels</span></span>](../api/chartdatalabels-get.md) | [<span data-ttu-id="5076d-110">WorkbookChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="5076d-110">WorkbookChartDataLabels</span></span>](chartdatalabels.md) |<span data-ttu-id="5076d-111">Leia as propriedades e os relacionamentos do objeto chartDataLabels.</span><span class="sxs-lookup"><span data-stu-id="5076d-111">Read properties and relationships of chartDataLabels object.</span></span>|
|[<span data-ttu-id="5076d-112">Update</span><span class="sxs-lookup"><span data-stu-id="5076d-112">Update</span></span>](../api/chartdatalabels-update.md) | [<span data-ttu-id="5076d-113">WorkbookChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="5076d-113">WorkbookChartDataLabels</span></span>](chartdatalabels.md) |<span data-ttu-id="5076d-114">Atualize o objeto ChartDataLabels.</span><span class="sxs-lookup"><span data-stu-id="5076d-114">Update ChartDataLabels object.</span></span> |

## <a name="properties"></a><span data-ttu-id="5076d-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5076d-115">Properties</span></span>
| <span data-ttu-id="5076d-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5076d-116">Property</span></span>     | <span data-ttu-id="5076d-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="5076d-117">Type</span></span>   |<span data-ttu-id="5076d-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="5076d-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5076d-119">position</span><span class="sxs-lookup"><span data-stu-id="5076d-119">position</span></span>|<span data-ttu-id="5076d-120">string</span><span class="sxs-lookup"><span data-stu-id="5076d-120">string</span></span>|<span data-ttu-id="5076d-121">Valor de DataLabelPosition que representa a posição do rótulo de dados.</span><span class="sxs-lookup"><span data-stu-id="5076d-121">DataLabelPosition value that represents the position of the data label.</span></span> <span data-ttu-id="5076d-122">Os valores possíveis são: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.</span><span class="sxs-lookup"><span data-stu-id="5076d-122">The possible values are: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.</span></span>|
|<span data-ttu-id="5076d-123">separador</span><span class="sxs-lookup"><span data-stu-id="5076d-123">separator</span></span>|<span data-ttu-id="5076d-124">string</span><span class="sxs-lookup"><span data-stu-id="5076d-124">string</span></span>|<span data-ttu-id="5076d-125">Cadeia de caracteres que representa o separador usado para os rótulos de dados em um gráfico.</span><span class="sxs-lookup"><span data-stu-id="5076d-125">String representing the separator used for the data labels on a chart.</span></span>|
|<span data-ttu-id="5076d-126">showBubbleSize</span><span class="sxs-lookup"><span data-stu-id="5076d-126">showBubbleSize</span></span>|<span data-ttu-id="5076d-127">booliano</span><span class="sxs-lookup"><span data-stu-id="5076d-127">boolean</span></span>|<span data-ttu-id="5076d-128">Valor booliano que determina se o tamanho da bolha do rótulo de dados fica visível ou não.</span><span class="sxs-lookup"><span data-stu-id="5076d-128">Boolean value representing if the data label bubble size is visible or not.</span></span>|
|<span data-ttu-id="5076d-129">showCategoryName</span><span class="sxs-lookup"><span data-stu-id="5076d-129">showCategoryName</span></span>|<span data-ttu-id="5076d-130">booliano</span><span class="sxs-lookup"><span data-stu-id="5076d-130">boolean</span></span>|<span data-ttu-id="5076d-131">Valor booliano que determina se o nome da categoria do rótulo de dados fica visível ou não.</span><span class="sxs-lookup"><span data-stu-id="5076d-131">Boolean value representing if the data label category name is visible or not.</span></span>|
|<span data-ttu-id="5076d-132">showLegendKey</span><span class="sxs-lookup"><span data-stu-id="5076d-132">showLegendKey</span></span>|<span data-ttu-id="5076d-133">booliano</span><span class="sxs-lookup"><span data-stu-id="5076d-133">boolean</span></span>|<span data-ttu-id="5076d-134">Valor booliano que determina se o código de legenda do rótulo de dados fica visível ou não.</span><span class="sxs-lookup"><span data-stu-id="5076d-134">Boolean value representing if the data label legend key is visible or not.</span></span>|
|<span data-ttu-id="5076d-135">showPercentage</span><span class="sxs-lookup"><span data-stu-id="5076d-135">showPercentage</span></span>|<span data-ttu-id="5076d-136">booliano</span><span class="sxs-lookup"><span data-stu-id="5076d-136">boolean</span></span>|<span data-ttu-id="5076d-137">Valor booliano que determina se o percentual do rótulo de dados fica visível ou não.</span><span class="sxs-lookup"><span data-stu-id="5076d-137">Boolean value representing if the data label percentage is visible or not.</span></span>|
|<span data-ttu-id="5076d-138">showSeriesName</span><span class="sxs-lookup"><span data-stu-id="5076d-138">showSeriesName</span></span>|<span data-ttu-id="5076d-139">booliano</span><span class="sxs-lookup"><span data-stu-id="5076d-139">boolean</span></span>|<span data-ttu-id="5076d-140">Valor booliano que determina se o nome da série do rótulo de dados fica visível ou não.</span><span class="sxs-lookup"><span data-stu-id="5076d-140">Boolean value representing if the data label series name is visible or not.</span></span>|
|<span data-ttu-id="5076d-141">showValue</span><span class="sxs-lookup"><span data-stu-id="5076d-141">showValue</span></span>|<span data-ttu-id="5076d-142">booliano</span><span class="sxs-lookup"><span data-stu-id="5076d-142">boolean</span></span>|<span data-ttu-id="5076d-143">Valor booliano que determina se o valor do rótulo de dados fica visível ou não.</span><span class="sxs-lookup"><span data-stu-id="5076d-143">Boolean value representing if the data label value is visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5076d-144">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="5076d-144">Relationships</span></span>
| <span data-ttu-id="5076d-145">Relação</span><span class="sxs-lookup"><span data-stu-id="5076d-145">Relationship</span></span> | <span data-ttu-id="5076d-146">Tipo</span><span class="sxs-lookup"><span data-stu-id="5076d-146">Type</span></span>   |<span data-ttu-id="5076d-147">Descrição</span><span class="sxs-lookup"><span data-stu-id="5076d-147">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5076d-148">formato</span><span class="sxs-lookup"><span data-stu-id="5076d-148">format</span></span>|[<span data-ttu-id="5076d-149">WorkbookChartDataLabelFormat</span><span class="sxs-lookup"><span data-stu-id="5076d-149">WorkbookChartDataLabelFormat</span></span>](chartdatalabelformat.md)|<span data-ttu-id="5076d-p102">Representa o formato dos rótulos de dados do gráfico, que inclui a formatação de fonte e de preenchimento. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5076d-p102">Represents the format of chart data labels, which includes fill and font formatting. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5076d-152">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5076d-152">JSON representation</span></span>

<span data-ttu-id="5076d-153">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5076d-153">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "ChartDataLabels resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chartdatalabels.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
