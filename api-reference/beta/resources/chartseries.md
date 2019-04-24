---
title: Tipo de recurso ChartSeries
description: Representa uma série de um gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: e5606516092633ff14d23947f73626adc6d83c2c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32460993"
---
# <a name="chartseries-resource-type"></a><span data-ttu-id="06522-103">Tipo de recurso ChartSeries</span><span class="sxs-lookup"><span data-stu-id="06522-103">ChartSeries resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="06522-104">Representa uma série de um gráfico.</span><span class="sxs-lookup"><span data-stu-id="06522-104">Represents a series in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="06522-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="06522-105">Methods</span></span>

| <span data-ttu-id="06522-106">Método</span><span class="sxs-lookup"><span data-stu-id="06522-106">Method</span></span>           | <span data-ttu-id="06522-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="06522-107">Return Type</span></span>    |<span data-ttu-id="06522-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="06522-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="06522-109">Get ChartSeries</span><span class="sxs-lookup"><span data-stu-id="06522-109">Get ChartSeries</span></span>](../api/chartseries-get.md) | [<span data-ttu-id="06522-110">ChartSeries</span><span class="sxs-lookup"><span data-stu-id="06522-110">ChartSeries</span></span>](chartseries.md) |<span data-ttu-id="06522-111">Leia as propriedades e os relacionamentos do objeto chartSeries.</span><span class="sxs-lookup"><span data-stu-id="06522-111">Read properties and relationships of chartSeries object.</span></span>|
|[<span data-ttu-id="06522-112">Create ChartPoints</span><span class="sxs-lookup"><span data-stu-id="06522-112">Create ChartPoints</span></span>](../api/chartseries-post-points.md) |[<span data-ttu-id="06522-113">ChartPoints</span><span class="sxs-lookup"><span data-stu-id="06522-113">ChartPoints</span></span>](chartpoint.md)| <span data-ttu-id="06522-114">Crie um novo ChartPoints postando na coleção de pontos.</span><span class="sxs-lookup"><span data-stu-id="06522-114">Create a new ChartPoints by posting to the points collection.</span></span>|
|[<span data-ttu-id="06522-115">List points</span><span class="sxs-lookup"><span data-stu-id="06522-115">List points</span></span>](../api/chartseries-list-points.md) |<span data-ttu-id="06522-116">Coleção [ChartPoints](chartpoint.md)</span><span class="sxs-lookup"><span data-stu-id="06522-116">[ChartPoints](chartpoint.md) collection</span></span>| <span data-ttu-id="06522-117">Obtenha uma coleção de objetos ChartPoints.</span><span class="sxs-lookup"><span data-stu-id="06522-117">Get a ChartPoints object collection.</span></span>|
|[<span data-ttu-id="06522-118">Update</span><span class="sxs-lookup"><span data-stu-id="06522-118">Update</span></span>](../api/chartseries-update.md) | [<span data-ttu-id="06522-119">ChartSeries</span><span class="sxs-lookup"><span data-stu-id="06522-119">ChartSeries</span></span>](chartseries.md) |<span data-ttu-id="06522-120">Atualize o objeto ChartSeries.</span><span class="sxs-lookup"><span data-stu-id="06522-120">Update ChartSeries object.</span></span> |
|[<span data-ttu-id="06522-121">List</span><span class="sxs-lookup"><span data-stu-id="06522-121">List</span></span>](../api/chartseries-list.md) | <span data-ttu-id="06522-122">Coleção [ChartSeries](chartseries.md)</span><span class="sxs-lookup"><span data-stu-id="06522-122">[ChartSeries](chartseries.md) collection</span></span> |<span data-ttu-id="06522-123">Obtenha uma coleção de objetos chartSeries.</span><span class="sxs-lookup"><span data-stu-id="06522-123">Get chartSeries object collection.</span></span> |
|[<span data-ttu-id="06522-124">Itemat</span><span class="sxs-lookup"><span data-stu-id="06522-124">Itemat</span></span>](../api/chartseriescollection-itemat.md)|[<span data-ttu-id="06522-125">ChartSeries</span><span class="sxs-lookup"><span data-stu-id="06522-125">ChartSeries</span></span>](chartseries.md)|<span data-ttu-id="06522-126">Recupera uma série com base na respectiva posição na coleção</span><span class="sxs-lookup"><span data-stu-id="06522-126">Retrieves a series based on its position in the collection</span></span>|

## <a name="properties"></a><span data-ttu-id="06522-127">Propriedades</span><span class="sxs-lookup"><span data-stu-id="06522-127">Properties</span></span>
| <span data-ttu-id="06522-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="06522-128">Property</span></span>     | <span data-ttu-id="06522-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="06522-129">Type</span></span>   |<span data-ttu-id="06522-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="06522-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="06522-131">nome</span><span class="sxs-lookup"><span data-stu-id="06522-131">name</span></span>|<span data-ttu-id="06522-132">string</span><span class="sxs-lookup"><span data-stu-id="06522-132">string</span></span>|<span data-ttu-id="06522-133">Representa o nome de uma série do gráfico.</span><span class="sxs-lookup"><span data-stu-id="06522-133">Represents the name of a series in a chart.</span></span>|

## <a name="relationships"></a><span data-ttu-id="06522-134">Relações</span><span class="sxs-lookup"><span data-stu-id="06522-134">Relationships</span></span>
| <span data-ttu-id="06522-135">Relação</span><span class="sxs-lookup"><span data-stu-id="06522-135">Relationship</span></span> | <span data-ttu-id="06522-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="06522-136">Type</span></span>   |<span data-ttu-id="06522-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="06522-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="06522-138">format</span><span class="sxs-lookup"><span data-stu-id="06522-138">format</span></span>|[<span data-ttu-id="06522-139">ChartSeriesFormat</span><span class="sxs-lookup"><span data-stu-id="06522-139">ChartSeriesFormat</span></span>](chartseriesformat.md)|<span data-ttu-id="06522-p101">Representa a formatação de uma série do gráfico, que inclui a formatação de linha e de preenchimento. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="06522-p101">Represents the formatting of a chart series, which includes fill and line formatting. Read-only.</span></span>|
|<span data-ttu-id="06522-142">points</span><span class="sxs-lookup"><span data-stu-id="06522-142">points</span></span>|<span data-ttu-id="06522-143">Coleção [ChartPoints](chartpoint.md)</span><span class="sxs-lookup"><span data-stu-id="06522-143">[ChartPoints](chartpoint.md) collection</span></span>|<span data-ttu-id="06522-p102">Representa uma coleção de todos os pontos da série. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="06522-p102">Represents a collection of all points in the series. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="06522-146">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="06522-146">JSON representation</span></span>

<span data-ttu-id="06522-147">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="06522-147">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartSeries"
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
  "suppressions": [
    "Error: /api-reference/beta/resources/chartseries.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
