---
title: Tipo de recurso ChartSeries
description: Representa uma série de um gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: f7d42633321c78eb03942072731b0636a8ca73b7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531828"
---
# <a name="chartseries-resource-type"></a><span data-ttu-id="b4869-103">Tipo de recurso ChartSeries</span><span class="sxs-lookup"><span data-stu-id="b4869-103">ChartSeries resource type</span></span>

<span data-ttu-id="b4869-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b4869-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b4869-105">Representa uma série de um gráfico.</span><span class="sxs-lookup"><span data-stu-id="b4869-105">Represents a series in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="b4869-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="b4869-106">Methods</span></span>

| <span data-ttu-id="b4869-107">Método</span><span class="sxs-lookup"><span data-stu-id="b4869-107">Method</span></span>           | <span data-ttu-id="b4869-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b4869-108">Return Type</span></span>    |<span data-ttu-id="b4869-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="b4869-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b4869-110">Get ChartSeries</span><span class="sxs-lookup"><span data-stu-id="b4869-110">Get ChartSeries</span></span>](../api/chartseries-get.md) | [<span data-ttu-id="b4869-111">WorkbookChartSeries</span><span class="sxs-lookup"><span data-stu-id="b4869-111">WorkbookChartSeries</span></span>](chartseries.md) |<span data-ttu-id="b4869-112">Leia as propriedades e os relacionamentos do objeto chartSeries.</span><span class="sxs-lookup"><span data-stu-id="b4869-112">Read properties and relationships of chartSeries object.</span></span>|
|[<span data-ttu-id="b4869-113">Create ChartPoints</span><span class="sxs-lookup"><span data-stu-id="b4869-113">Create ChartPoints</span></span>](../api/chartseries-post-points.md) |[<span data-ttu-id="b4869-114">ChartPoints</span><span class="sxs-lookup"><span data-stu-id="b4869-114">ChartPoints</span></span>](chartpoint.md)| <span data-ttu-id="b4869-115">Crie um novo ChartPoints postando na coleção de pontos.</span><span class="sxs-lookup"><span data-stu-id="b4869-115">Create a new ChartPoints by posting to the points collection.</span></span>|
|[<span data-ttu-id="b4869-116">List points</span><span class="sxs-lookup"><span data-stu-id="b4869-116">List points</span></span>](../api/chartseries-list-points.md) |<span data-ttu-id="b4869-117">Coleção [ChartPoints](chartpoint.md)</span><span class="sxs-lookup"><span data-stu-id="b4869-117">[ChartPoints](chartpoint.md) collection</span></span>| <span data-ttu-id="b4869-118">Obtenha uma coleção de objetos ChartPoints.</span><span class="sxs-lookup"><span data-stu-id="b4869-118">Get a ChartPoints object collection.</span></span>|
|[<span data-ttu-id="b4869-119">Update</span><span class="sxs-lookup"><span data-stu-id="b4869-119">Update</span></span>](../api/chartseries-update.md) | [<span data-ttu-id="b4869-120">WorkbookChartSeries</span><span class="sxs-lookup"><span data-stu-id="b4869-120">WorkbookChartSeries</span></span>](chartseries.md) |<span data-ttu-id="b4869-121">Atualize o objeto ChartSeries.</span><span class="sxs-lookup"><span data-stu-id="b4869-121">Update ChartSeries object.</span></span> |
|[<span data-ttu-id="b4869-122">List</span><span class="sxs-lookup"><span data-stu-id="b4869-122">List</span></span>](../api/chartseries-list.md) | <span data-ttu-id="b4869-123">Coleção [WorkbookChartSeries](chartseries.md)</span><span class="sxs-lookup"><span data-stu-id="b4869-123">[WorkbookChartSeries](chartseries.md) collection</span></span> |<span data-ttu-id="b4869-124">Obtenha uma coleção de objetos chartSeries.</span><span class="sxs-lookup"><span data-stu-id="b4869-124">Get chartSeries object collection.</span></span> |
|[<span data-ttu-id="b4869-125">ItemAt</span><span class="sxs-lookup"><span data-stu-id="b4869-125">ItemAt</span></span>](../api/chartseriescollection-itemat.md)|[<span data-ttu-id="b4869-126">WorkbookChartSeries</span><span class="sxs-lookup"><span data-stu-id="b4869-126">WorkbookChartSeries</span></span>](chartseries.md)|<span data-ttu-id="b4869-127">Recupera uma série com base na respectiva posição na coleção</span><span class="sxs-lookup"><span data-stu-id="b4869-127">Retrieves a series based on its position in the collection</span></span>|

## <a name="properties"></a><span data-ttu-id="b4869-128">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b4869-128">Properties</span></span>
| <span data-ttu-id="b4869-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b4869-129">Property</span></span>     | <span data-ttu-id="b4869-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="b4869-130">Type</span></span>   |<span data-ttu-id="b4869-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="b4869-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b4869-132">nome</span><span class="sxs-lookup"><span data-stu-id="b4869-132">name</span></span>|<span data-ttu-id="b4869-133">string</span><span class="sxs-lookup"><span data-stu-id="b4869-133">string</span></span>|<span data-ttu-id="b4869-134">Representa o nome de uma série do gráfico.</span><span class="sxs-lookup"><span data-stu-id="b4869-134">Represents the name of a series in a chart.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b4869-135">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="b4869-135">Relationships</span></span>
| <span data-ttu-id="b4869-136">Relação</span><span class="sxs-lookup"><span data-stu-id="b4869-136">Relationship</span></span> | <span data-ttu-id="b4869-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="b4869-137">Type</span></span>   |<span data-ttu-id="b4869-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="b4869-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b4869-139">formato</span><span class="sxs-lookup"><span data-stu-id="b4869-139">format</span></span>|[<span data-ttu-id="b4869-140">WorkbookChartSeriesFormat</span><span class="sxs-lookup"><span data-stu-id="b4869-140">WorkbookChartSeriesFormat</span></span>](chartseriesformat.md)|<span data-ttu-id="b4869-p101">Representa a formatação de uma série do gráfico, que inclui a formatação de linha e de preenchimento. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b4869-p101">Represents the formatting of a chart series, which includes fill and line formatting. Read-only.</span></span>|
|<span data-ttu-id="b4869-143">points</span><span class="sxs-lookup"><span data-stu-id="b4869-143">points</span></span>|<span data-ttu-id="b4869-144">Coleção [WorkbookChartPoint](chartpoint.md)</span><span class="sxs-lookup"><span data-stu-id="b4869-144">[WorkbookChartPoint](chartpoint.md) collection</span></span>|<span data-ttu-id="b4869-145">Representa uma coleção de todos os pontos da série.</span><span class="sxs-lookup"><span data-stu-id="b4869-145">Represents a collection of all points in the series.</span></span> <span data-ttu-id="b4869-146">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b4869-146">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b4869-147">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b4869-147">JSON representation</span></span>

<span data-ttu-id="b4869-148">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b4869-148">Here is a JSON representation of the resource.</span></span>

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
