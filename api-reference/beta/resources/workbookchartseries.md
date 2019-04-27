---
title: tipo de recurso workbookChartSeries
description: Representa uma série de um gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: e9ff478a5f7e91c3d116ca2dbd78e20699077aab
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348501"
---
# <a name="workbookchartseries-resource-type"></a><span data-ttu-id="38898-103">tipo de recurso workbookChartSeries</span><span class="sxs-lookup"><span data-stu-id="38898-103">workbookChartSeries resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="38898-104">Representa uma série de um gráfico.</span><span class="sxs-lookup"><span data-stu-id="38898-104">Represents a series in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="38898-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="38898-105">Methods</span></span>

| <span data-ttu-id="38898-106">Método</span><span class="sxs-lookup"><span data-stu-id="38898-106">Method</span></span>           | <span data-ttu-id="38898-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="38898-107">Return Type</span></span>    |<span data-ttu-id="38898-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="38898-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="38898-109">Get ChartSeries</span><span class="sxs-lookup"><span data-stu-id="38898-109">Get ChartSeries</span></span>](../api/chartseries-get.md) | [<span data-ttu-id="38898-110">workbookChartSeries</span><span class="sxs-lookup"><span data-stu-id="38898-110">workbookChartSeries</span></span>](workbookchartseries.md) |<span data-ttu-id="38898-111">Leia as propriedades e os relacionamentos do objeto chartSeries.</span><span class="sxs-lookup"><span data-stu-id="38898-111">Read properties and relationships of chartSeries object.</span></span>|
|[<span data-ttu-id="38898-112">Criar ChartPoint</span><span class="sxs-lookup"><span data-stu-id="38898-112">Create ChartPoint</span></span>](../api/chartseries-post-points.md) |[<span data-ttu-id="38898-113">chartPoints</span><span class="sxs-lookup"><span data-stu-id="38898-113">chartPoints</span></span>](workbookchartpoint.md)| <span data-ttu-id="38898-114">Crie um novo chartPoint postando na coleção Points.</span><span class="sxs-lookup"><span data-stu-id="38898-114">Create a new chartPoint by posting to the points collection.</span></span>|
|[<span data-ttu-id="38898-115">List points</span><span class="sxs-lookup"><span data-stu-id="38898-115">List points</span></span>](../api/chartseries-list-points.md) |<span data-ttu-id="38898-116">coleção [workbookChartPoints](workbookchartpoint.md)</span><span class="sxs-lookup"><span data-stu-id="38898-116">[workbookChartPoints](workbookchartpoint.md) collection</span></span>| <span data-ttu-id="38898-117">Obtenha uma coleção de objetos chartPoints.</span><span class="sxs-lookup"><span data-stu-id="38898-117">Get a chartPoints object collection.</span></span>|
|[<span data-ttu-id="38898-118">Update</span><span class="sxs-lookup"><span data-stu-id="38898-118">Update</span></span>](../api/chartseries-update.md) | [<span data-ttu-id="38898-119">workbookChartSeries</span><span class="sxs-lookup"><span data-stu-id="38898-119">workbookChartSeries</span></span>](workbookchartseries.md) |<span data-ttu-id="38898-120">Atualize o objeto chartSeries.</span><span class="sxs-lookup"><span data-stu-id="38898-120">Update chartSeries object.</span></span> |
|[<span data-ttu-id="38898-121">Lista</span><span class="sxs-lookup"><span data-stu-id="38898-121">List</span></span>](../api/chartseries-list.md) | <span data-ttu-id="38898-122">coleção [workbookChartSeries](workbookchartseries.md)</span><span class="sxs-lookup"><span data-stu-id="38898-122">[workbookChartSeries](workbookchartseries.md) collection</span></span> |<span data-ttu-id="38898-123">Obtenha uma coleção de objetos chartSeries.</span><span class="sxs-lookup"><span data-stu-id="38898-123">Get chartSeries object collection.</span></span> |
|[<span data-ttu-id="38898-124">ItemAt</span><span class="sxs-lookup"><span data-stu-id="38898-124">ItemAt</span></span>](../api/chartseriescollection-itemat.md)|[<span data-ttu-id="38898-125">workbookChartSeries</span><span class="sxs-lookup"><span data-stu-id="38898-125">workbookChartSeries</span></span>](workbookchartseries.md)|<span data-ttu-id="38898-126">Recupera uma série com base na respectiva posição na coleção</span><span class="sxs-lookup"><span data-stu-id="38898-126">Retrieves a series based on its position in the collection</span></span>|

## <a name="properties"></a><span data-ttu-id="38898-127">Propriedades</span><span class="sxs-lookup"><span data-stu-id="38898-127">Properties</span></span>
| <span data-ttu-id="38898-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="38898-128">Property</span></span>     | <span data-ttu-id="38898-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="38898-129">Type</span></span>   |<span data-ttu-id="38898-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="38898-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="38898-131">name</span><span class="sxs-lookup"><span data-stu-id="38898-131">name</span></span>|<span data-ttu-id="38898-132">string</span><span class="sxs-lookup"><span data-stu-id="38898-132">string</span></span>|<span data-ttu-id="38898-133">Representa o nome de uma série do gráfico.</span><span class="sxs-lookup"><span data-stu-id="38898-133">Represents the name of a series in a chart.</span></span>|

## <a name="relationships"></a><span data-ttu-id="38898-134">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="38898-134">Relationships</span></span>
| <span data-ttu-id="38898-135">Relação</span><span class="sxs-lookup"><span data-stu-id="38898-135">Relationship</span></span> | <span data-ttu-id="38898-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="38898-136">Type</span></span>   |<span data-ttu-id="38898-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="38898-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="38898-138">formato</span><span class="sxs-lookup"><span data-stu-id="38898-138">format</span></span>|[<span data-ttu-id="38898-139">workbookChartSeriesFormat</span><span class="sxs-lookup"><span data-stu-id="38898-139">workbookChartSeriesFormat</span></span>](workbookchartseriesformat.md)|<span data-ttu-id="38898-p101">Representa a formatação de uma série do gráfico, que inclui a formatação de linha e de preenchimento. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="38898-p101">Represents the formatting of a chart series, which includes fill and line formatting. Read-only.</span></span>|
|<span data-ttu-id="38898-142">points</span><span class="sxs-lookup"><span data-stu-id="38898-142">points</span></span>|<span data-ttu-id="38898-143">coleção [workbookChartPoint](workbookchartpoint.md)</span><span class="sxs-lookup"><span data-stu-id="38898-143">[workbookChartPoint](workbookchartpoint.md) collection</span></span>|<span data-ttu-id="38898-144">Representa uma coleção de todos os pontos da série.</span><span class="sxs-lookup"><span data-stu-id="38898-144">Represents a collection of all points in the series.</span></span> <span data-ttu-id="38898-145">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="38898-145">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="38898-146">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="38898-146">JSON representation</span></span>

<span data-ttu-id="38898-147">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="38898-147">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "ChartSeries resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
