---
title: tipo de recurso workbookChartDataLabels
description: Representa uma coleção de todos os rótulos de dados em um ponto do gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 2e276a3d4e6f958930add9095e8c6c67972bed4f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519341"
---
# <a name="workbookchartdatalabels-resource-type"></a><span data-ttu-id="2820d-103">tipo de recurso workbookChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="2820d-103">workbookChartDataLabels resource type</span></span>

<span data-ttu-id="2820d-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="2820d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2820d-105">Representa uma coleção de todos os rótulos de dados em um ponto do gráfico.</span><span class="sxs-lookup"><span data-stu-id="2820d-105">Represents a collection of all the data labels on a chart point.</span></span>


## <a name="methods"></a><span data-ttu-id="2820d-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="2820d-106">Methods</span></span>

| <span data-ttu-id="2820d-107">Método</span><span class="sxs-lookup"><span data-stu-id="2820d-107">Method</span></span>           | <span data-ttu-id="2820d-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="2820d-108">Return Type</span></span>    |<span data-ttu-id="2820d-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="2820d-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2820d-110">Obter workbookChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="2820d-110">Get workbookChartDataLabels</span></span>](../api/chartdatalabels-get.md) | [<span data-ttu-id="2820d-111">workbookChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="2820d-111">workbookChartDataLabels</span></span>](workbookchartdatalabels.md) |<span data-ttu-id="2820d-112">Leia as propriedades e os relacionamentos do objeto chartDataLabels.</span><span class="sxs-lookup"><span data-stu-id="2820d-112">Read properties and relationships of chartDataLabels object.</span></span>|
|[<span data-ttu-id="2820d-113">Update</span><span class="sxs-lookup"><span data-stu-id="2820d-113">Update</span></span>](../api/chartdatalabels-update.md) | [<span data-ttu-id="2820d-114">workbookChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="2820d-114">workbookChartDataLabels</span></span>](workbookchartdatalabels.md) |<span data-ttu-id="2820d-115">Atualize o objeto ChartDataLabels.</span><span class="sxs-lookup"><span data-stu-id="2820d-115">Update ChartDataLabels object.</span></span> |

