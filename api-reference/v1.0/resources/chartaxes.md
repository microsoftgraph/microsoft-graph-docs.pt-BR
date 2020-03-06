---
title: Tipo de recurso ChartAxes
description: Representa os eixos de um gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: a5a33108de8225e3222ecea74afa3c0d9f1caa4b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531912"
---
# <a name="chartaxes-resource-type"></a><span data-ttu-id="de1a9-103">Tipo de recurso ChartAxes</span><span class="sxs-lookup"><span data-stu-id="de1a9-103">ChartAxes resource type</span></span>

<span data-ttu-id="de1a9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="de1a9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="de1a9-105">Representa os eixos de um gráfico.</span><span class="sxs-lookup"><span data-stu-id="de1a9-105">Represents the chart axes.</span></span>


## <a name="methods"></a><span data-ttu-id="de1a9-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="de1a9-106">Methods</span></span>
<span data-ttu-id="de1a9-107">Nenhum</span><span class="sxs-lookup"><span data-stu-id="de1a9-107">None</span></span>

## <a name="properties"></a><span data-ttu-id="de1a9-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="de1a9-108">Properties</span></span>
<span data-ttu-id="de1a9-109">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="de1a9-109">None</span></span>

## <a name="relationships"></a><span data-ttu-id="de1a9-110">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="de1a9-110">Relationships</span></span>
| <span data-ttu-id="de1a9-111">Relação</span><span class="sxs-lookup"><span data-stu-id="de1a9-111">Relationship</span></span> | <span data-ttu-id="de1a9-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="de1a9-112">Type</span></span>   |<span data-ttu-id="de1a9-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="de1a9-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="de1a9-114">categoryAxis</span><span class="sxs-lookup"><span data-stu-id="de1a9-114">categoryAxis</span></span>|[<span data-ttu-id="de1a9-115">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="de1a9-115">WorkbookChartAxis</span></span>](chartaxis.md)|<span data-ttu-id="de1a9-p101">Representa o eixo de categoria em um gráfico. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="de1a9-p101">Represents the category axis in a chart. Read-only.</span></span>|
|<span data-ttu-id="de1a9-118">seriesAxis</span><span class="sxs-lookup"><span data-stu-id="de1a9-118">seriesAxis</span></span>|[<span data-ttu-id="de1a9-119">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="de1a9-119">WorkbookChartAxis</span></span>](chartaxis.md)|<span data-ttu-id="de1a9-p102">Representa o eixo das séries de um gráfico 3D. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="de1a9-p102">Represents the series axis of a 3-dimensional chart. Read-only.</span></span>|
|<span data-ttu-id="de1a9-122">valueAxis</span><span class="sxs-lookup"><span data-stu-id="de1a9-122">valueAxis</span></span>|[<span data-ttu-id="de1a9-123">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="de1a9-123">WorkbookChartAxis</span></span>](chartaxis.md)|<span data-ttu-id="de1a9-124">Representa o eixo dos valores em um eixo.</span><span class="sxs-lookup"><span data-stu-id="de1a9-124">Represents the value axis in an axis.</span></span> <span data-ttu-id="de1a9-125">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="de1a9-125">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="de1a9-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="de1a9-126">JSON representation</span></span>

<span data-ttu-id="de1a9-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="de1a9-127">Here is a JSON representation of the resource.</span></span>

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
