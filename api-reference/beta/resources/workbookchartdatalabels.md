---
title: tipo de recurso workbookChartDataLabels
description: Representa uma coleção de todos os rótulos de dados em um ponto do gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 9c3521274b93d33780539c04643c5c0225fdecef
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348456"
---
# <a name="workbookchartdatalabels-resource-type"></a><span data-ttu-id="fae6c-103">tipo de recurso workbookChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="fae6c-103">workbookChartDataLabels resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fae6c-104">Representa uma coleção de todos os rótulos de dados em um ponto do gráfico.</span><span class="sxs-lookup"><span data-stu-id="fae6c-104">Represents a collection of all the data labels on a chart point.</span></span>


## <a name="methods"></a><span data-ttu-id="fae6c-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="fae6c-105">Methods</span></span>

| <span data-ttu-id="fae6c-106">Método</span><span class="sxs-lookup"><span data-stu-id="fae6c-106">Method</span></span>           | <span data-ttu-id="fae6c-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="fae6c-107">Return Type</span></span>    |<span data-ttu-id="fae6c-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="fae6c-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="fae6c-109">Obter workbookChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="fae6c-109">Get workbookChartDataLabels</span></span>](../api/chartdatalabels-get.md) | [<span data-ttu-id="fae6c-110">workbookChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="fae6c-110">workbookChartDataLabels</span></span>](workbookchartdatalabels.md) |<span data-ttu-id="fae6c-111">Leia as propriedades e os relacionamentos do objeto chartDataLabels.</span><span class="sxs-lookup"><span data-stu-id="fae6c-111">Read properties and relationships of chartDataLabels object.</span></span>|
|[<span data-ttu-id="fae6c-112">Update</span><span class="sxs-lookup"><span data-stu-id="fae6c-112">Update</span></span>](../api/chartdatalabels-update.md) | [<span data-ttu-id="fae6c-113">workbookChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="fae6c-113">workbookChartDataLabels</span></span>](workbookchartdatalabels.md) |<span data-ttu-id="fae6c-114">Atualize o objeto ChartDataLabels.</span><span class="sxs-lookup"><span data-stu-id="fae6c-114">Update ChartDataLabels object.</span></span> |

