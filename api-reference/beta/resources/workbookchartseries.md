---
title: tipo de recurso workbookChartSeries
description: Representa uma série de um gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 22ce2138da7ae8163304978370ada1f71abe7026
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47979228"
---
# <a name="workbookchartseries-resource-type"></a><span data-ttu-id="16a68-103">tipo de recurso workbookChartSeries</span><span class="sxs-lookup"><span data-stu-id="16a68-103">workbookChartSeries resource type</span></span>

<span data-ttu-id="16a68-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="16a68-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="16a68-105">Representa uma série de um gráfico.</span><span class="sxs-lookup"><span data-stu-id="16a68-105">Represents a series in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="16a68-106">Methods</span><span class="sxs-lookup"><span data-stu-id="16a68-106">Methods</span></span>

| <span data-ttu-id="16a68-107">Método</span><span class="sxs-lookup"><span data-stu-id="16a68-107">Method</span></span>           | <span data-ttu-id="16a68-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="16a68-108">Return Type</span></span>    |<span data-ttu-id="16a68-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="16a68-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="16a68-110">Get ChartSeries</span><span class="sxs-lookup"><span data-stu-id="16a68-110">Get ChartSeries</span></span>](../api/chartseries-get.md) | [<span data-ttu-id="16a68-111">workbookChartSeries</span><span class="sxs-lookup"><span data-stu-id="16a68-111">workbookChartSeries</span></span>](workbookchartseries.md) |<span data-ttu-id="16a68-112">Leia as propriedades e os relacionamentos do objeto chartSeries.</span><span class="sxs-lookup"><span data-stu-id="16a68-112">Read properties and relationships of chartSeries object.</span></span>|
|[<span data-ttu-id="16a68-113">Criar ChartPoint</span><span class="sxs-lookup"><span data-stu-id="16a68-113">Create ChartPoint</span></span>](../api/chartseries-post-points.md) |[<span data-ttu-id="16a68-114">chartPoints</span><span class="sxs-lookup"><span data-stu-id="16a68-114">chartPoints</span></span>](workbookchartpoint.md)| <span data-ttu-id="16a68-115">Crie um novo chartPoint postando na coleção Points.</span><span class="sxs-lookup"><span data-stu-id="16a68-115">Create a new chartPoint by posting to the points collection.</span></span>|
|[<span data-ttu-id="16a68-116">List points</span><span class="sxs-lookup"><span data-stu-id="16a68-116">List points</span></span>](../api/chartseries-list-points.md) |<span data-ttu-id="16a68-117">coleção [workbookChartPoints](workbookchartpoint.md)</span><span class="sxs-lookup"><span data-stu-id="16a68-117">[workbookChartPoints](workbookchartpoint.md) collection</span></span>| <span data-ttu-id="16a68-118">Obtenha uma coleção de objetos chartPoints.</span><span class="sxs-lookup"><span data-stu-id="16a68-118">Get a chartPoints object collection.</span></span>|
|[<span data-ttu-id="16a68-119">Atualização</span><span class="sxs-lookup"><span data-stu-id="16a68-119">Update</span></span>](../api/chartseries-update.md) | [<span data-ttu-id="16a68-120">workbookChartSeries</span><span class="sxs-lookup"><span data-stu-id="16a68-120">workbookChartSeries</span></span>](workbookchartseries.md) |<span data-ttu-id="16a68-121">Atualize o objeto chartSeries.</span><span class="sxs-lookup"><span data-stu-id="16a68-121">Update chartSeries object.</span></span> |
|[<span data-ttu-id="16a68-122">List</span><span class="sxs-lookup"><span data-stu-id="16a68-122">List</span></span>](../api/chartseries-list.md) | <span data-ttu-id="16a68-123">coleção [workbookChartSeries](workbookchartseries.md)</span><span class="sxs-lookup"><span data-stu-id="16a68-123">[workbookChartSeries](workbookchartseries.md) collection</span></span> |<span data-ttu-id="16a68-124">Obtenha uma coleção de objetos chartSeries.</span><span class="sxs-lookup"><span data-stu-id="16a68-124">Get chartSeries object collection.</span></span> |
|[<span data-ttu-id="16a68-125">ItemAt</span><span class="sxs-lookup"><span data-stu-id="16a68-125">ItemAt</span></span>](../api/chartseriescollection-itemat.md)|[<span data-ttu-id="16a68-126">workbookChartSeries</span><span class="sxs-lookup"><span data-stu-id="16a68-126">workbookChartSeries</span></span>](workbookchartseries.md)|<span data-ttu-id="16a68-127">Recupera uma série com base na respectiva posição na coleção</span><span class="sxs-lookup"><span data-stu-id="16a68-127">Retrieves a series based on its position in the collection</span></span>|

## <a name="properties"></a><span data-ttu-id="16a68-128">Propriedades</span><span class="sxs-lookup"><span data-stu-id="16a68-128">Properties</span></span>
| <span data-ttu-id="16a68-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="16a68-129">Property</span></span>     | <span data-ttu-id="16a68-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="16a68-130">Type</span></span>   |<span data-ttu-id="16a68-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="16a68-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="16a68-132">nome</span><span class="sxs-lookup"><span data-stu-id="16a68-132">name</span></span>|<span data-ttu-id="16a68-133">string</span><span class="sxs-lookup"><span data-stu-id="16a68-133">string</span></span>|<span data-ttu-id="16a68-134">Representa o nome de uma série do gráfico.</span><span class="sxs-lookup"><span data-stu-id="16a68-134">Represents the name of a series in a chart.</span></span>|

## <a name="relationships"></a><span data-ttu-id="16a68-135">Relações</span><span class="sxs-lookup"><span data-stu-id="16a68-135">Relationships</span></span>
| <span data-ttu-id="16a68-136">Relação</span><span class="sxs-lookup"><span data-stu-id="16a68-136">Relationship</span></span> | <span data-ttu-id="16a68-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="16a68-137">Type</span></span>   |<span data-ttu-id="16a68-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="16a68-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="16a68-139">formato</span><span class="sxs-lookup"><span data-stu-id="16a68-139">format</span></span>|[<span data-ttu-id="16a68-140">workbookChartSeriesFormat</span><span class="sxs-lookup"><span data-stu-id="16a68-140">workbookChartSeriesFormat</span></span>](workbookchartseriesformat.md)|<span data-ttu-id="16a68-p101">Representa a formatação de uma série do gráfico, que inclui a formatação de linha e de preenchimento. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="16a68-p101">Represents the formatting of a chart series, which includes fill and line formatting. Read-only.</span></span>|
|<span data-ttu-id="16a68-143">points</span><span class="sxs-lookup"><span data-stu-id="16a68-143">points</span></span>|<span data-ttu-id="16a68-144">coleção [workbookChartPoint](workbookchartpoint.md)</span><span class="sxs-lookup"><span data-stu-id="16a68-144">[workbookChartPoint](workbookchartpoint.md) collection</span></span>|<span data-ttu-id="16a68-145">Representa uma coleção de todos os pontos da série.</span><span class="sxs-lookup"><span data-stu-id="16a68-145">Represents a collection of all points in the series.</span></span> <span data-ttu-id="16a68-146">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="16a68-146">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="16a68-147">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="16a68-147">JSON representation</span></span>

<span data-ttu-id="16a68-148">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="16a68-148">Here is a JSON representation of the resource.</span></span>

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


