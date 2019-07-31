---
title: tipo de recurso workbookChartAxes
description: Representa os eixos de um gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: e7cd34ab250f5232d1620af3b3be4fe36c286f41
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964078"
---
# <a name="workbookchartaxes-resource-type"></a><span data-ttu-id="e291c-103">tipo de recurso workbookChartAxes</span><span class="sxs-lookup"><span data-stu-id="e291c-103">workbookChartAxes resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e291c-104">Representa os eixos de um gráfico.</span><span class="sxs-lookup"><span data-stu-id="e291c-104">Represents the chart axes.</span></span>


## <a name="methods"></a><span data-ttu-id="e291c-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="e291c-105">Methods</span></span>
<span data-ttu-id="e291c-106">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e291c-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="e291c-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e291c-107">Properties</span></span>
<span data-ttu-id="e291c-108">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="e291c-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="e291c-109">Relações</span><span class="sxs-lookup"><span data-stu-id="e291c-109">Relationships</span></span>
| <span data-ttu-id="e291c-110">Relação</span><span class="sxs-lookup"><span data-stu-id="e291c-110">Relationship</span></span> | <span data-ttu-id="e291c-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="e291c-111">Type</span></span>   |<span data-ttu-id="e291c-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="e291c-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e291c-113">categoryAxis</span><span class="sxs-lookup"><span data-stu-id="e291c-113">categoryAxis</span></span>|[<span data-ttu-id="e291c-114">workbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="e291c-114">workbookChartAxis</span></span>](workbookchartaxis.md)|<span data-ttu-id="e291c-p101">Representa o eixo de categoria em um gráfico. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e291c-p101">Represents the category axis in a chart. Read-only.</span></span>|
|<span data-ttu-id="e291c-117">seriesAxis</span><span class="sxs-lookup"><span data-stu-id="e291c-117">seriesAxis</span></span>|[<span data-ttu-id="e291c-118">workbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="e291c-118">workbookChartAxis</span></span>](workbookchartaxis.md)|<span data-ttu-id="e291c-p102">Representa o eixo das séries de um gráfico 3D. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e291c-p102">Represents the series axis of a 3-dimensional chart. Read-only.</span></span>|
|<span data-ttu-id="e291c-121">valueAxis</span><span class="sxs-lookup"><span data-stu-id="e291c-121">valueAxis</span></span>|[<span data-ttu-id="e291c-122">workbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="e291c-122">workbookChartAxis</span></span>](workbookchartaxis.md)|<span data-ttu-id="e291c-123">Representa o eixo dos valores em um eixo.</span><span class="sxs-lookup"><span data-stu-id="e291c-123">Represents the value axis in an axis.</span></span> <span data-ttu-id="e291c-124">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e291c-124">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e291c-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e291c-125">JSON representation</span></span>

<span data-ttu-id="e291c-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e291c-126">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "ChartAxes resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
