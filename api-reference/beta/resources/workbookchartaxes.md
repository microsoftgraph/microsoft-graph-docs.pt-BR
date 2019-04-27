---
title: tipo de recurso workbookChartAxes
description: Representa os eixos de um gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 15e63af1e7b648288dba813790302f1dee6536ba
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348466"
---
# <a name="workbookchartaxes-resource-type"></a><span data-ttu-id="a49cb-103">tipo de recurso workbookChartAxes</span><span class="sxs-lookup"><span data-stu-id="a49cb-103">workbookChartAxes resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a49cb-104">Representa os eixos de um gráfico.</span><span class="sxs-lookup"><span data-stu-id="a49cb-104">Represents the chart axes.</span></span>


## <a name="methods"></a><span data-ttu-id="a49cb-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="a49cb-105">Methods</span></span>
<span data-ttu-id="a49cb-106">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a49cb-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="a49cb-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a49cb-107">Properties</span></span>
<span data-ttu-id="a49cb-108">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="a49cb-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="a49cb-109">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="a49cb-109">Relationships</span></span>
| <span data-ttu-id="a49cb-110">Relação</span><span class="sxs-lookup"><span data-stu-id="a49cb-110">Relationship</span></span> | <span data-ttu-id="a49cb-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="a49cb-111">Type</span></span>   |<span data-ttu-id="a49cb-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="a49cb-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a49cb-113">categoryAxis</span><span class="sxs-lookup"><span data-stu-id="a49cb-113">categoryAxis</span></span>|[<span data-ttu-id="a49cb-114">workbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="a49cb-114">workbookChartAxis</span></span>](workbookchartaxis.md)|<span data-ttu-id="a49cb-p101">Representa o eixo de categoria em um gráfico. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a49cb-p101">Represents the category axis in a chart. Read-only.</span></span>|
|<span data-ttu-id="a49cb-117">seriesAxis</span><span class="sxs-lookup"><span data-stu-id="a49cb-117">seriesAxis</span></span>|[<span data-ttu-id="a49cb-118">workbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="a49cb-118">workbookChartAxis</span></span>](workbookchartaxis.md)|<span data-ttu-id="a49cb-p102">Representa o eixo das séries de um gráfico 3D. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a49cb-p102">Represents the series axis of a 3-dimensional chart. Read-only.</span></span>|
|<span data-ttu-id="a49cb-121">valueAxis</span><span class="sxs-lookup"><span data-stu-id="a49cb-121">valueAxis</span></span>|[<span data-ttu-id="a49cb-122">workbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="a49cb-122">workbookChartAxis</span></span>](workbookchartaxis.md)|<span data-ttu-id="a49cb-123">Representa o eixo dos valores em um eixo.</span><span class="sxs-lookup"><span data-stu-id="a49cb-123">Represents the value axis in an axis.</span></span> <span data-ttu-id="a49cb-124">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a49cb-124">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a49cb-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a49cb-125">JSON representation</span></span>

<span data-ttu-id="a49cb-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a49cb-126">Here is a JSON representation of the resource.</span></span>

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
