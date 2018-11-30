---
title: Tipo de recurso ChartSeries
description: Representa uma série em um gráfico.
ms.openlocfilehash: 970a35511b1851e09c47257bf3f67d05228d4454
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27003889"
---
# <a name="chartseries-resource-type"></a><span data-ttu-id="43e76-103">Tipo de recurso ChartSeries</span><span class="sxs-lookup"><span data-stu-id="43e76-103">ChartSeries resource type</span></span>

<span data-ttu-id="43e76-104">Representa uma série em um gráfico.</span><span class="sxs-lookup"><span data-stu-id="43e76-104">Represents a series in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="43e76-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="43e76-105">Methods</span></span>

| <span data-ttu-id="43e76-106">Método</span><span class="sxs-lookup"><span data-stu-id="43e76-106">Method</span></span>           | <span data-ttu-id="43e76-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="43e76-107">Return Type</span></span>    |<span data-ttu-id="43e76-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="43e76-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="43e76-109">Get ChartSeries</span><span class="sxs-lookup"><span data-stu-id="43e76-109">Get ChartSeries</span></span>](../api/chartseries-get.md) | [<span data-ttu-id="43e76-110">WorkbookChartSeries</span><span class="sxs-lookup"><span data-stu-id="43e76-110">WorkbookChartSeries</span></span>](chartseries.md) |<span data-ttu-id="43e76-111">Leia as propriedades e os relacionamentos do objeto chartSeries.</span><span class="sxs-lookup"><span data-stu-id="43e76-111">Read properties and relationships of chartSeries object.</span></span>|
|[<span data-ttu-id="43e76-112">Create ChartPoints</span><span class="sxs-lookup"><span data-stu-id="43e76-112">Create ChartPoints</span></span>](../api/chartseries-post-points.md) |[<span data-ttu-id="43e76-113">ChartPoints</span><span class="sxs-lookup"><span data-stu-id="43e76-113">ChartPoints</span></span>](chartpoint.md)| <span data-ttu-id="43e76-114">Crie um novo ChartPoints postando na coleção de pontos.</span><span class="sxs-lookup"><span data-stu-id="43e76-114">Create a new ChartPoints by posting to the points collection.</span></span>|
|[<span data-ttu-id="43e76-115">List points</span><span class="sxs-lookup"><span data-stu-id="43e76-115">List points</span></span>](../api/chartseries-list-points.md) |<span data-ttu-id="43e76-116">Coleção [ChartPoints](chartpoint.md)</span><span class="sxs-lookup"><span data-stu-id="43e76-116">[ChartPoints](chartpoint.md) collection</span></span>| <span data-ttu-id="43e76-117">Obtenha uma coleção de objetos ChartPoints.</span><span class="sxs-lookup"><span data-stu-id="43e76-117">Get a ChartPoints object collection.</span></span>|
|[<span data-ttu-id="43e76-118">Update</span><span class="sxs-lookup"><span data-stu-id="43e76-118">Update</span></span>](../api/chartseries-update.md) | [<span data-ttu-id="43e76-119">WorkbookChartSeries</span><span class="sxs-lookup"><span data-stu-id="43e76-119">WorkbookChartSeries</span></span>](chartseries.md) |<span data-ttu-id="43e76-120">Atualize o objeto ChartSeries.</span><span class="sxs-lookup"><span data-stu-id="43e76-120">Update ChartSeries object.</span></span> |
|[<span data-ttu-id="43e76-121">List</span><span class="sxs-lookup"><span data-stu-id="43e76-121">List</span></span>](../api/chartseries-list.md) | <span data-ttu-id="43e76-122">Coleção [WorkbookChartSeries](chartseries.md)</span><span class="sxs-lookup"><span data-stu-id="43e76-122">[WorkbookChartSeries](chartseries.md) collection</span></span> |<span data-ttu-id="43e76-123">Obtenha uma coleção de objetos chartSeries.</span><span class="sxs-lookup"><span data-stu-id="43e76-123">Get chartSeries object collection.</span></span> |
|[<span data-ttu-id="43e76-124">ItemAt</span><span class="sxs-lookup"><span data-stu-id="43e76-124">ItemAt</span></span>](../api/chartseriescollection-itemat.md)|[<span data-ttu-id="43e76-125">WorkbookChartSeries</span><span class="sxs-lookup"><span data-stu-id="43e76-125">WorkbookChartSeries</span></span>](chartseries.md)|<span data-ttu-id="43e76-126">Recupera uma série com base na respectiva posição na coleção.</span><span class="sxs-lookup"><span data-stu-id="43e76-126">Retrieves a series based on its position in the collection</span></span>|

## <a name="properties"></a><span data-ttu-id="43e76-127">Propriedades</span><span class="sxs-lookup"><span data-stu-id="43e76-127">Properties</span></span>
| <span data-ttu-id="43e76-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="43e76-128">Property</span></span>     | <span data-ttu-id="43e76-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="43e76-129">Type</span></span>   |<span data-ttu-id="43e76-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="43e76-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="43e76-131">name</span><span class="sxs-lookup"><span data-stu-id="43e76-131">name</span></span>|<span data-ttu-id="43e76-132">string</span><span class="sxs-lookup"><span data-stu-id="43e76-132">string</span></span>|<span data-ttu-id="43e76-133">Representa o nome de uma série em um gráfico.</span><span class="sxs-lookup"><span data-stu-id="43e76-133">Represents the name of a series in a chart.</span></span>|

## <a name="relationships"></a><span data-ttu-id="43e76-134">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="43e76-134">Relationships</span></span>
| <span data-ttu-id="43e76-135">Relação</span><span class="sxs-lookup"><span data-stu-id="43e76-135">Relationship</span></span> | <span data-ttu-id="43e76-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="43e76-136">Type</span></span>   |<span data-ttu-id="43e76-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="43e76-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="43e76-138">formato</span><span class="sxs-lookup"><span data-stu-id="43e76-138">format</span></span>|[<span data-ttu-id="43e76-139">WorkbookChartSeriesFormat</span><span class="sxs-lookup"><span data-stu-id="43e76-139">WorkbookChartSeriesFormat</span></span>](chartseriesformat.md)|<span data-ttu-id="43e76-p101">Representa a formatação de uma série do gráfico, que inclui a formatação de linha e de preenchimento. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="43e76-p101">Represents the formatting of a chart series, which includes fill and line formatting. Read-only.</span></span>|
|<span data-ttu-id="43e76-142">points</span><span class="sxs-lookup"><span data-stu-id="43e76-142">points</span></span>|<span data-ttu-id="43e76-143">Coleção [WorkbookChartPoint](chartpoint.md)</span><span class="sxs-lookup"><span data-stu-id="43e76-143">[WorkbookChartPoint](chartpoint.md) collection</span></span>|<span data-ttu-id="43e76-p102">Representa uma coleção de todos os pontos da série. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="43e76-p102">Represents a collection of all points in the series. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="43e76-146">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="43e76-146">JSON representation</span></span>

<span data-ttu-id="43e76-147">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="43e76-147">Here is a JSON representation of the resource.</span></span>

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