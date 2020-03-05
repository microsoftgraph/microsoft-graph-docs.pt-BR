---
title: tipo de recurso workbookChartPoint
description: Representa o ponto de uma série do gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 54342227c15eeb1b11c3ddfb157e1ef3bc83390e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519285"
---
# <a name="workbookchartpoint-resource-type"></a><span data-ttu-id="2edc0-103">tipo de recurso workbookChartPoint</span><span class="sxs-lookup"><span data-stu-id="2edc0-103">workbookChartPoint resource type</span></span>

<span data-ttu-id="2edc0-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="2edc0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2edc0-105">Representa o ponto de uma série do gráfico.</span><span class="sxs-lookup"><span data-stu-id="2edc0-105">Represents a point of a series in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="2edc0-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="2edc0-106">Methods</span></span>

| <span data-ttu-id="2edc0-107">Método</span><span class="sxs-lookup"><span data-stu-id="2edc0-107">Method</span></span>           | <span data-ttu-id="2edc0-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="2edc0-108">Return Type</span></span>    |<span data-ttu-id="2edc0-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="2edc0-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2edc0-110">Obter workbookChartPoint</span><span class="sxs-lookup"><span data-stu-id="2edc0-110">Get workbookChartPoint</span></span>](../api/chartpoint-get.md) | [<span data-ttu-id="2edc0-111">workbookChartPoint</span><span class="sxs-lookup"><span data-stu-id="2edc0-111">workbookChartPoint</span></span>](workbookchartpoint.md) |<span data-ttu-id="2edc0-112">Leia as propriedades e os relacionamentos do objeto chartPoint.</span><span class="sxs-lookup"><span data-stu-id="2edc0-112">Read properties and relationships of chartPoint object.</span></span>|
|[<span data-ttu-id="2edc0-113">List</span><span class="sxs-lookup"><span data-stu-id="2edc0-113">List</span></span>](../api/chartpoint-list.md) | <span data-ttu-id="2edc0-114">coleção [workbookChartPoint](workbookchartpoint.md)</span><span class="sxs-lookup"><span data-stu-id="2edc0-114">[workbookChartPoint](workbookchartpoint.md) collection</span></span> |<span data-ttu-id="2edc0-115">Obtenha a coleção de objetos chartPoint.</span><span class="sxs-lookup"><span data-stu-id="2edc0-115">Get chartPoint object collection.</span></span> |
|[<span data-ttu-id="2edc0-116">ItemAt</span><span class="sxs-lookup"><span data-stu-id="2edc0-116">ItemAt</span></span>](../api/chartpointscollection-itemat.md)|[<span data-ttu-id="2edc0-117">workbookChartPoint</span><span class="sxs-lookup"><span data-stu-id="2edc0-117">workbookChartPoint</span></span>](workbookchartpoint.md)|<span data-ttu-id="2edc0-118">Recupera um ponto com base na respectiva posição dentro da série.</span><span class="sxs-lookup"><span data-stu-id="2edc0-118">Retrieve a point based on its position within the series.</span></span>|

## <a name="properties"></a><span data-ttu-id="2edc0-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2edc0-119">Properties</span></span>
| <span data-ttu-id="2edc0-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2edc0-120">Property</span></span>     | <span data-ttu-id="2edc0-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="2edc0-121">Type</span></span>   |<span data-ttu-id="2edc0-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="2edc0-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2edc0-123">valor</span><span class="sxs-lookup"><span data-stu-id="2edc0-123">value</span></span>|<span data-ttu-id="2edc0-124">Json</span><span class="sxs-lookup"><span data-stu-id="2edc0-124">Json</span></span>|<span data-ttu-id="2edc0-125">Retorna o valor de um ponto do gráfico.</span><span class="sxs-lookup"><span data-stu-id="2edc0-125">Returns the value of a chart point.</span></span> <span data-ttu-id="2edc0-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2edc0-126">Read-only.</span></span>|
|<span data-ttu-id="2edc0-127">id</span><span class="sxs-lookup"><span data-stu-id="2edc0-127">id</span></span>|<span data-ttu-id="2edc0-128">string</span><span class="sxs-lookup"><span data-stu-id="2edc0-128">string</span></span>|<span data-ttu-id="2edc0-129">identificador exclusivo</span><span class="sxs-lookup"><span data-stu-id="2edc0-129">unique identifier</span></span>|

## <a name="relationships"></a><span data-ttu-id="2edc0-130">Relações</span><span class="sxs-lookup"><span data-stu-id="2edc0-130">Relationships</span></span>
| <span data-ttu-id="2edc0-131">Relação</span><span class="sxs-lookup"><span data-stu-id="2edc0-131">Relationship</span></span> | <span data-ttu-id="2edc0-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="2edc0-132">Type</span></span>   |<span data-ttu-id="2edc0-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="2edc0-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2edc0-134">formato</span><span class="sxs-lookup"><span data-stu-id="2edc0-134">format</span></span>|[<span data-ttu-id="2edc0-135">workbookChartPointFormat</span><span class="sxs-lookup"><span data-stu-id="2edc0-135">workbookChartPointFormat</span></span>](workbookchartpointformat.md)|<span data-ttu-id="2edc0-136">Encapsula as propriedades de formato de um ponto do gráfico.</span><span class="sxs-lookup"><span data-stu-id="2edc0-136">Encapsulates the format properties chart point.</span></span> <span data-ttu-id="2edc0-137">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2edc0-137">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2edc0-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2edc0-138">JSON representation</span></span>

<span data-ttu-id="2edc0-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2edc0-139">Here is a JSON representation of the resource.</span></span>

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
