---
title: Tipo de recurso ChartDataLabels
description: Representa uma coleção de todos os rótulos de dados em um ponto do gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: bda2c1849f154435608f311671026e224b0c7e3c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510334"
---
# <a name="chartdatalabels-resource-type"></a><span data-ttu-id="04426-103">Tipo de recurso ChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="04426-103">ChartDataLabels resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="04426-104">Representa uma coleção de todos os rótulos de dados em um ponto do gráfico.</span><span class="sxs-lookup"><span data-stu-id="04426-104">Represents a collection of all the data labels on a chart point.</span></span>


## <a name="methods"></a><span data-ttu-id="04426-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="04426-105">Methods</span></span>

| <span data-ttu-id="04426-106">Método</span><span class="sxs-lookup"><span data-stu-id="04426-106">Method</span></span>           | <span data-ttu-id="04426-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="04426-107">Return Type</span></span>    |<span data-ttu-id="04426-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="04426-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="04426-109">Get ChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="04426-109">[Get ChartDataLabels](../api/chartdatalabels-get.md)</span></span> | [<span data-ttu-id="04426-110">chartDataLabels</span><span class="sxs-lookup"><span data-stu-id="04426-110">ChartDataLabels</span></span>](chartdatalabels.md) |<span data-ttu-id="04426-111">Leia as propriedades e os relacionamentos do objeto chartDataLabels.</span><span class="sxs-lookup"><span data-stu-id="04426-111">Read properties and relationships of chartDataLabels object.</span></span>|
|[<span data-ttu-id="04426-112">Update</span><span class="sxs-lookup"><span data-stu-id="04426-112">Update</span></span>](../api/chartdatalabels-update.md) | <span data-ttu-id="04426-113">ChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="04426-113">[ChartDataLabels](chartdatalabels.md)</span></span> |<span data-ttu-id="04426-114">Atualize o objeto ChartDataLabels.</span><span class="sxs-lookup"><span data-stu-id="04426-114">Update ChartDataLabels object.</span></span> |

