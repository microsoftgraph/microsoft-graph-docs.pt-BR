---
title: Tipo de recurso ChartSeries
description: Representa uma série em um gráfico.
author: lumine2008
ms.openlocfilehash: 443b6b3dfea54b59ff92babc2776d9624bd28b20
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27325281"
---
# <a name="chartseries-resource-type"></a><span data-ttu-id="21344-103">Tipo de recurso ChartSeries</span><span class="sxs-lookup"><span data-stu-id="21344-103">ChartSeries resource type</span></span>

> <span data-ttu-id="21344-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="21344-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="21344-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="21344-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="21344-106">Representa uma série de um gráfico.</span><span class="sxs-lookup"><span data-stu-id="21344-106">Represents a series in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="21344-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="21344-107">Methods</span></span>

| <span data-ttu-id="21344-108">Método</span><span class="sxs-lookup"><span data-stu-id="21344-108">Method</span></span>           | <span data-ttu-id="21344-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="21344-109">Return Type</span></span>    |<span data-ttu-id="21344-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="21344-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="21344-111">Get ChartSeries</span><span class="sxs-lookup"><span data-stu-id="21344-111">Get ChartSeries</span></span>](../api/chartseries-get.md) | [<span data-ttu-id="21344-112">ChartSeries</span><span class="sxs-lookup"><span data-stu-id="21344-112">ChartSeries</span></span>](chartseries.md) |<span data-ttu-id="21344-113">Leia as propriedades e os relacionamentos do objeto chartSeries.</span><span class="sxs-lookup"><span data-stu-id="21344-113">Read properties and relationships of chartSeries object.</span></span>|
|[<span data-ttu-id="21344-114">Create ChartPoints</span><span class="sxs-lookup"><span data-stu-id="21344-114">Create ChartPoints</span></span>](../api/chartseries-post-points.md) |[<span data-ttu-id="21344-115">ChartPoints</span><span class="sxs-lookup"><span data-stu-id="21344-115">ChartPoints</span></span>](chartpoint.md)| <span data-ttu-id="21344-116">Crie um novo ChartPoints postando na coleção de pontos.</span><span class="sxs-lookup"><span data-stu-id="21344-116">Create a new ChartPoints by posting to the points collection.</span></span>|
|[<span data-ttu-id="21344-117">List points</span><span class="sxs-lookup"><span data-stu-id="21344-117">List points</span></span>](../api/chartseries-list-points.md) |<span data-ttu-id="21344-118">Coleção [ChartPoints](chartpoint.md)</span><span class="sxs-lookup"><span data-stu-id="21344-118">[ChartPoints](chartpoint.md) collection</span></span>| <span data-ttu-id="21344-119">Obtenha uma coleção de objetos ChartPoints.</span><span class="sxs-lookup"><span data-stu-id="21344-119">Get a ChartPoints object collection.</span></span>|
|[<span data-ttu-id="21344-120">Update</span><span class="sxs-lookup"><span data-stu-id="21344-120">Update</span></span>](../api/chartseries-update.md) | [<span data-ttu-id="21344-121">ChartSeries</span><span class="sxs-lookup"><span data-stu-id="21344-121">ChartSeries</span></span>](chartseries.md) |<span data-ttu-id="21344-122">Atualize o objeto ChartSeries.</span><span class="sxs-lookup"><span data-stu-id="21344-122">Update ChartSeries object.</span></span> |
|[<span data-ttu-id="21344-123">List</span><span class="sxs-lookup"><span data-stu-id="21344-123">List</span></span>](../api/chartseries-list.md) | <span data-ttu-id="21344-124">Coleção [ChartSeries](chartseries.md)</span><span class="sxs-lookup"><span data-stu-id="21344-124">[ChartSeries](chartseries.md) collection</span></span> |<span data-ttu-id="21344-125">Obtenha uma coleção de objetos chartSeries.</span><span class="sxs-lookup"><span data-stu-id="21344-125">Get chartSeries object collection.</span></span> |
|[<span data-ttu-id="21344-126">Itemat</span><span class="sxs-lookup"><span data-stu-id="21344-126">Itemat</span></span>](../api/chartseriescollection-itemat.md)|[<span data-ttu-id="21344-127">ChartSeries</span><span class="sxs-lookup"><span data-stu-id="21344-127">ChartSeries</span></span>](chartseries.md)|<span data-ttu-id="21344-128">Recupera uma série com base na respectiva posição na coleção.</span><span class="sxs-lookup"><span data-stu-id="21344-128">Retrieves a series based on its position in the collection</span></span>|

## <a name="properties"></a><span data-ttu-id="21344-129">Propriedades</span><span class="sxs-lookup"><span data-stu-id="21344-129">Properties</span></span>
| <span data-ttu-id="21344-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="21344-130">Property</span></span>     | <span data-ttu-id="21344-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="21344-131">Type</span></span>   |<span data-ttu-id="21344-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="21344-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="21344-133">name</span><span class="sxs-lookup"><span data-stu-id="21344-133">name</span></span>|<span data-ttu-id="21344-134">string</span><span class="sxs-lookup"><span data-stu-id="21344-134">string</span></span>|<span data-ttu-id="21344-135">Representa o nome de uma série em um gráfico.</span><span class="sxs-lookup"><span data-stu-id="21344-135">Represents the name of a series in a chart.</span></span>|

## <a name="relationships"></a><span data-ttu-id="21344-136">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="21344-136">Relationships</span></span>
| <span data-ttu-id="21344-137">Relação</span><span class="sxs-lookup"><span data-stu-id="21344-137">Relationship</span></span> | <span data-ttu-id="21344-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="21344-138">Type</span></span>   |<span data-ttu-id="21344-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="21344-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="21344-140">formato</span><span class="sxs-lookup"><span data-stu-id="21344-140">format</span></span>|[<span data-ttu-id="21344-141">ChartSeriesFormat</span><span class="sxs-lookup"><span data-stu-id="21344-141">ChartSeriesFormat</span></span>](chartseriesformat.md)|<span data-ttu-id="21344-p102">Representa a formatação de uma série do gráfico, que inclui a formatação de linha e de preenchimento. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="21344-p102">Represents the formatting of a chart series, which includes fill and line formatting. Read-only.</span></span>|
|<span data-ttu-id="21344-144">points</span><span class="sxs-lookup"><span data-stu-id="21344-144">points</span></span>|<span data-ttu-id="21344-145">Coleção [ChartPoints](chartpoint.md)</span><span class="sxs-lookup"><span data-stu-id="21344-145">[ChartPoints](chartpoint.md) collection</span></span>|<span data-ttu-id="21344-p103">Representa uma coleção de todos os pontos da série. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="21344-p103">Represents a collection of all points in the series. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="21344-148">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="21344-148">JSON representation</span></span>

<span data-ttu-id="21344-149">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="21344-149">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "ChartSeries resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->