## <a name="properties"></a><span data-ttu-id="fae6c-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fae6c-115">Properties</span></span>
| <span data-ttu-id="fae6c-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fae6c-116">Property</span></span>     | <span data-ttu-id="fae6c-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="fae6c-117">Type</span></span>   |<span data-ttu-id="fae6c-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="fae6c-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fae6c-119">position</span><span class="sxs-lookup"><span data-stu-id="fae6c-119">position</span></span>|<span data-ttu-id="fae6c-120">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fae6c-120">string</span></span>|<span data-ttu-id="fae6c-121">Valor de DataLabelPosition que representa a posição do rótulo de dados.</span><span class="sxs-lookup"><span data-stu-id="fae6c-121">DataLabelPosition value that represents the position of the data label.</span></span> <span data-ttu-id="fae6c-122">Os valores possíveis são: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.</span><span class="sxs-lookup"><span data-stu-id="fae6c-122">The possible values are: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.</span></span>|
|<span data-ttu-id="fae6c-123">separator</span><span class="sxs-lookup"><span data-stu-id="fae6c-123">separator</span></span>|<span data-ttu-id="fae6c-124">string</span><span class="sxs-lookup"><span data-stu-id="fae6c-124">string</span></span>|<span data-ttu-id="fae6c-125">Cadeia de caracteres que representa o separador usado para os rótulos de dados em um gráfico.</span><span class="sxs-lookup"><span data-stu-id="fae6c-125">String representing the separator used for the data labels on a chart.</span></span>|
|<span data-ttu-id="fae6c-126">showBubbleSize</span><span class="sxs-lookup"><span data-stu-id="fae6c-126">showBubbleSize</span></span>|<span data-ttu-id="fae6c-127">booliano</span><span class="sxs-lookup"><span data-stu-id="fae6c-127">boolean</span></span>|<span data-ttu-id="fae6c-128">Valor booliano que determina se o tamanho da bolha do rótulo de dados fica visível ou não.</span><span class="sxs-lookup"><span data-stu-id="fae6c-128">Boolean value representing if the data label bubble size is visible or not.</span></span>|
|<span data-ttu-id="fae6c-129">showCategoryName</span><span class="sxs-lookup"><span data-stu-id="fae6c-129">showCategoryName</span></span>|<span data-ttu-id="fae6c-130">booliano</span><span class="sxs-lookup"><span data-stu-id="fae6c-130">boolean</span></span>|<span data-ttu-id="fae6c-131">Valor booliano que determina se o nome da categoria do rótulo de dados fica visível ou não.</span><span class="sxs-lookup"><span data-stu-id="fae6c-131">Boolean value representing if the data label category name is visible or not.</span></span>|
|<span data-ttu-id="fae6c-132">showLegendKey</span><span class="sxs-lookup"><span data-stu-id="fae6c-132">showLegendKey</span></span>|<span data-ttu-id="fae6c-133">booliano</span><span class="sxs-lookup"><span data-stu-id="fae6c-133">boolean</span></span>|<span data-ttu-id="fae6c-134">Valor booliano que determina se o código de legenda do rótulo de dados fica visível ou não.</span><span class="sxs-lookup"><span data-stu-id="fae6c-134">Boolean value representing if the data label legend key is visible or not.</span></span>|
|<span data-ttu-id="fae6c-135">showPercentage</span><span class="sxs-lookup"><span data-stu-id="fae6c-135">showPercentage</span></span>|<span data-ttu-id="fae6c-136">booliano</span><span class="sxs-lookup"><span data-stu-id="fae6c-136">boolean</span></span>|<span data-ttu-id="fae6c-137">Valor booliano que determina se o percentual do rótulo de dados fica visível ou não.</span><span class="sxs-lookup"><span data-stu-id="fae6c-137">Boolean value representing if the data label percentage is visible or not.</span></span>|
|<span data-ttu-id="fae6c-138">showSeriesName</span><span class="sxs-lookup"><span data-stu-id="fae6c-138">showSeriesName</span></span>|<span data-ttu-id="fae6c-139">booliano</span><span class="sxs-lookup"><span data-stu-id="fae6c-139">boolean</span></span>|<span data-ttu-id="fae6c-140">Valor booliano que determina se o nome da série do rótulo de dados fica visível ou não.</span><span class="sxs-lookup"><span data-stu-id="fae6c-140">Boolean value representing if the data label series name is visible or not.</span></span>|
|<span data-ttu-id="fae6c-141">showValue</span><span class="sxs-lookup"><span data-stu-id="fae6c-141">showValue</span></span>|<span data-ttu-id="fae6c-142">booliano</span><span class="sxs-lookup"><span data-stu-id="fae6c-142">boolean</span></span>|<span data-ttu-id="fae6c-143">Valor booliano que determina se o valor do rótulo de dados fica visível ou não.</span><span class="sxs-lookup"><span data-stu-id="fae6c-143">Boolean value representing if the data label value is visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fae6c-144">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="fae6c-144">Relationships</span></span>
| <span data-ttu-id="fae6c-145">Relação</span><span class="sxs-lookup"><span data-stu-id="fae6c-145">Relationship</span></span> | <span data-ttu-id="fae6c-146">Tipo</span><span class="sxs-lookup"><span data-stu-id="fae6c-146">Type</span></span>   |<span data-ttu-id="fae6c-147">Descrição</span><span class="sxs-lookup"><span data-stu-id="fae6c-147">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fae6c-148">formato</span><span class="sxs-lookup"><span data-stu-id="fae6c-148">format</span></span>|[<span data-ttu-id="fae6c-149">workbookChartDataLabelFormat</span><span class="sxs-lookup"><span data-stu-id="fae6c-149">workbookChartDataLabelFormat</span></span>](workbookchartdatalabelformat.md)|<span data-ttu-id="fae6c-150">Representa o formato dos rótulos de dados do gráfico, que inclui a formatação de fonte e de preenchimento.</span><span class="sxs-lookup"><span data-stu-id="fae6c-150">Represents the format of chart data labels, which includes fill and font formatting.</span></span> <span data-ttu-id="fae6c-151">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fae6c-151">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fae6c-152">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fae6c-152">JSON representation</span></span>

<span data-ttu-id="fae6c-153">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fae6c-153">Here is a JSON representation of the resource.</span></span>

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