## <a name="properties"></a><span data-ttu-id="04426-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="04426-115">Properties</span></span>
| <span data-ttu-id="04426-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="04426-116">Property</span></span>     | <span data-ttu-id="04426-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="04426-117">Type</span></span>   |<span data-ttu-id="04426-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="04426-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="04426-119">position</span><span class="sxs-lookup"><span data-stu-id="04426-119">position</span></span>|<span data-ttu-id="04426-120">string</span><span class="sxs-lookup"><span data-stu-id="04426-120">string</span></span>|<span data-ttu-id="04426-p101">Valor de DataLabelPosition que representa a posição do rótulo de dados. Os valores possíveis são: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit` e `Callout`.</span><span class="sxs-lookup"><span data-stu-id="04426-p101">DataLabelPosition value that represents the position of the data label. Possible values are: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.</span></span>|
|<span data-ttu-id="04426-123">separador</span><span class="sxs-lookup"><span data-stu-id="04426-123">separator</span></span>|<span data-ttu-id="04426-124">string</span><span class="sxs-lookup"><span data-stu-id="04426-124">string</span></span>|<span data-ttu-id="04426-125">Cadeia de caracteres que representa o separador usado para os rótulos de dados em um gráfico.</span><span class="sxs-lookup"><span data-stu-id="04426-125">String representing the separator used for the data labels on a chart.</span></span>|
|<span data-ttu-id="04426-126">showBubbleSize</span><span class="sxs-lookup"><span data-stu-id="04426-126">showBubbleSize</span></span>|<span data-ttu-id="04426-127">booliano</span><span class="sxs-lookup"><span data-stu-id="04426-127">boolean</span></span>|<span data-ttu-id="04426-128">Valor booliano que determina se o tamanho da bolha do rótulo de dados fica visível ou não.</span><span class="sxs-lookup"><span data-stu-id="04426-128">Boolean value representing if the data label bubble size is visible or not.</span></span>|
|<span data-ttu-id="04426-129">showCategoryName</span><span class="sxs-lookup"><span data-stu-id="04426-129">showCategoryName</span></span>|<span data-ttu-id="04426-130">booliano</span><span class="sxs-lookup"><span data-stu-id="04426-130">boolean</span></span>|<span data-ttu-id="04426-131">Valor booliano que determina se o nome da categoria do rótulo de dados fica visível ou não.</span><span class="sxs-lookup"><span data-stu-id="04426-131">Boolean value representing if the data label category name is visible or not.</span></span>|
|<span data-ttu-id="04426-132">showLegendKey</span><span class="sxs-lookup"><span data-stu-id="04426-132">showLegendKey</span></span>|<span data-ttu-id="04426-133">booliano</span><span class="sxs-lookup"><span data-stu-id="04426-133">boolean</span></span>|<span data-ttu-id="04426-134">Valor booliano que determina se o código de legenda do rótulo de dados fica visível ou não.</span><span class="sxs-lookup"><span data-stu-id="04426-134">Boolean value representing if the data label legend key is visible or not.</span></span>|
|<span data-ttu-id="04426-135">showPercentage</span><span class="sxs-lookup"><span data-stu-id="04426-135">showPercentage</span></span>|<span data-ttu-id="04426-136">booliano</span><span class="sxs-lookup"><span data-stu-id="04426-136">boolean</span></span>|<span data-ttu-id="04426-137">Valor booliano que determina se o percentual do rótulo de dados fica visível ou não.</span><span class="sxs-lookup"><span data-stu-id="04426-137">Boolean value representing if the data label percentage is visible or not.</span></span>|
|<span data-ttu-id="04426-138">showSeriesName</span><span class="sxs-lookup"><span data-stu-id="04426-138">showSeriesName</span></span>|<span data-ttu-id="04426-139">booliano</span><span class="sxs-lookup"><span data-stu-id="04426-139">boolean</span></span>|<span data-ttu-id="04426-140">Valor booliano que determina se o nome da série do rótulo de dados fica visível ou não.</span><span class="sxs-lookup"><span data-stu-id="04426-140">Boolean value representing if the data label series name is visible or not.</span></span>|
|<span data-ttu-id="04426-141">showValue</span><span class="sxs-lookup"><span data-stu-id="04426-141">showValue</span></span>|<span data-ttu-id="04426-142">booliano</span><span class="sxs-lookup"><span data-stu-id="04426-142">boolean</span></span>|<span data-ttu-id="04426-143">Valor booliano que determina se o valor do rótulo de dados fica visível ou não.</span><span class="sxs-lookup"><span data-stu-id="04426-143">Boolean value representing if the data label value is visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="04426-144">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="04426-144">Relationships</span></span>
| <span data-ttu-id="04426-145">Relação</span><span class="sxs-lookup"><span data-stu-id="04426-145">Relationship</span></span> | <span data-ttu-id="04426-146">Tipo</span><span class="sxs-lookup"><span data-stu-id="04426-146">Type</span></span>   |<span data-ttu-id="04426-147">Descrição</span><span class="sxs-lookup"><span data-stu-id="04426-147">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="04426-148">formato</span><span class="sxs-lookup"><span data-stu-id="04426-148">format</span></span>|[<span data-ttu-id="04426-149">ChartDataLabelFormat</span><span class="sxs-lookup"><span data-stu-id="04426-149">ChartDataLabelFormat</span></span>](chartdatalabelformat.md)|<span data-ttu-id="04426-p102">Representa o formato dos rótulos de dados do gráfico, que inclui a formatação de fonte e de preenchimento. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="04426-p102">Represents the format of chart data labels, which includes fill and font formatting. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="04426-152">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="04426-152">JSON representation</span></span>

<span data-ttu-id="04426-153">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="04426-153">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartDataLabels"
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
