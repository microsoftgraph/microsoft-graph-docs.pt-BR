---
title: tipo de recurso workbookChartPoint
description: Representa o ponto de uma série do gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: df7f7254251f2b424af0ffc8a6fca725285393cf
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47993005"
---
# <a name="workbookchartpoint-resource-type"></a><span data-ttu-id="5efed-103">tipo de recurso workbookChartPoint</span><span class="sxs-lookup"><span data-stu-id="5efed-103">workbookChartPoint resource type</span></span>

<span data-ttu-id="5efed-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5efed-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5efed-105">Representa o ponto de uma série do gráfico.</span><span class="sxs-lookup"><span data-stu-id="5efed-105">Represents a point of a series in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="5efed-106">Methods</span><span class="sxs-lookup"><span data-stu-id="5efed-106">Methods</span></span>

| <span data-ttu-id="5efed-107">Método</span><span class="sxs-lookup"><span data-stu-id="5efed-107">Method</span></span>           | <span data-ttu-id="5efed-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="5efed-108">Return Type</span></span>    |<span data-ttu-id="5efed-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="5efed-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5efed-110">Obter workbookChartPoint</span><span class="sxs-lookup"><span data-stu-id="5efed-110">Get workbookChartPoint</span></span>](../api/chartpoint-get.md) | [<span data-ttu-id="5efed-111">workbookChartPoint</span><span class="sxs-lookup"><span data-stu-id="5efed-111">workbookChartPoint</span></span>](workbookchartpoint.md) |<span data-ttu-id="5efed-112">Leia as propriedades e os relacionamentos do objeto chartPoint.</span><span class="sxs-lookup"><span data-stu-id="5efed-112">Read properties and relationships of chartPoint object.</span></span>|
|[<span data-ttu-id="5efed-113">List</span><span class="sxs-lookup"><span data-stu-id="5efed-113">List</span></span>](../api/chartpoint-list.md) | <span data-ttu-id="5efed-114">coleção [workbookChartPoint](workbookchartpoint.md)</span><span class="sxs-lookup"><span data-stu-id="5efed-114">[workbookChartPoint](workbookchartpoint.md) collection</span></span> |<span data-ttu-id="5efed-115">Obtenha a coleção de objetos chartPoint.</span><span class="sxs-lookup"><span data-stu-id="5efed-115">Get chartPoint object collection.</span></span> |
|[<span data-ttu-id="5efed-116">ItemAt</span><span class="sxs-lookup"><span data-stu-id="5efed-116">ItemAt</span></span>](../api/chartpointscollection-itemat.md)|[<span data-ttu-id="5efed-117">workbookChartPoint</span><span class="sxs-lookup"><span data-stu-id="5efed-117">workbookChartPoint</span></span>](workbookchartpoint.md)|<span data-ttu-id="5efed-118">Recupera um ponto com base na respectiva posição dentro da série.</span><span class="sxs-lookup"><span data-stu-id="5efed-118">Retrieve a point based on its position within the series.</span></span>|

## <a name="properties"></a><span data-ttu-id="5efed-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5efed-119">Properties</span></span>
| <span data-ttu-id="5efed-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5efed-120">Property</span></span>     | <span data-ttu-id="5efed-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="5efed-121">Type</span></span>   |<span data-ttu-id="5efed-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="5efed-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5efed-123">valor</span><span class="sxs-lookup"><span data-stu-id="5efed-123">value</span></span>|<span data-ttu-id="5efed-124">Json</span><span class="sxs-lookup"><span data-stu-id="5efed-124">Json</span></span>|<span data-ttu-id="5efed-125">Retorna o valor de um ponto do gráfico.</span><span class="sxs-lookup"><span data-stu-id="5efed-125">Returns the value of a chart point.</span></span> <span data-ttu-id="5efed-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5efed-126">Read-only.</span></span>|
|<span data-ttu-id="5efed-127">id</span><span class="sxs-lookup"><span data-stu-id="5efed-127">id</span></span>|<span data-ttu-id="5efed-128">string</span><span class="sxs-lookup"><span data-stu-id="5efed-128">string</span></span>|<span data-ttu-id="5efed-129">identificador exclusivo</span><span class="sxs-lookup"><span data-stu-id="5efed-129">unique identifier</span></span>|

## <a name="relationships"></a><span data-ttu-id="5efed-130">Relações</span><span class="sxs-lookup"><span data-stu-id="5efed-130">Relationships</span></span>
| <span data-ttu-id="5efed-131">Relação</span><span class="sxs-lookup"><span data-stu-id="5efed-131">Relationship</span></span> | <span data-ttu-id="5efed-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="5efed-132">Type</span></span>   |<span data-ttu-id="5efed-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="5efed-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5efed-134">formato</span><span class="sxs-lookup"><span data-stu-id="5efed-134">format</span></span>|[<span data-ttu-id="5efed-135">workbookChartPointFormat</span><span class="sxs-lookup"><span data-stu-id="5efed-135">workbookChartPointFormat</span></span>](workbookchartpointformat.md)|<span data-ttu-id="5efed-136">Encapsula as propriedades de formato de um ponto do gráfico.</span><span class="sxs-lookup"><span data-stu-id="5efed-136">Encapsulates the format properties chart point.</span></span> <span data-ttu-id="5efed-137">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5efed-137">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5efed-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5efed-138">JSON representation</span></span>

<span data-ttu-id="5efed-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5efed-139">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "format"
    ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartPoint"
}-->

```json
{
  "value": "string",
  "id": "string",
  "format": {"@odata.type": "microsoft.graph.workbookChartPointFormat"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ChartPoint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


