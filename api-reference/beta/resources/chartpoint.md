---
title: Tipo de recurso ChartPoint
description: Representa um ponto de uma série do gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: e8ede39ef53bfc39574ebfc86c8138a70fc31ad6
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573064"
---
# <a name="chartpoint-resource-type"></a><span data-ttu-id="933b7-103">Tipo de recurso ChartPoint</span><span class="sxs-lookup"><span data-stu-id="933b7-103">ChartPoint resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="933b7-104">Representa um ponto de uma série do gráfico.</span><span class="sxs-lookup"><span data-stu-id="933b7-104">Represents a point of a series in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="933b7-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="933b7-105">Methods</span></span>

| <span data-ttu-id="933b7-106">Método</span><span class="sxs-lookup"><span data-stu-id="933b7-106">Method</span></span>           | <span data-ttu-id="933b7-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="933b7-107">Return Type</span></span>    |<span data-ttu-id="933b7-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="933b7-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="933b7-109">Get ChartPoint</span><span class="sxs-lookup"><span data-stu-id="933b7-109">Get ChartPoint</span></span>](../api/chartpoint-get.md) | [<span data-ttu-id="933b7-110">workbookChartPoint</span><span class="sxs-lookup"><span data-stu-id="933b7-110">workbookChartPoint</span></span>](chartpoint.md) |<span data-ttu-id="933b7-111">Leia as propriedades e os relacionamentos do objeto chartPoint.</span><span class="sxs-lookup"><span data-stu-id="933b7-111">Read properties and relationships of chartPoint object.</span></span>|
|[<span data-ttu-id="933b7-112">List</span><span class="sxs-lookup"><span data-stu-id="933b7-112">List</span></span>](../api/chartpoint-list.md) | <span data-ttu-id="933b7-113">coleção [workbookChartPoint](chartpoint.md)</span><span class="sxs-lookup"><span data-stu-id="933b7-113">[workbookChartPoint](chartpoint.md) collection</span></span> |<span data-ttu-id="933b7-114">Obtenha a coleção de objetos chartPoint.</span><span class="sxs-lookup"><span data-stu-id="933b7-114">Get chartPoint object collection.</span></span> |
|[<span data-ttu-id="933b7-115">ItemAt</span><span class="sxs-lookup"><span data-stu-id="933b7-115">ItemAt</span></span>](../api/chartpointscollection-itemat.md)|[<span data-ttu-id="933b7-116">workbookChartPoint</span><span class="sxs-lookup"><span data-stu-id="933b7-116">workbookChartPoint</span></span>](chartpoint.md)|<span data-ttu-id="933b7-117">Recupera um ponto com base na respectiva posição dentro da série.</span><span class="sxs-lookup"><span data-stu-id="933b7-117">Retrieve a point based on its position within the series.</span></span>|

## <a name="properties"></a><span data-ttu-id="933b7-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="933b7-118">Properties</span></span>
| <span data-ttu-id="933b7-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="933b7-119">Property</span></span>     | <span data-ttu-id="933b7-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="933b7-120">Type</span></span>   |<span data-ttu-id="933b7-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="933b7-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="933b7-122">valor</span><span class="sxs-lookup"><span data-stu-id="933b7-122">value</span></span>|<span data-ttu-id="933b7-123">Json</span><span class="sxs-lookup"><span data-stu-id="933b7-123">Json</span></span>|<span data-ttu-id="933b7-p101">Retorna o valor de um ponto do gráfico. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="933b7-p101">Returns the value of a chart point. Read-only.</span></span>|
|<span data-ttu-id="933b7-126">id</span><span class="sxs-lookup"><span data-stu-id="933b7-126">id</span></span>|<span data-ttu-id="933b7-127">string</span><span class="sxs-lookup"><span data-stu-id="933b7-127">string</span></span>|<span data-ttu-id="933b7-128">Identificador exclusivo</span><span class="sxs-lookup"><span data-stu-id="933b7-128">unique identifier</span></span>|

## <a name="relationships"></a><span data-ttu-id="933b7-129">Relações</span><span class="sxs-lookup"><span data-stu-id="933b7-129">Relationships</span></span>
| <span data-ttu-id="933b7-130">Relação</span><span class="sxs-lookup"><span data-stu-id="933b7-130">Relationship</span></span> | <span data-ttu-id="933b7-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="933b7-131">Type</span></span>   |<span data-ttu-id="933b7-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="933b7-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="933b7-133">formato</span><span class="sxs-lookup"><span data-stu-id="933b7-133">format</span></span>|[<span data-ttu-id="933b7-134">workbookChartPointFormat</span><span class="sxs-lookup"><span data-stu-id="933b7-134">workbookChartPointFormat</span></span>](chartpointformat.md)|<span data-ttu-id="933b7-p102">Encapsula as propriedades de formato de um ponto do gráfico. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="933b7-p102">Encapsulates the format properties chart point. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="933b7-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="933b7-137">JSON representation</span></span>

<span data-ttu-id="933b7-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="933b7-138">Here is a JSON representation of the resource.</span></span>

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
