---
title: Tipo de recurso ChartDataLabels
description: Representa uma coleção de todos os rótulos de dados em um ponto do gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 16e2e3acafc98a4066b8620f41f15c7cae1667cc
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27954677"
---
# <a name="chartdatalabels-resource-type"></a><span data-ttu-id="61447-103">Tipo de recurso ChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="61447-103">ChartDataLabels resource type</span></span>

> <span data-ttu-id="61447-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="61447-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="61447-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="61447-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="61447-106">Representa uma coleção de todos os rótulos de dados em um ponto do gráfico.</span><span class="sxs-lookup"><span data-stu-id="61447-106">Represents a collection of all the data labels on a chart point.</span></span>


## <a name="methods"></a><span data-ttu-id="61447-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="61447-107">Methods</span></span>

| <span data-ttu-id="61447-108">Método</span><span class="sxs-lookup"><span data-stu-id="61447-108">Method</span></span>           | <span data-ttu-id="61447-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="61447-109">Return Type</span></span>    |<span data-ttu-id="61447-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="61447-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="61447-111">Get ChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="61447-111">Get ChartDataLabels</span></span>](../api/chartdatalabels-get.md) | [<span data-ttu-id="61447-112">ChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="61447-112">ChartDataLabels</span></span>](chartdatalabels.md) |<span data-ttu-id="61447-113">Leia as propriedades e os relacionamentos do objeto chartDataLabels.</span><span class="sxs-lookup"><span data-stu-id="61447-113">Read properties and relationships of chartDataLabels object.</span></span>|
|[<span data-ttu-id="61447-114">Update</span><span class="sxs-lookup"><span data-stu-id="61447-114">Update</span></span>](../api/chartdatalabels-update.md) | [<span data-ttu-id="61447-115">ChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="61447-115">ChartDataLabels</span></span>](chartdatalabels.md) |<span data-ttu-id="61447-116">Atualize o objeto ChartDataLabels.</span><span class="sxs-lookup"><span data-stu-id="61447-116">Update ChartDataLabels object.</span></span> |

