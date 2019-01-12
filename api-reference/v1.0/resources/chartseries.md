---
title: Tipo de recurso ChartSeries
description: Representa uma série em um gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: b9a857f127848f1ed0da8de673902527e3858ffe
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27970384"
---
# <a name="chartseries-resource-type"></a><span data-ttu-id="c5480-103">Tipo de recurso ChartSeries</span><span class="sxs-lookup"><span data-stu-id="c5480-103">ChartSeries resource type</span></span>

<span data-ttu-id="c5480-104">Representa uma série em um gráfico.</span><span class="sxs-lookup"><span data-stu-id="c5480-104">Represents a series in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="c5480-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="c5480-105">Methods</span></span>

| <span data-ttu-id="c5480-106">Método</span><span class="sxs-lookup"><span data-stu-id="c5480-106">Method</span></span>           | <span data-ttu-id="c5480-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c5480-107">Return Type</span></span>    |<span data-ttu-id="c5480-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="c5480-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c5480-109">Get ChartSeries</span><span class="sxs-lookup"><span data-stu-id="c5480-109">Get ChartSeries</span></span>](../api/chartseries-get.md) | [<span data-ttu-id="c5480-110">WorkbookChartSeries</span><span class="sxs-lookup"><span data-stu-id="c5480-110">WorkbookChartSeries</span></span>](chartseries.md) |<span data-ttu-id="c5480-111">Leia as propriedades e os relacionamentos do objeto chartSeries.</span><span class="sxs-lookup"><span data-stu-id="c5480-111">Read properties and relationships of chartSeries object.</span></span>|
|[<span data-ttu-id="c5480-112">Create ChartPoints</span><span class="sxs-lookup"><span data-stu-id="c5480-112">Create ChartPoints</span></span>](../api/chartseries-post-points.md) |[<span data-ttu-id="c5480-113">ChartPoints</span><span class="sxs-lookup"><span data-stu-id="c5480-113">ChartPoints</span></span>](chartpoint.md)| <span data-ttu-id="c5480-114">Crie um novo ChartPoints postando na coleção de pontos.</span><span class="sxs-lookup"><span data-stu-id="c5480-114">Create a new ChartPoints by posting to the points collection.</span></span>|
|[<span data-ttu-id="c5480-115">List points</span><span class="sxs-lookup"><span data-stu-id="c5480-115">List points</span></span>](../api/chartseries-list-points.md) |<span data-ttu-id="c5480-116">Coleção [ChartPoints](chartpoint.md)</span><span class="sxs-lookup"><span data-stu-id="c5480-116">[ChartPoints](chartpoint.md) collection</span></span>| <span data-ttu-id="c5480-117">Obtenha uma coleção de objetos ChartPoints.</span><span class="sxs-lookup"><span data-stu-id="c5480-117">Get a ChartPoints object collection.</span></span>|
|[<span data-ttu-id="c5480-118">Update</span><span class="sxs-lookup"><span data-stu-id="c5480-118">Update</span></span>](../api/chartseries-update.md) | [<span data-ttu-id="c5480-119">WorkbookChartSeries</span><span class="sxs-lookup"><span data-stu-id="c5480-119">WorkbookChartSeries</span></span>](chartseries.md) |<span data-ttu-id="c5480-120">Atualize o objeto ChartSeries.</span><span class="sxs-lookup"><span data-stu-id="c5480-120">Update ChartSeries object.</span></span> |
|[<span data-ttu-id="c5480-121">List</span><span class="sxs-lookup"><span data-stu-id="c5480-121">List</span></span>](../api/chartseries-list.md) | <span data-ttu-id="c5480-122">Coleção [WorkbookChartSeries](chartseries.md)</span><span class="sxs-lookup"><span data-stu-id="c5480-122">[WorkbookChartSeries](chartseries.md) collection</span></span> |<span data-ttu-id="c5480-123">Obtenha uma coleção de objetos chartSeries.</span><span class="sxs-lookup"><span data-stu-id="c5480-123">Get chartSeries object collection.</span></span> |
|[<span data-ttu-id="c5480-124">ItemAt</span><span class="sxs-lookup"><span data-stu-id="c5480-124">ItemAt</span></span>](../api/chartseriescollection-itemat.md)|[<span data-ttu-id="c5480-125">WorkbookChartSeries</span><span class="sxs-lookup"><span data-stu-id="c5480-125">WorkbookChartSeries</span></span>](chartseries.md)|<span data-ttu-id="c5480-126">Recupera uma série com base na respectiva posição na coleção.</span><span class="sxs-lookup"><span data-stu-id="c5480-126">Retrieves a series based on its position in the collection</span></span>|

## <a name="properties"></a><span data-ttu-id="c5480-127">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c5480-127">Properties</span></span>
| <span data-ttu-id="c5480-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c5480-128">Property</span></span>     | <span data-ttu-id="c5480-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="c5480-129">Type</span></span>   |<span data-ttu-id="c5480-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="c5480-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c5480-131">name</span><span class="sxs-lookup"><span data-stu-id="c5480-131">name</span></span>|<span data-ttu-id="c5480-132">string</span><span class="sxs-lookup"><span data-stu-id="c5480-132">string</span></span>|<span data-ttu-id="c5480-133">Representa o nome de uma série em um gráfico.</span><span class="sxs-lookup"><span data-stu-id="c5480-133">Represents the name of a series in a chart.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c5480-134">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="c5480-134">Relationships</span></span>
| <span data-ttu-id="c5480-135">Relação</span><span class="sxs-lookup"><span data-stu-id="c5480-135">Relationship</span></span> | <span data-ttu-id="c5480-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="c5480-136">Type</span></span>   |<span data-ttu-id="c5480-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="c5480-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c5480-138">formato</span><span class="sxs-lookup"><span data-stu-id="c5480-138">format</span></span>|[<span data-ttu-id="c5480-139">WorkbookChartSeriesFormat</span><span class="sxs-lookup"><span data-stu-id="c5480-139">WorkbookChartSeriesFormat</span></span>](chartseriesformat.md)|<span data-ttu-id="c5480-p101">Representa a formatação de uma série do gráfico, que inclui a formatação de linha e de preenchimento. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c5480-p101">Represents the formatting of a chart series, which includes fill and line formatting. Read-only.</span></span>|
|<span data-ttu-id="c5480-142">points</span><span class="sxs-lookup"><span data-stu-id="c5480-142">points</span></span>|<span data-ttu-id="c5480-143">Coleção [WorkbookChartPoint](chartpoint.md)</span><span class="sxs-lookup"><span data-stu-id="c5480-143">[WorkbookChartPoint](chartpoint.md) collection</span></span>|<span data-ttu-id="c5480-p102">Representa uma coleção de todos os pontos da série. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c5480-p102">Represents a collection of all points in the series. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c5480-146">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c5480-146">JSON representation</span></span>

<span data-ttu-id="c5480-147">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c5480-147">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookChartSeries"
}-->

```json
{
  "name": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartSeries resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
