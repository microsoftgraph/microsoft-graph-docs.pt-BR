---
title: tipo de recurso workbookChartPoint
description: Representa o ponto de uma série do gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: db0037e91f1ee9279a131c5a318c4425e7878aed
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007253"
---
# <a name="workbookchartpoint-resource-type"></a><span data-ttu-id="2e5ca-103">tipo de recurso workbookChartPoint</span><span class="sxs-lookup"><span data-stu-id="2e5ca-103">workbookChartPoint resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2e5ca-104">Representa o ponto de uma série do gráfico.</span><span class="sxs-lookup"><span data-stu-id="2e5ca-104">Represents a point of a series in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="2e5ca-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="2e5ca-105">Methods</span></span>

| <span data-ttu-id="2e5ca-106">Método</span><span class="sxs-lookup"><span data-stu-id="2e5ca-106">Method</span></span>           | <span data-ttu-id="2e5ca-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="2e5ca-107">Return Type</span></span>    |<span data-ttu-id="2e5ca-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="2e5ca-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2e5ca-109">Obter workbookChartPoint</span><span class="sxs-lookup"><span data-stu-id="2e5ca-109">Get workbookChartPoint</span></span>](../api/chartpoint-get.md) | [<span data-ttu-id="2e5ca-110">workbookChartPoint</span><span class="sxs-lookup"><span data-stu-id="2e5ca-110">workbookChartPoint</span></span>](workbookchartpoint.md) |<span data-ttu-id="2e5ca-111">Leia as propriedades e os relacionamentos do objeto chartPoint.</span><span class="sxs-lookup"><span data-stu-id="2e5ca-111">Read properties and relationships of chartPoint object.</span></span>|
|[<span data-ttu-id="2e5ca-112">List</span><span class="sxs-lookup"><span data-stu-id="2e5ca-112">List</span></span>](../api/chartpoint-list.md) | <span data-ttu-id="2e5ca-113">coleção [workbookChartPoint](workbookchartpoint.md)</span><span class="sxs-lookup"><span data-stu-id="2e5ca-113">[workbookChartPoint](workbookchartpoint.md) collection</span></span> |<span data-ttu-id="2e5ca-114">Obtenha a coleção de objetos chartPoint.</span><span class="sxs-lookup"><span data-stu-id="2e5ca-114">Get chartPoint object collection.</span></span> |
|[<span data-ttu-id="2e5ca-115">ItemAt</span><span class="sxs-lookup"><span data-stu-id="2e5ca-115">ItemAt</span></span>](../api/chartpointscollection-itemat.md)|[<span data-ttu-id="2e5ca-116">workbookChartPoint</span><span class="sxs-lookup"><span data-stu-id="2e5ca-116">workbookChartPoint</span></span>](workbookchartpoint.md)|<span data-ttu-id="2e5ca-117">Recupera um ponto com base na respectiva posição dentro da série.</span><span class="sxs-lookup"><span data-stu-id="2e5ca-117">Retrieve a point based on its position within the series.</span></span>|

## <a name="properties"></a><span data-ttu-id="2e5ca-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2e5ca-118">Properties</span></span>
| <span data-ttu-id="2e5ca-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2e5ca-119">Property</span></span>     | <span data-ttu-id="2e5ca-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="2e5ca-120">Type</span></span>   |<span data-ttu-id="2e5ca-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="2e5ca-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2e5ca-122">valor</span><span class="sxs-lookup"><span data-stu-id="2e5ca-122">value</span></span>|<span data-ttu-id="2e5ca-123">Json</span><span class="sxs-lookup"><span data-stu-id="2e5ca-123">Json</span></span>|<span data-ttu-id="2e5ca-124">Retorna o valor de um ponto do gráfico.</span><span class="sxs-lookup"><span data-stu-id="2e5ca-124">Returns the value of a chart point.</span></span> <span data-ttu-id="2e5ca-125">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2e5ca-125">Read-only.</span></span>|
|<span data-ttu-id="2e5ca-126">id</span><span class="sxs-lookup"><span data-stu-id="2e5ca-126">id</span></span>|<span data-ttu-id="2e5ca-127">string</span><span class="sxs-lookup"><span data-stu-id="2e5ca-127">string</span></span>|<span data-ttu-id="2e5ca-128">identificador exclusivo</span><span class="sxs-lookup"><span data-stu-id="2e5ca-128">unique identifier</span></span>|

## <a name="relationships"></a><span data-ttu-id="2e5ca-129">Relações</span><span class="sxs-lookup"><span data-stu-id="2e5ca-129">Relationships</span></span>
| <span data-ttu-id="2e5ca-130">Relação</span><span class="sxs-lookup"><span data-stu-id="2e5ca-130">Relationship</span></span> | <span data-ttu-id="2e5ca-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="2e5ca-131">Type</span></span>   |<span data-ttu-id="2e5ca-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="2e5ca-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2e5ca-133">formato</span><span class="sxs-lookup"><span data-stu-id="2e5ca-133">format</span></span>|[<span data-ttu-id="2e5ca-134">workbookChartPointFormat</span><span class="sxs-lookup"><span data-stu-id="2e5ca-134">workbookChartPointFormat</span></span>](workbookchartpointformat.md)|<span data-ttu-id="2e5ca-135">Encapsula as propriedades de formato de um ponto do gráfico.</span><span class="sxs-lookup"><span data-stu-id="2e5ca-135">Encapsulates the format properties chart point.</span></span> <span data-ttu-id="2e5ca-136">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2e5ca-136">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2e5ca-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2e5ca-137">JSON representation</span></span>

<span data-ttu-id="2e5ca-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2e5ca-138">Here is a JSON representation of the resource.</span></span>

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