## <a name="properties"></a><span data-ttu-id="61447-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="61447-117">Properties</span></span>
| <span data-ttu-id="61447-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="61447-118">Property</span></span>     | <span data-ttu-id="61447-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="61447-119">Type</span></span>   |<span data-ttu-id="61447-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="61447-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="61447-121">position</span><span class="sxs-lookup"><span data-stu-id="61447-121">position</span></span>|<span data-ttu-id="61447-122">string</span><span class="sxs-lookup"><span data-stu-id="61447-122">string</span></span>|<span data-ttu-id="61447-p102">Valor de DataLabelPosition que representa a posição do rótulo de dados. Os valores possíveis são: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit` e `Callout`.</span><span class="sxs-lookup"><span data-stu-id="61447-p102">DataLabelPosition value that represents the position of the data label. Possible values are: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.</span></span>|
|<span data-ttu-id="61447-125">separador</span><span class="sxs-lookup"><span data-stu-id="61447-125">separator</span></span>|<span data-ttu-id="61447-126">string</span><span class="sxs-lookup"><span data-stu-id="61447-126">string</span></span>|<span data-ttu-id="61447-127">Cadeia de caracteres que representa o separador usado para os rótulos de dados em um gráfico.</span><span class="sxs-lookup"><span data-stu-id="61447-127">String representing the separator used for the data labels on a chart.</span></span>|
|<span data-ttu-id="61447-128">showBubbleSize</span><span class="sxs-lookup"><span data-stu-id="61447-128">showBubbleSize</span></span>|<span data-ttu-id="61447-129">booliano</span><span class="sxs-lookup"><span data-stu-id="61447-129">boolean</span></span>|<span data-ttu-id="61447-130">Valor booliano que determina se o tamanho da bolha do rótulo de dados fica visível ou não.</span><span class="sxs-lookup"><span data-stu-id="61447-130">Boolean value representing if the data label bubble size is visible or not.</span></span>|
|<span data-ttu-id="61447-131">showCategoryName</span><span class="sxs-lookup"><span data-stu-id="61447-131">showCategoryName</span></span>|<span data-ttu-id="61447-132">booliano</span><span class="sxs-lookup"><span data-stu-id="61447-132">boolean</span></span>|<span data-ttu-id="61447-133">Valor booliano que determina se o nome da categoria do rótulo de dados fica visível ou não.</span><span class="sxs-lookup"><span data-stu-id="61447-133">Boolean value representing if the data label category name is visible or not.</span></span>|
|<span data-ttu-id="61447-134">showLegendKey</span><span class="sxs-lookup"><span data-stu-id="61447-134">showLegendKey</span></span>|<span data-ttu-id="61447-135">booliano</span><span class="sxs-lookup"><span data-stu-id="61447-135">boolean</span></span>|<span data-ttu-id="61447-136">Valor booliano que determina se o código de legenda do rótulo de dados fica visível ou não.</span><span class="sxs-lookup"><span data-stu-id="61447-136">Boolean value representing if the data label legend key is visible or not.</span></span>|
|<span data-ttu-id="61447-137">showPercentage</span><span class="sxs-lookup"><span data-stu-id="61447-137">showPercentage</span></span>|<span data-ttu-id="61447-138">booliano</span><span class="sxs-lookup"><span data-stu-id="61447-138">boolean</span></span>|<span data-ttu-id="61447-139">Valor booliano que determina se o percentual do rótulo de dados fica visível ou não.</span><span class="sxs-lookup"><span data-stu-id="61447-139">Boolean value representing if the data label percentage is visible or not.</span></span>|
|<span data-ttu-id="61447-140">showSeriesName</span><span class="sxs-lookup"><span data-stu-id="61447-140">showSeriesName</span></span>|<span data-ttu-id="61447-141">booliano</span><span class="sxs-lookup"><span data-stu-id="61447-141">boolean</span></span>|<span data-ttu-id="61447-142">Valor booliano que determina se o nome da série do rótulo de dados fica visível ou não.</span><span class="sxs-lookup"><span data-stu-id="61447-142">Boolean value representing if the data label series name is visible or not.</span></span>|
|<span data-ttu-id="61447-143">showValue</span><span class="sxs-lookup"><span data-stu-id="61447-143">showValue</span></span>|<span data-ttu-id="61447-144">booliano</span><span class="sxs-lookup"><span data-stu-id="61447-144">boolean</span></span>|<span data-ttu-id="61447-145">Valor booliano que determina se o valor do rótulo de dados fica visível ou não.</span><span class="sxs-lookup"><span data-stu-id="61447-145">Boolean value representing if the data label value is visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="61447-146">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="61447-146">Relationships</span></span>
| <span data-ttu-id="61447-147">Relação</span><span class="sxs-lookup"><span data-stu-id="61447-147">Relationship</span></span> | <span data-ttu-id="61447-148">Tipo</span><span class="sxs-lookup"><span data-stu-id="61447-148">Type</span></span>   |<span data-ttu-id="61447-149">Descrição</span><span class="sxs-lookup"><span data-stu-id="61447-149">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="61447-150">formato</span><span class="sxs-lookup"><span data-stu-id="61447-150">format</span></span>|[<span data-ttu-id="61447-151">ChartDataLabelFormat</span><span class="sxs-lookup"><span data-stu-id="61447-151">ChartDataLabelFormat</span></span>](chartdatalabelformat.md)|<span data-ttu-id="61447-p103">Representa o formato dos rótulos de dados do gráfico, que inclui a formatação de fonte e de preenchimento. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="61447-p103">Represents the format of chart data labels, which includes fill and font formatting. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="61447-154">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="61447-154">JSON representation</span></span>

<span data-ttu-id="61447-155">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="61447-155">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "ChartDataLabels resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
