---
title: Tipo de recurso ChartAxes
description: Representa os eixos de um gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 483a69f11425f3b8991305e6acdf6b970d0e2db1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27976384"
---
# <a name="chartaxes-resource-type"></a><span data-ttu-id="07529-103">Tipo de recurso ChartAxes</span><span class="sxs-lookup"><span data-stu-id="07529-103">ChartAxes resource type</span></span>

<span data-ttu-id="07529-104">Representa os eixos de um gráfico.</span><span class="sxs-lookup"><span data-stu-id="07529-104">Represents the chart axes.</span></span>


## <a name="methods"></a><span data-ttu-id="07529-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="07529-105">Methods</span></span>
<span data-ttu-id="07529-106">Nenhum</span><span class="sxs-lookup"><span data-stu-id="07529-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="07529-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="07529-107">Properties</span></span>
<span data-ttu-id="07529-108">Nenhum</span><span class="sxs-lookup"><span data-stu-id="07529-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="07529-109">Relações</span><span class="sxs-lookup"><span data-stu-id="07529-109">Relationships</span></span>
| <span data-ttu-id="07529-110">Relação</span><span class="sxs-lookup"><span data-stu-id="07529-110">Relationship</span></span> | <span data-ttu-id="07529-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="07529-111">Type</span></span>   |<span data-ttu-id="07529-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="07529-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="07529-113">categoryAxis</span><span class="sxs-lookup"><span data-stu-id="07529-113">categoryAxis</span></span>|[<span data-ttu-id="07529-114">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="07529-114">WorkbookChartAxis</span></span>](chartaxis.md)|<span data-ttu-id="07529-p101">Representa o eixo de categoria em um gráfico. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="07529-p101">Represents the category axis in a chart. Read-only.</span></span>|
|<span data-ttu-id="07529-117">seriesAxis</span><span class="sxs-lookup"><span data-stu-id="07529-117">seriesAxis</span></span>|[<span data-ttu-id="07529-118">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="07529-118">WorkbookChartAxis</span></span>](chartaxis.md)|<span data-ttu-id="07529-p102">Representa o eixo das séries de um gráfico 3D. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="07529-p102">Represents the series axis of a 3-dimensional chart. Read-only.</span></span>|
|<span data-ttu-id="07529-121">valueAxis</span><span class="sxs-lookup"><span data-stu-id="07529-121">valueAxis</span></span>|[<span data-ttu-id="07529-122">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="07529-122">WorkbookChartAxis</span></span>](chartaxis.md)|<span data-ttu-id="07529-p103">Representa o eixo dos valores em um eixo. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="07529-p103">Represents the value axis in an axis. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="07529-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="07529-125">JSON representation</span></span>

<span data-ttu-id="07529-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="07529-126">Here is a JSON representation of the resource.</span></span>

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
