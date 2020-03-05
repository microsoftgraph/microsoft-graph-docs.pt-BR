---
title: tipo de recurso workbookChartAxes
description: Representa os eixos de um gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 89d9a45f0f9e992ac8a93cde6114fc8c9f073359
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519383"
---
# <a name="workbookchartaxes-resource-type"></a><span data-ttu-id="9bd8c-103">tipo de recurso workbookChartAxes</span><span class="sxs-lookup"><span data-stu-id="9bd8c-103">workbookChartAxes resource type</span></span>

<span data-ttu-id="9bd8c-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="9bd8c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9bd8c-105">Representa os eixos de um gráfico.</span><span class="sxs-lookup"><span data-stu-id="9bd8c-105">Represents the chart axes.</span></span>


## <a name="methods"></a><span data-ttu-id="9bd8c-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="9bd8c-106">Methods</span></span>
<span data-ttu-id="9bd8c-107">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9bd8c-107">None</span></span>

## <a name="properties"></a><span data-ttu-id="9bd8c-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9bd8c-108">Properties</span></span>
<span data-ttu-id="9bd8c-109">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="9bd8c-109">None</span></span>

## <a name="relationships"></a><span data-ttu-id="9bd8c-110">Relações</span><span class="sxs-lookup"><span data-stu-id="9bd8c-110">Relationships</span></span>
| <span data-ttu-id="9bd8c-111">Relação</span><span class="sxs-lookup"><span data-stu-id="9bd8c-111">Relationship</span></span> | <span data-ttu-id="9bd8c-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="9bd8c-112">Type</span></span>   |<span data-ttu-id="9bd8c-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="9bd8c-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9bd8c-114">categoryAxis</span><span class="sxs-lookup"><span data-stu-id="9bd8c-114">categoryAxis</span></span>|[<span data-ttu-id="9bd8c-115">workbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="9bd8c-115">workbookChartAxis</span></span>](workbookchartaxis.md)|<span data-ttu-id="9bd8c-p101">Representa o eixo de categoria em um gráfico. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9bd8c-p101">Represents the category axis in a chart. Read-only.</span></span>|
|<span data-ttu-id="9bd8c-118">seriesAxis</span><span class="sxs-lookup"><span data-stu-id="9bd8c-118">seriesAxis</span></span>|[<span data-ttu-id="9bd8c-119">workbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="9bd8c-119">workbookChartAxis</span></span>](workbookchartaxis.md)|<span data-ttu-id="9bd8c-p102">Representa o eixo das séries de um gráfico 3D. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9bd8c-p102">Represents the series axis of a 3-dimensional chart. Read-only.</span></span>|
|<span data-ttu-id="9bd8c-122">valueAxis</span><span class="sxs-lookup"><span data-stu-id="9bd8c-122">valueAxis</span></span>|[<span data-ttu-id="9bd8c-123">workbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="9bd8c-123">workbookChartAxis</span></span>](workbookchartaxis.md)|<span data-ttu-id="9bd8c-124">Representa o eixo dos valores em um eixo.</span><span class="sxs-lookup"><span data-stu-id="9bd8c-124">Represents the value axis in an axis.</span></span> <span data-ttu-id="9bd8c-125">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9bd8c-125">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9bd8c-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9bd8c-126">JSON representation</span></span>

<span data-ttu-id="9bd8c-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9bd8c-127">Here is a JSON representation of the resource.</span></span>

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
