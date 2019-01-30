---
title: Tipo de recurso ChartPoint
description: Representa um ponto de uma série do gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 4fd50e2e0b0f289f719dd6636eab16544e6a80f5
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29641964"
---
# <a name="chartpoint-resource-type"></a><span data-ttu-id="18523-103">Tipo de recurso ChartPoint</span><span class="sxs-lookup"><span data-stu-id="18523-103">ChartPoint resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="18523-104">Representa um ponto de uma série do gráfico.</span><span class="sxs-lookup"><span data-stu-id="18523-104">Represents a point of a series in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="18523-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="18523-105">Methods</span></span>

| <span data-ttu-id="18523-106">Método</span><span class="sxs-lookup"><span data-stu-id="18523-106">Method</span></span>           | <span data-ttu-id="18523-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="18523-107">Return Type</span></span>    |<span data-ttu-id="18523-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="18523-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="18523-109">Get ChartPoint</span><span class="sxs-lookup"><span data-stu-id="18523-109">Get ChartPoint</span></span>](../api/chartpoint-get.md) | [<span data-ttu-id="18523-110">ChartPoint</span><span class="sxs-lookup"><span data-stu-id="18523-110">ChartPoint</span></span>](chartpoint.md) |<span data-ttu-id="18523-111">Leia as propriedades e os relacionamentos do objeto chartPoint.</span><span class="sxs-lookup"><span data-stu-id="18523-111">Read properties and relationships of chartPoint object.</span></span>|
|[<span data-ttu-id="18523-112">List</span><span class="sxs-lookup"><span data-stu-id="18523-112">List</span></span>](../api/chartpoint-list.md) | <span data-ttu-id="18523-113">Coleção [ChartPoint](chartpoint.md)</span><span class="sxs-lookup"><span data-stu-id="18523-113">[ChartPoint](chartpoint.md) collection</span></span> |<span data-ttu-id="18523-114">Obtenha a coleção de objetos chartPoint.</span><span class="sxs-lookup"><span data-stu-id="18523-114">Get chartPoint object collection.</span></span> |
|[<span data-ttu-id="18523-115">Itemat</span><span class="sxs-lookup"><span data-stu-id="18523-115">Itemat</span></span>](../api/chartpointscollection-itemat.md)|[<span data-ttu-id="18523-116">ChartPoint</span><span class="sxs-lookup"><span data-stu-id="18523-116">ChartPoint</span></span>](chartpoint.md)|<span data-ttu-id="18523-117">Recupera um ponto com base na respectiva posição dentro da série.</span><span class="sxs-lookup"><span data-stu-id="18523-117">Retrieve a point based on its position within the series.</span></span>|

## <a name="properties"></a><span data-ttu-id="18523-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="18523-118">Properties</span></span>
| <span data-ttu-id="18523-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="18523-119">Property</span></span>     | <span data-ttu-id="18523-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="18523-120">Type</span></span>   |<span data-ttu-id="18523-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="18523-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="18523-122">valor</span><span class="sxs-lookup"><span data-stu-id="18523-122">value</span></span>|<span data-ttu-id="18523-123">object</span><span class="sxs-lookup"><span data-stu-id="18523-123">object</span></span>|<span data-ttu-id="18523-p101">Retorna o valor de um ponto do gráfico. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="18523-p101">Returns the value of a chart point. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="18523-126">Relações</span><span class="sxs-lookup"><span data-stu-id="18523-126">Relationships</span></span>
| <span data-ttu-id="18523-127">Relação</span><span class="sxs-lookup"><span data-stu-id="18523-127">Relationship</span></span> | <span data-ttu-id="18523-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="18523-128">Type</span></span>   |<span data-ttu-id="18523-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="18523-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="18523-130">formato</span><span class="sxs-lookup"><span data-stu-id="18523-130">format</span></span>|[<span data-ttu-id="18523-131">ChartPointFormat</span><span class="sxs-lookup"><span data-stu-id="18523-131">ChartPointFormat</span></span>](chartpointformat.md)|<span data-ttu-id="18523-p102">Encapsula as propriedades de formato de um ponto do gráfico. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="18523-p102">Encapsulates the format properties chart point. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="18523-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="18523-134">JSON representation</span></span>

<span data-ttu-id="18523-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="18523-135">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartPoint"
}-->

```json
{
  "value": "string"
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
  "suppressions": [
    "Error: /api-reference/beta/resources/chartpoint.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
