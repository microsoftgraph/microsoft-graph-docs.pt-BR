---
title: Tipo de recurso ChartAxes
description: Representa os eixos de um gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: f2a3744e38ffebef0c28784c0fd4be8f35b8af23
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29570859"
---
# <a name="chartaxes-resource-type"></a><span data-ttu-id="f9b0e-103">Tipo de recurso ChartAxes</span><span class="sxs-lookup"><span data-stu-id="f9b0e-103">ChartAxes resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f9b0e-104">Representa os eixos de um gráfico.</span><span class="sxs-lookup"><span data-stu-id="f9b0e-104">Represents the chart axes.</span></span>


## <a name="methods"></a><span data-ttu-id="f9b0e-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="f9b0e-105">Methods</span></span>
<span data-ttu-id="f9b0e-106">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f9b0e-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="f9b0e-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f9b0e-107">Properties</span></span>
<span data-ttu-id="f9b0e-108">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f9b0e-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="f9b0e-109">Relações</span><span class="sxs-lookup"><span data-stu-id="f9b0e-109">Relationships</span></span>
| <span data-ttu-id="f9b0e-110">Relação</span><span class="sxs-lookup"><span data-stu-id="f9b0e-110">Relationship</span></span> | <span data-ttu-id="f9b0e-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="f9b0e-111">Type</span></span>   |<span data-ttu-id="f9b0e-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="f9b0e-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f9b0e-113">categoryAxis</span><span class="sxs-lookup"><span data-stu-id="f9b0e-113">categoryAxis</span></span>|[<span data-ttu-id="f9b0e-114">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="f9b0e-114">WorkbookChartAxis</span></span>](chartaxis.md)|<span data-ttu-id="f9b0e-p101">Representa o eixo de categoria em um gráfico. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9b0e-p101">Represents the category axis in a chart. Read-only.</span></span>|
|<span data-ttu-id="f9b0e-117">seriesAxis</span><span class="sxs-lookup"><span data-stu-id="f9b0e-117">seriesAxis</span></span>|[<span data-ttu-id="f9b0e-118">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="f9b0e-118">WorkbookChartAxis</span></span>](chartaxis.md)|<span data-ttu-id="f9b0e-p102">Representa o eixo das séries de um gráfico 3D. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9b0e-p102">Represents the series axis of a 3-dimensional chart. Read-only.</span></span>|
|<span data-ttu-id="f9b0e-121">valueAxis</span><span class="sxs-lookup"><span data-stu-id="f9b0e-121">valueAxis</span></span>|[<span data-ttu-id="f9b0e-122">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="f9b0e-122">WorkbookChartAxis</span></span>](chartaxis.md)|<span data-ttu-id="f9b0e-p103">Representa o eixo dos valores em um eixo. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9b0e-p103">Represents the value axis in an axis. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f9b0e-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f9b0e-125">JSON representation</span></span>

<span data-ttu-id="f9b0e-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f9b0e-126">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/chartaxes.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