## <a name="properties"></a><span data-ttu-id="2820d-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2820d-116">Properties</span></span>
| <span data-ttu-id="2820d-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2820d-117">Property</span></span>     | <span data-ttu-id="2820d-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="2820d-118">Type</span></span>   |<span data-ttu-id="2820d-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="2820d-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2820d-120">position</span><span class="sxs-lookup"><span data-stu-id="2820d-120">position</span></span>|<span data-ttu-id="2820d-121">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2820d-121">string</span></span>|<span data-ttu-id="2820d-122">Valor de DataLabelPosition que representa a posição do rótulo de dados.</span><span class="sxs-lookup"><span data-stu-id="2820d-122">DataLabelPosition value that represents the position of the data label.</span></span> <span data-ttu-id="2820d-123">Os valores possíveis são: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.</span><span class="sxs-lookup"><span data-stu-id="2820d-123">The possible values are: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.</span></span>|
|<span data-ttu-id="2820d-124">separator</span><span class="sxs-lookup"><span data-stu-id="2820d-124">separator</span></span>|<span data-ttu-id="2820d-125">string</span><span class="sxs-lookup"><span data-stu-id="2820d-125">string</span></span>|<span data-ttu-id="2820d-126">Cadeia de caracteres que representa o separador usado para os rótulos de dados em um gráfico.</span><span class="sxs-lookup"><span data-stu-id="2820d-126">String representing the separator used for the data labels on a chart.</span></span>|
|<span data-ttu-id="2820d-127">showBubbleSize</span><span class="sxs-lookup"><span data-stu-id="2820d-127">showBubbleSize</span></span>|<span data-ttu-id="2820d-128">booliano</span><span class="sxs-lookup"><span data-stu-id="2820d-128">boolean</span></span>|<span data-ttu-id="2820d-129">Valor booliano que determina se o tamanho da bolha do rótulo de dados fica visível ou não.</span><span class="sxs-lookup"><span data-stu-id="2820d-129">Boolean value representing if the data label bubble size is visible or not.</span></span>|
|<span data-ttu-id="2820d-130">showCategoryName</span><span class="sxs-lookup"><span data-stu-id="2820d-130">showCategoryName</span></span>|<span data-ttu-id="2820d-131">booliano</span><span class="sxs-lookup"><span data-stu-id="2820d-131">boolean</span></span>|<span data-ttu-id="2820d-132">Valor booliano que determina se o nome da categoria do rótulo de dados fica visível ou não.</span><span class="sxs-lookup"><span data-stu-id="2820d-132">Boolean value representing if the data label category name is visible or not.</span></span>|
|<span data-ttu-id="2820d-133">showLegendKey</span><span class="sxs-lookup"><span data-stu-id="2820d-133">showLegendKey</span></span>|<span data-ttu-id="2820d-134">booliano</span><span class="sxs-lookup"><span data-stu-id="2820d-134">boolean</span></span>|<span data-ttu-id="2820d-135">Valor booliano que determina se o código de legenda do rótulo de dados fica visível ou não.</span><span class="sxs-lookup"><span data-stu-id="2820d-135">Boolean value representing if the data label legend key is visible or not.</span></span>|
|<span data-ttu-id="2820d-136">showPercentage</span><span class="sxs-lookup"><span data-stu-id="2820d-136">showPercentage</span></span>|<span data-ttu-id="2820d-137">booliano</span><span class="sxs-lookup"><span data-stu-id="2820d-137">boolean</span></span>|<span data-ttu-id="2820d-138">Valor booliano que determina se o percentual do rótulo de dados fica visível ou não.</span><span class="sxs-lookup"><span data-stu-id="2820d-138">Boolean value representing if the data label percentage is visible or not.</span></span>|
|<span data-ttu-id="2820d-139">showSeriesName</span><span class="sxs-lookup"><span data-stu-id="2820d-139">showSeriesName</span></span>|<span data-ttu-id="2820d-140">booliano</span><span class="sxs-lookup"><span data-stu-id="2820d-140">boolean</span></span>|<span data-ttu-id="2820d-141">Valor booliano que determina se o nome da série do rótulo de dados fica visível ou não.</span><span class="sxs-lookup"><span data-stu-id="2820d-141">Boolean value representing if the data label series name is visible or not.</span></span>|
|<span data-ttu-id="2820d-142">showValue</span><span class="sxs-lookup"><span data-stu-id="2820d-142">showValue</span></span>|<span data-ttu-id="2820d-143">booliano</span><span class="sxs-lookup"><span data-stu-id="2820d-143">boolean</span></span>|<span data-ttu-id="2820d-144">Valor booliano que determina se o valor do rótulo de dados fica visível ou não.</span><span class="sxs-lookup"><span data-stu-id="2820d-144">Boolean value representing if the data label value is visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2820d-145">Relações</span><span class="sxs-lookup"><span data-stu-id="2820d-145">Relationships</span></span>
| <span data-ttu-id="2820d-146">Relação</span><span class="sxs-lookup"><span data-stu-id="2820d-146">Relationship</span></span> | <span data-ttu-id="2820d-147">Tipo</span><span class="sxs-lookup"><span data-stu-id="2820d-147">Type</span></span>   |<span data-ttu-id="2820d-148">Descrição</span><span class="sxs-lookup"><span data-stu-id="2820d-148">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2820d-149">formato</span><span class="sxs-lookup"><span data-stu-id="2820d-149">format</span></span>|[<span data-ttu-id="2820d-150">workbookChartDataLabelFormat</span><span class="sxs-lookup"><span data-stu-id="2820d-150">workbookChartDataLabelFormat</span></span>](workbookchartdatalabelformat.md)|<span data-ttu-id="2820d-151">Representa o formato dos rótulos de dados do gráfico, que inclui a formatação de fonte e de preenchimento.</span><span class="sxs-lookup"><span data-stu-id="2820d-151">Represents the format of chart data labels, which includes fill and font formatting.</span></span> <span data-ttu-id="2820d-152">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2820d-152">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2820d-153">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2820d-153">JSON representation</span></span>

<span data-ttu-id="2820d-154">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2820d-154">Here is a JSON representation of the resource.</span></span>

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
  "description": "workbookChartDataLabels resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
