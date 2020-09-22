---
title: Tipo de recurso ChartPoint
description: Representa o ponto de uma série do gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 208f4eb90763210639540c9fd15bdaec89b7466c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47988377"
---
# <a name="chartpoint-resource-type"></a><span data-ttu-id="687d8-103">Tipo de recurso ChartPoint</span><span class="sxs-lookup"><span data-stu-id="687d8-103">ChartPoint resource type</span></span>

<span data-ttu-id="687d8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="687d8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="687d8-105">Representa o ponto de uma série do gráfico.</span><span class="sxs-lookup"><span data-stu-id="687d8-105">Represents a point of a series in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="687d8-106">Methods</span><span class="sxs-lookup"><span data-stu-id="687d8-106">Methods</span></span>

| <span data-ttu-id="687d8-107">Método</span><span class="sxs-lookup"><span data-stu-id="687d8-107">Method</span></span>           | <span data-ttu-id="687d8-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="687d8-108">Return Type</span></span>    |<span data-ttu-id="687d8-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="687d8-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="687d8-110">Get ChartPoint</span><span class="sxs-lookup"><span data-stu-id="687d8-110">Get ChartPoint</span></span>](../api/chartpoint-get.md) | [<span data-ttu-id="687d8-111">WorkbookChartPoint</span><span class="sxs-lookup"><span data-stu-id="687d8-111">WorkbookChartPoint</span></span>](chartpoint.md) |<span data-ttu-id="687d8-112">Leia as propriedades e os relacionamentos do objeto chartPoint.</span><span class="sxs-lookup"><span data-stu-id="687d8-112">Read properties and relationships of chartPoint object.</span></span>|
|[<span data-ttu-id="687d8-113">List</span><span class="sxs-lookup"><span data-stu-id="687d8-113">List</span></span>](../api/chartpoint-list.md) | <span data-ttu-id="687d8-114">Coleção [WorkbookChartPoint](chartpoint.md)</span><span class="sxs-lookup"><span data-stu-id="687d8-114">[WorkbookChartPoint](chartpoint.md) collection</span></span> |<span data-ttu-id="687d8-115">Obtenha a coleção de objetos chartPoint.</span><span class="sxs-lookup"><span data-stu-id="687d8-115">Get chartPoint object collection.</span></span> |
|[<span data-ttu-id="687d8-116">ItemAt</span><span class="sxs-lookup"><span data-stu-id="687d8-116">ItemAt</span></span>](../api/chartpointscollection-itemat.md)|[<span data-ttu-id="687d8-117">WorkbookChartPoint</span><span class="sxs-lookup"><span data-stu-id="687d8-117">WorkbookChartPoint</span></span>](chartpoint.md)|<span data-ttu-id="687d8-118">Recupera um ponto com base na respectiva posição dentro da série.</span><span class="sxs-lookup"><span data-stu-id="687d8-118">Retrieve a point based on its position within the series.</span></span>|

## <a name="properties"></a><span data-ttu-id="687d8-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="687d8-119">Properties</span></span>
| <span data-ttu-id="687d8-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="687d8-120">Property</span></span>     | <span data-ttu-id="687d8-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="687d8-121">Type</span></span>   |<span data-ttu-id="687d8-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="687d8-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="687d8-123">valor</span><span class="sxs-lookup"><span data-stu-id="687d8-123">value</span></span>|<span data-ttu-id="687d8-124">Json</span><span class="sxs-lookup"><span data-stu-id="687d8-124">Json</span></span>|<span data-ttu-id="687d8-125">Retorna o valor de um ponto do gráfico.</span><span class="sxs-lookup"><span data-stu-id="687d8-125">Returns the value of a chart point.</span></span> <span data-ttu-id="687d8-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="687d8-126">Read-only.</span></span>|
|<span data-ttu-id="687d8-127">id</span><span class="sxs-lookup"><span data-stu-id="687d8-127">id</span></span>|<span data-ttu-id="687d8-128">string</span><span class="sxs-lookup"><span data-stu-id="687d8-128">string</span></span>|<span data-ttu-id="687d8-129">identificador exclusivo</span><span class="sxs-lookup"><span data-stu-id="687d8-129">unique identifier</span></span>|

## <a name="relationships"></a><span data-ttu-id="687d8-130">Relações</span><span class="sxs-lookup"><span data-stu-id="687d8-130">Relationships</span></span>
| <span data-ttu-id="687d8-131">Relação</span><span class="sxs-lookup"><span data-stu-id="687d8-131">Relationship</span></span> | <span data-ttu-id="687d8-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="687d8-132">Type</span></span>   |<span data-ttu-id="687d8-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="687d8-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="687d8-134">formato</span><span class="sxs-lookup"><span data-stu-id="687d8-134">format</span></span>|[<span data-ttu-id="687d8-135">WorkbookChartPointFormat</span><span class="sxs-lookup"><span data-stu-id="687d8-135">WorkbookChartPointFormat</span></span>](chartpointformat.md)|<span data-ttu-id="687d8-136">Encapsula as propriedades de formato de um ponto do gráfico.</span><span class="sxs-lookup"><span data-stu-id="687d8-136">Encapsulates the format properties chart point.</span></span> <span data-ttu-id="687d8-137">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="687d8-137">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="687d8-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="687d8-138">JSON representation</span></span>

<span data-ttu-id="687d8-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="687d8-139">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartPoint"
}-->

```json
{
  "value": "string",
  "id": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartPoint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

