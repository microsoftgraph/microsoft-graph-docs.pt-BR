---
title: Tipo de recurso ChartPoint
description: Representa o ponto de uma série do gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 4fd50e2e0b0f289f719dd6636eab16544e6a80f5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32460916"
---
# <a name="chartpoint-resource-type"></a><span data-ttu-id="434cb-103">Tipo de recurso ChartPoint</span><span class="sxs-lookup"><span data-stu-id="434cb-103">ChartPoint resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="434cb-104">Representa o ponto de uma série do gráfico.</span><span class="sxs-lookup"><span data-stu-id="434cb-104">Represents a point of a series in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="434cb-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="434cb-105">Methods</span></span>

| <span data-ttu-id="434cb-106">Método</span><span class="sxs-lookup"><span data-stu-id="434cb-106">Method</span></span>           | <span data-ttu-id="434cb-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="434cb-107">Return Type</span></span>    |<span data-ttu-id="434cb-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="434cb-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="434cb-109">Get ChartPoint</span><span class="sxs-lookup"><span data-stu-id="434cb-109">Get ChartPoint</span></span>](../api/chartpoint-get.md) | [<span data-ttu-id="434cb-110">ChartPoint</span><span class="sxs-lookup"><span data-stu-id="434cb-110">ChartPoint</span></span>](chartpoint.md) |<span data-ttu-id="434cb-111">Leia as propriedades e os relacionamentos do objeto chartPoint.</span><span class="sxs-lookup"><span data-stu-id="434cb-111">Read properties and relationships of chartPoint object.</span></span>|
|[<span data-ttu-id="434cb-112">List</span><span class="sxs-lookup"><span data-stu-id="434cb-112">List</span></span>](../api/chartpoint-list.md) | <span data-ttu-id="434cb-113">Coleção [ChartPoint](chartpoint.md)</span><span class="sxs-lookup"><span data-stu-id="434cb-113">[ChartPoint](chartpoint.md) collection</span></span> |<span data-ttu-id="434cb-114">Obtenha a coleção de objetos chartPoint.</span><span class="sxs-lookup"><span data-stu-id="434cb-114">Get chartPoint object collection.</span></span> |
|[<span data-ttu-id="434cb-115">Itemat</span><span class="sxs-lookup"><span data-stu-id="434cb-115">Itemat</span></span>](../api/chartpointscollection-itemat.md)|[<span data-ttu-id="434cb-116">ChartPoint</span><span class="sxs-lookup"><span data-stu-id="434cb-116">ChartPoint</span></span>](chartpoint.md)|<span data-ttu-id="434cb-117">Recupera um ponto com base na respectiva posição dentro da série.</span><span class="sxs-lookup"><span data-stu-id="434cb-117">Retrieve a point based on its position within the series.</span></span>|

## <a name="properties"></a><span data-ttu-id="434cb-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="434cb-118">Properties</span></span>
| <span data-ttu-id="434cb-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="434cb-119">Property</span></span>     | <span data-ttu-id="434cb-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="434cb-120">Type</span></span>   |<span data-ttu-id="434cb-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="434cb-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="434cb-122">valor</span><span class="sxs-lookup"><span data-stu-id="434cb-122">value</span></span>|<span data-ttu-id="434cb-123">objeto</span><span class="sxs-lookup"><span data-stu-id="434cb-123">object</span></span>|<span data-ttu-id="434cb-p101">Retorna o valor de um ponto do gráfico. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="434cb-p101">Returns the value of a chart point. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="434cb-126">Relações</span><span class="sxs-lookup"><span data-stu-id="434cb-126">Relationships</span></span>
| <span data-ttu-id="434cb-127">Relação</span><span class="sxs-lookup"><span data-stu-id="434cb-127">Relationship</span></span> | <span data-ttu-id="434cb-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="434cb-128">Type</span></span>   |<span data-ttu-id="434cb-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="434cb-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="434cb-130">format</span><span class="sxs-lookup"><span data-stu-id="434cb-130">format</span></span>|[<span data-ttu-id="434cb-131">ChartPointFormat</span><span class="sxs-lookup"><span data-stu-id="434cb-131">ChartPointFormat</span></span>](chartpointformat.md)|<span data-ttu-id="434cb-p102">Encapsula as propriedades de formato de um ponto do gráfico. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="434cb-p102">Encapsulates the format properties chart point. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="434cb-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="434cb-134">JSON representation</span></span>

<span data-ttu-id="434cb-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="434cb-135">Here is a JSON representation of the resource.</span></span>

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
