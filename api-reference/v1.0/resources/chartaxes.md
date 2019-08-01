---
title: Tipo de recurso ChartAxes
description: Representa os eixos de um gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 7e8ee5eac8face4d16418799d627d3aa168c48c2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029873"
---
# <a name="chartaxes-resource-type"></a><span data-ttu-id="414f5-103">Tipo de recurso ChartAxes</span><span class="sxs-lookup"><span data-stu-id="414f5-103">ChartAxes resource type</span></span>

<span data-ttu-id="414f5-104">Representa os eixos de um gráfico.</span><span class="sxs-lookup"><span data-stu-id="414f5-104">Represents the chart axes.</span></span>


## <a name="methods"></a><span data-ttu-id="414f5-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="414f5-105">Methods</span></span>
<span data-ttu-id="414f5-106">Nenhum</span><span class="sxs-lookup"><span data-stu-id="414f5-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="414f5-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="414f5-107">Properties</span></span>
<span data-ttu-id="414f5-108">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="414f5-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="414f5-109">Relações</span><span class="sxs-lookup"><span data-stu-id="414f5-109">Relationships</span></span>
| <span data-ttu-id="414f5-110">Relação</span><span class="sxs-lookup"><span data-stu-id="414f5-110">Relationship</span></span> | <span data-ttu-id="414f5-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="414f5-111">Type</span></span>   |<span data-ttu-id="414f5-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="414f5-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="414f5-113">categoryAxis</span><span class="sxs-lookup"><span data-stu-id="414f5-113">categoryAxis</span></span>|[<span data-ttu-id="414f5-114">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="414f5-114">WorkbookChartAxis</span></span>](chartaxis.md)|<span data-ttu-id="414f5-p101">Representa o eixo de categoria em um gráfico. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="414f5-p101">Represents the category axis in a chart. Read-only.</span></span>|
|<span data-ttu-id="414f5-117">seriesAxis</span><span class="sxs-lookup"><span data-stu-id="414f5-117">seriesAxis</span></span>|[<span data-ttu-id="414f5-118">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="414f5-118">WorkbookChartAxis</span></span>](chartaxis.md)|<span data-ttu-id="414f5-p102">Representa o eixo das séries de um gráfico 3D. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="414f5-p102">Represents the series axis of a 3-dimensional chart. Read-only.</span></span>|
|<span data-ttu-id="414f5-121">valueAxis</span><span class="sxs-lookup"><span data-stu-id="414f5-121">valueAxis</span></span>|[<span data-ttu-id="414f5-122">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="414f5-122">WorkbookChartAxis</span></span>](chartaxis.md)|<span data-ttu-id="414f5-123">Representa o eixo dos valores em um eixo.</span><span class="sxs-lookup"><span data-stu-id="414f5-123">Represents the value axis in an axis.</span></span> <span data-ttu-id="414f5-124">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="414f5-124">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="414f5-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="414f5-125">JSON representation</span></span>

<span data-ttu-id="414f5-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="414f5-126">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartAxes"
}-->

```json
{
  "categoryAxis": {"@odata.type": "microsoft.graph.workbookChartAxis"},
  "seriesAxis": {"@odata.type": "microsoft.graph.workbookChartAxis"},
  "valueAxis": {"@odata.type": "microsoft.graph.workbookChartAxis"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartAxes resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
