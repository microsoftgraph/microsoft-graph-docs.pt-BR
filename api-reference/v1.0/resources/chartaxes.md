---
title: Tipo de recurso ChartAxes
description: Representa os eixos de um gráfico.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 53f0e4a7344ddfab89330203f90032266e0c622d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27885901"
---
# <a name="chartaxes-resource-type"></a><span data-ttu-id="4336e-103">Tipo de recurso ChartAxes</span><span class="sxs-lookup"><span data-stu-id="4336e-103">ChartAxes resource type</span></span>

<span data-ttu-id="4336e-104">Representa os eixos de um gráfico.</span><span class="sxs-lookup"><span data-stu-id="4336e-104">Represents the chart axes.</span></span>


## <a name="methods"></a><span data-ttu-id="4336e-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="4336e-105">Methods</span></span>
<span data-ttu-id="4336e-106">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4336e-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="4336e-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4336e-107">Properties</span></span>
<span data-ttu-id="4336e-108">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4336e-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="4336e-109">Relações</span><span class="sxs-lookup"><span data-stu-id="4336e-109">Relationships</span></span>
| <span data-ttu-id="4336e-110">Relação</span><span class="sxs-lookup"><span data-stu-id="4336e-110">Relationship</span></span> | <span data-ttu-id="4336e-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="4336e-111">Type</span></span>   |<span data-ttu-id="4336e-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="4336e-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4336e-113">categoryAxis</span><span class="sxs-lookup"><span data-stu-id="4336e-113">categoryAxis</span></span>|[<span data-ttu-id="4336e-114">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="4336e-114">WorkbookChartAxis</span></span>](chartaxis.md)|<span data-ttu-id="4336e-p101">Representa o eixo de categoria em um gráfico. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4336e-p101">Represents the category axis in a chart. Read-only.</span></span>|
|<span data-ttu-id="4336e-117">seriesAxis</span><span class="sxs-lookup"><span data-stu-id="4336e-117">seriesAxis</span></span>|[<span data-ttu-id="4336e-118">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="4336e-118">WorkbookChartAxis</span></span>](chartaxis.md)|<span data-ttu-id="4336e-p102">Representa o eixo das séries de um gráfico 3D. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4336e-p102">Represents the series axis of a 3-dimensional chart. Read-only.</span></span>|
|<span data-ttu-id="4336e-121">valueAxis</span><span class="sxs-lookup"><span data-stu-id="4336e-121">valueAxis</span></span>|[<span data-ttu-id="4336e-122">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="4336e-122">WorkbookChartAxis</span></span>](chartaxis.md)|<span data-ttu-id="4336e-p103">Representa o eixo dos valores em um eixo. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4336e-p103">Represents the value axis in an axis. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4336e-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4336e-125">JSON representation</span></span>

<span data-ttu-id="4336e-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4336e-126">Here is a JSON representation of the resource.</span></span>

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
