---
title: Tipo de recurso ChartPoint
description: Representa um ponto de uma série do gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 3318415094a36100851b1c604cba2507de31f558
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962503"
---
# <a name="chartpoint-resource-type"></a><span data-ttu-id="5efac-103">Tipo de recurso ChartPoint</span><span class="sxs-lookup"><span data-stu-id="5efac-103">ChartPoint resource type</span></span>

<span data-ttu-id="5efac-104">Representa um ponto de uma série do gráfico.</span><span class="sxs-lookup"><span data-stu-id="5efac-104">Represents a point of a series in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="5efac-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="5efac-105">Methods</span></span>

| <span data-ttu-id="5efac-106">Método</span><span class="sxs-lookup"><span data-stu-id="5efac-106">Method</span></span>           | <span data-ttu-id="5efac-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="5efac-107">Return Type</span></span>    |<span data-ttu-id="5efac-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="5efac-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5efac-109">Get ChartPoint</span><span class="sxs-lookup"><span data-stu-id="5efac-109">Get ChartPoint</span></span>](../api/chartpoint-get.md) | [<span data-ttu-id="5efac-110">WorkbookChartPoint</span><span class="sxs-lookup"><span data-stu-id="5efac-110">WorkbookChartPoint</span></span>](chartpoint.md) |<span data-ttu-id="5efac-111">Leia as propriedades e os relacionamentos do objeto chartPoint.</span><span class="sxs-lookup"><span data-stu-id="5efac-111">Read properties and relationships of chartPoint object.</span></span>|
|[<span data-ttu-id="5efac-112">List</span><span class="sxs-lookup"><span data-stu-id="5efac-112">List</span></span>](../api/chartpoint-list.md) | <span data-ttu-id="5efac-113">Coleção [WorkbookChartPoint](chartpoint.md)</span><span class="sxs-lookup"><span data-stu-id="5efac-113">[WorkbookChartPoint](chartpoint.md) collection</span></span> |<span data-ttu-id="5efac-114">Obtenha a coleção de objetos chartPoint.</span><span class="sxs-lookup"><span data-stu-id="5efac-114">Get chartPoint object collection.</span></span> |
|[<span data-ttu-id="5efac-115">ItemAt</span><span class="sxs-lookup"><span data-stu-id="5efac-115">ItemAt</span></span>](../api/chartpointscollection-itemat.md)|[<span data-ttu-id="5efac-116">WorkbookChartPoint</span><span class="sxs-lookup"><span data-stu-id="5efac-116">WorkbookChartPoint</span></span>](chartpoint.md)|<span data-ttu-id="5efac-117">Recupera um ponto com base na respectiva posição dentro da série.</span><span class="sxs-lookup"><span data-stu-id="5efac-117">Retrieve a point based on its position within the series.</span></span>|

## <a name="properties"></a><span data-ttu-id="5efac-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5efac-118">Properties</span></span>
| <span data-ttu-id="5efac-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5efac-119">Property</span></span>     | <span data-ttu-id="5efac-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="5efac-120">Type</span></span>   |<span data-ttu-id="5efac-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="5efac-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5efac-122">valor</span><span class="sxs-lookup"><span data-stu-id="5efac-122">value</span></span>|<span data-ttu-id="5efac-123">Json</span><span class="sxs-lookup"><span data-stu-id="5efac-123">Json</span></span>|<span data-ttu-id="5efac-p101">Retorna o valor de um ponto do gráfico. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5efac-p101">Returns the value of a chart point. Read-only.</span></span>|
|<span data-ttu-id="5efac-126">id</span><span class="sxs-lookup"><span data-stu-id="5efac-126">id</span></span>|<span data-ttu-id="5efac-127">string</span><span class="sxs-lookup"><span data-stu-id="5efac-127">string</span></span>|<span data-ttu-id="5efac-128">Identificador exclusivo</span><span class="sxs-lookup"><span data-stu-id="5efac-128">unique identifier</span></span>|

## <a name="relationships"></a><span data-ttu-id="5efac-129">Relações</span><span class="sxs-lookup"><span data-stu-id="5efac-129">Relationships</span></span>
| <span data-ttu-id="5efac-130">Relação</span><span class="sxs-lookup"><span data-stu-id="5efac-130">Relationship</span></span> | <span data-ttu-id="5efac-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="5efac-131">Type</span></span>   |<span data-ttu-id="5efac-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="5efac-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5efac-133">formato</span><span class="sxs-lookup"><span data-stu-id="5efac-133">format</span></span>|[<span data-ttu-id="5efac-134">WorkbookChartPointFormat</span><span class="sxs-lookup"><span data-stu-id="5efac-134">WorkbookChartPointFormat</span></span>](chartpointformat.md)|<span data-ttu-id="5efac-p102">Encapsula as propriedades de formato de um ponto do gráfico. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5efac-p102">Encapsulates the format properties chart point. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5efac-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5efac-137">JSON representation</span></span>

<span data-ttu-id="5efac-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5efac-138">Here is a JSON representation of the resource.</span></span>

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
