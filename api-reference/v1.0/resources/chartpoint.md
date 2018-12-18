---
title: Tipo de recurso ChartPoint
description: Representa um ponto de uma série do gráfico.
author: lumine2008
ms.openlocfilehash: b2d1fab0c76100aae1a5606690772a0aa3854f42
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27316223"
---
# <a name="chartpoint-resource-type"></a><span data-ttu-id="60edf-103">Tipo de recurso ChartPoint</span><span class="sxs-lookup"><span data-stu-id="60edf-103">ChartPoint resource type</span></span>

<span data-ttu-id="60edf-104">Representa um ponto de uma série do gráfico.</span><span class="sxs-lookup"><span data-stu-id="60edf-104">Represents a point of a series in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="60edf-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="60edf-105">Methods</span></span>

| <span data-ttu-id="60edf-106">Método</span><span class="sxs-lookup"><span data-stu-id="60edf-106">Method</span></span>           | <span data-ttu-id="60edf-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="60edf-107">Return Type</span></span>    |<span data-ttu-id="60edf-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="60edf-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="60edf-109">Get ChartPoint</span><span class="sxs-lookup"><span data-stu-id="60edf-109">Get ChartPoint</span></span>](../api/chartpoint-get.md) | [<span data-ttu-id="60edf-110">WorkbookChartPoint</span><span class="sxs-lookup"><span data-stu-id="60edf-110">WorkbookChartPoint</span></span>](chartpoint.md) |<span data-ttu-id="60edf-111">Leia as propriedades e os relacionamentos do objeto chartPoint.</span><span class="sxs-lookup"><span data-stu-id="60edf-111">Read properties and relationships of chartPoint object.</span></span>|
|[<span data-ttu-id="60edf-112">List</span><span class="sxs-lookup"><span data-stu-id="60edf-112">List</span></span>](../api/chartpoint-list.md) | <span data-ttu-id="60edf-113">Coleção [WorkbookChartPoint](chartpoint.md)</span><span class="sxs-lookup"><span data-stu-id="60edf-113">[WorkbookChartPoint](chartpoint.md) collection</span></span> |<span data-ttu-id="60edf-114">Obtenha a coleção de objetos chartPoint.</span><span class="sxs-lookup"><span data-stu-id="60edf-114">Get chartPoint object collection.</span></span> |
|[<span data-ttu-id="60edf-115">ItemAt</span><span class="sxs-lookup"><span data-stu-id="60edf-115">ItemAt</span></span>](../api/chartpointscollection-itemat.md)|[<span data-ttu-id="60edf-116">WorkbookChartPoint</span><span class="sxs-lookup"><span data-stu-id="60edf-116">WorkbookChartPoint</span></span>](chartpoint.md)|<span data-ttu-id="60edf-117">Recupera um ponto com base na respectiva posição dentro da série.</span><span class="sxs-lookup"><span data-stu-id="60edf-117">Retrieve a point based on its position within the series.</span></span>|

## <a name="properties"></a><span data-ttu-id="60edf-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="60edf-118">Properties</span></span>
| <span data-ttu-id="60edf-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="60edf-119">Property</span></span>     | <span data-ttu-id="60edf-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="60edf-120">Type</span></span>   |<span data-ttu-id="60edf-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="60edf-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="60edf-122">valor</span><span class="sxs-lookup"><span data-stu-id="60edf-122">value</span></span>|<span data-ttu-id="60edf-123">Json</span><span class="sxs-lookup"><span data-stu-id="60edf-123">Json</span></span>|<span data-ttu-id="60edf-p101">Retorna o valor de um ponto do gráfico. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="60edf-p101">Returns the value of a chart point. Read-only.</span></span>|
|<span data-ttu-id="60edf-126">id</span><span class="sxs-lookup"><span data-stu-id="60edf-126">id</span></span>|<span data-ttu-id="60edf-127">string</span><span class="sxs-lookup"><span data-stu-id="60edf-127">string</span></span>|<span data-ttu-id="60edf-128">Identificador exclusivo</span><span class="sxs-lookup"><span data-stu-id="60edf-128">unique identifier</span></span>|

## <a name="relationships"></a><span data-ttu-id="60edf-129">Relações</span><span class="sxs-lookup"><span data-stu-id="60edf-129">Relationships</span></span>
| <span data-ttu-id="60edf-130">Relação</span><span class="sxs-lookup"><span data-stu-id="60edf-130">Relationship</span></span> | <span data-ttu-id="60edf-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="60edf-131">Type</span></span>   |<span data-ttu-id="60edf-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="60edf-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="60edf-133">formato</span><span class="sxs-lookup"><span data-stu-id="60edf-133">format</span></span>|[<span data-ttu-id="60edf-134">WorkbookChartPointFormat</span><span class="sxs-lookup"><span data-stu-id="60edf-134">WorkbookChartPointFormat</span></span>](chartpointformat.md)|<span data-ttu-id="60edf-p102">Encapsula as propriedades de formato de um ponto do gráfico. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="60edf-p102">Encapsulates the format properties chart point. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="60edf-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="60edf-137">JSON representation</span></span>

<span data-ttu-id="60edf-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="60edf-138">Here is a JSON representation of the resource.</span></span>

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