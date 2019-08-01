---
title: Tipo de recurso ChartPoint
description: Representa o ponto de uma série do gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 5e0a9d9fe558f53fe87ae8e3a0a447a5bd93aa71
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032946"
---
# <a name="chartpoint-resource-type"></a><span data-ttu-id="c22dd-103">Tipo de recurso ChartPoint</span><span class="sxs-lookup"><span data-stu-id="c22dd-103">ChartPoint resource type</span></span>

<span data-ttu-id="c22dd-104">Representa o ponto de uma série do gráfico.</span><span class="sxs-lookup"><span data-stu-id="c22dd-104">Represents a point of a series in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="c22dd-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="c22dd-105">Methods</span></span>

| <span data-ttu-id="c22dd-106">Método</span><span class="sxs-lookup"><span data-stu-id="c22dd-106">Method</span></span>           | <span data-ttu-id="c22dd-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c22dd-107">Return Type</span></span>    |<span data-ttu-id="c22dd-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="c22dd-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c22dd-109">Get ChartPoint</span><span class="sxs-lookup"><span data-stu-id="c22dd-109">Get ChartPoint</span></span>](../api/chartpoint-get.md) | [<span data-ttu-id="c22dd-110">WorkbookChartPoint</span><span class="sxs-lookup"><span data-stu-id="c22dd-110">WorkbookChartPoint</span></span>](chartpoint.md) |<span data-ttu-id="c22dd-111">Leia as propriedades e os relacionamentos do objeto chartPoint.</span><span class="sxs-lookup"><span data-stu-id="c22dd-111">Read properties and relationships of chartPoint object.</span></span>|
|[<span data-ttu-id="c22dd-112">List</span><span class="sxs-lookup"><span data-stu-id="c22dd-112">List</span></span>](../api/chartpoint-list.md) | <span data-ttu-id="c22dd-113">Coleção [WorkbookChartPoint](chartpoint.md)</span><span class="sxs-lookup"><span data-stu-id="c22dd-113">[WorkbookChartPoint](chartpoint.md) collection</span></span> |<span data-ttu-id="c22dd-114">Obtenha a coleção de objetos chartPoint.</span><span class="sxs-lookup"><span data-stu-id="c22dd-114">Get chartPoint object collection.</span></span> |
|[<span data-ttu-id="c22dd-115">ItemAt</span><span class="sxs-lookup"><span data-stu-id="c22dd-115">ItemAt</span></span>](../api/chartpointscollection-itemat.md)|[<span data-ttu-id="c22dd-116">WorkbookChartPoint</span><span class="sxs-lookup"><span data-stu-id="c22dd-116">WorkbookChartPoint</span></span>](chartpoint.md)|<span data-ttu-id="c22dd-117">Recupera um ponto com base na respectiva posição dentro da série.</span><span class="sxs-lookup"><span data-stu-id="c22dd-117">Retrieve a point based on its position within the series.</span></span>|

## <a name="properties"></a><span data-ttu-id="c22dd-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c22dd-118">Properties</span></span>
| <span data-ttu-id="c22dd-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c22dd-119">Property</span></span>     | <span data-ttu-id="c22dd-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="c22dd-120">Type</span></span>   |<span data-ttu-id="c22dd-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="c22dd-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c22dd-122">valor</span><span class="sxs-lookup"><span data-stu-id="c22dd-122">value</span></span>|<span data-ttu-id="c22dd-123">Json</span><span class="sxs-lookup"><span data-stu-id="c22dd-123">Json</span></span>|<span data-ttu-id="c22dd-124">Retorna o valor de um ponto do gráfico.</span><span class="sxs-lookup"><span data-stu-id="c22dd-124">Returns the value of a chart point.</span></span> <span data-ttu-id="c22dd-125">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c22dd-125">Read-only.</span></span>|
|<span data-ttu-id="c22dd-126">id</span><span class="sxs-lookup"><span data-stu-id="c22dd-126">id</span></span>|<span data-ttu-id="c22dd-127">string</span><span class="sxs-lookup"><span data-stu-id="c22dd-127">string</span></span>|<span data-ttu-id="c22dd-128">identificador exclusivo</span><span class="sxs-lookup"><span data-stu-id="c22dd-128">unique identifier</span></span>|

## <a name="relationships"></a><span data-ttu-id="c22dd-129">Relações</span><span class="sxs-lookup"><span data-stu-id="c22dd-129">Relationships</span></span>
| <span data-ttu-id="c22dd-130">Relação</span><span class="sxs-lookup"><span data-stu-id="c22dd-130">Relationship</span></span> | <span data-ttu-id="c22dd-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="c22dd-131">Type</span></span>   |<span data-ttu-id="c22dd-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="c22dd-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c22dd-133">formato</span><span class="sxs-lookup"><span data-stu-id="c22dd-133">format</span></span>|[<span data-ttu-id="c22dd-134">WorkbookChartPointFormat</span><span class="sxs-lookup"><span data-stu-id="c22dd-134">WorkbookChartPointFormat</span></span>](chartpointformat.md)|<span data-ttu-id="c22dd-135">Encapsula as propriedades de formato de um ponto do gráfico.</span><span class="sxs-lookup"><span data-stu-id="c22dd-135">Encapsulates the format properties chart point.</span></span> <span data-ttu-id="c22dd-136">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c22dd-136">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c22dd-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c22dd-137">JSON representation</span></span>

<span data-ttu-id="c22dd-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c22dd-138">Here is a JSON representation of the resource.</span></span>

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
