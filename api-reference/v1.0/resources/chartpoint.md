---
title: Tipo de recurso ChartPoint
description: Representa um ponto de uma série do gráfico.
ms.openlocfilehash: 93c89bca61f27924621df0376bdf50e925e25c86
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006769"
---
# <a name="chartpoint-resource-type"></a><span data-ttu-id="29917-103">Tipo de recurso ChartPoint</span><span class="sxs-lookup"><span data-stu-id="29917-103">ChartPoint resource type</span></span>

<span data-ttu-id="29917-104">Representa um ponto de uma série do gráfico.</span><span class="sxs-lookup"><span data-stu-id="29917-104">Represents a point of a series in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="29917-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="29917-105">Methods</span></span>

| <span data-ttu-id="29917-106">Método</span><span class="sxs-lookup"><span data-stu-id="29917-106">Method</span></span>           | <span data-ttu-id="29917-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="29917-107">Return Type</span></span>    |<span data-ttu-id="29917-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="29917-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="29917-109">Get ChartPoint</span><span class="sxs-lookup"><span data-stu-id="29917-109">Get ChartPoint</span></span>](../api/chartpoint-get.md) | [<span data-ttu-id="29917-110">WorkbookChartPoint</span><span class="sxs-lookup"><span data-stu-id="29917-110">WorkbookChartPoint</span></span>](chartpoint.md) |<span data-ttu-id="29917-111">Leia as propriedades e os relacionamentos do objeto chartPoint.</span><span class="sxs-lookup"><span data-stu-id="29917-111">Read properties and relationships of chartPoint object.</span></span>|
|[<span data-ttu-id="29917-112">List</span><span class="sxs-lookup"><span data-stu-id="29917-112">List</span></span>](../api/chartpoint-list.md) | <span data-ttu-id="29917-113">Coleção [WorkbookChartPoint](chartpoint.md)</span><span class="sxs-lookup"><span data-stu-id="29917-113">[WorkbookChartPoint](chartpoint.md) collection</span></span> |<span data-ttu-id="29917-114">Obtenha a coleção de objetos chartPoint.</span><span class="sxs-lookup"><span data-stu-id="29917-114">Get chartPoint object collection.</span></span> |
|[<span data-ttu-id="29917-115">ItemAt</span><span class="sxs-lookup"><span data-stu-id="29917-115">ItemAt</span></span>](../api/chartpointscollection-itemat.md)|[<span data-ttu-id="29917-116">WorkbookChartPoint</span><span class="sxs-lookup"><span data-stu-id="29917-116">WorkbookChartPoint</span></span>](chartpoint.md)|<span data-ttu-id="29917-117">Recupera um ponto com base na respectiva posição dentro da série.</span><span class="sxs-lookup"><span data-stu-id="29917-117">Retrieve a point based on its position within the series.</span></span>|

## <a name="properties"></a><span data-ttu-id="29917-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="29917-118">Properties</span></span>
| <span data-ttu-id="29917-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="29917-119">Property</span></span>     | <span data-ttu-id="29917-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="29917-120">Type</span></span>   |<span data-ttu-id="29917-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="29917-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="29917-122">valor</span><span class="sxs-lookup"><span data-stu-id="29917-122">value</span></span>|<span data-ttu-id="29917-123">Json</span><span class="sxs-lookup"><span data-stu-id="29917-123">Json</span></span>|<span data-ttu-id="29917-p101">Retorna o valor de um ponto do gráfico. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="29917-p101">Returns the value of a chart point. Read-only.</span></span>|
|<span data-ttu-id="29917-126">id</span><span class="sxs-lookup"><span data-stu-id="29917-126">id</span></span>|<span data-ttu-id="29917-127">string</span><span class="sxs-lookup"><span data-stu-id="29917-127">string</span></span>|<span data-ttu-id="29917-128">Identificador exclusivo</span><span class="sxs-lookup"><span data-stu-id="29917-128">unique identifier</span></span>|

## <a name="relationships"></a><span data-ttu-id="29917-129">Relações</span><span class="sxs-lookup"><span data-stu-id="29917-129">Relationships</span></span>
| <span data-ttu-id="29917-130">Relação</span><span class="sxs-lookup"><span data-stu-id="29917-130">Relationship</span></span> | <span data-ttu-id="29917-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="29917-131">Type</span></span>   |<span data-ttu-id="29917-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="29917-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="29917-133">formato</span><span class="sxs-lookup"><span data-stu-id="29917-133">format</span></span>|[<span data-ttu-id="29917-134">WorkbookChartPointFormat</span><span class="sxs-lookup"><span data-stu-id="29917-134">WorkbookChartPointFormat</span></span>](chartpointformat.md)|<span data-ttu-id="29917-p102">Encapsula as propriedades de formato de um ponto do gráfico. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="29917-p102">Encapsulates the format properties chart point. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="29917-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="29917-137">JSON representation</span></span>

<span data-ttu-id="29917-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="29917-138">Here is a JSON representation of the resource.</span></span>

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