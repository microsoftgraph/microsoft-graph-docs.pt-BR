---
title: Tipo de recurso ChartSeriesFormat
description: Abrange as propriedades de formatação da série do gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: c5fdfffdf5bcf6aeefc5068392f689cbf66d683d
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573582"
---
# <a name="chartseriesformat-resource-type"></a><span data-ttu-id="576cb-103">Tipo de recurso ChartSeriesFormat</span><span class="sxs-lookup"><span data-stu-id="576cb-103">ChartSeriesFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="576cb-104">Abrange as propriedades de formatação da série do gráfico.</span><span class="sxs-lookup"><span data-stu-id="576cb-104">encapsulates the format properties for the chart series</span></span>


## <a name="methods"></a><span data-ttu-id="576cb-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="576cb-105">Methods</span></span>
<span data-ttu-id="576cb-106">Nenhum</span><span class="sxs-lookup"><span data-stu-id="576cb-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="576cb-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="576cb-107">Properties</span></span>
<span data-ttu-id="576cb-108">Nenhum</span><span class="sxs-lookup"><span data-stu-id="576cb-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="576cb-109">Relações</span><span class="sxs-lookup"><span data-stu-id="576cb-109">Relationships</span></span>
| <span data-ttu-id="576cb-110">Relação</span><span class="sxs-lookup"><span data-stu-id="576cb-110">Relationship</span></span> | <span data-ttu-id="576cb-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="576cb-111">Type</span></span>   |<span data-ttu-id="576cb-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="576cb-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="576cb-113">fill</span><span class="sxs-lookup"><span data-stu-id="576cb-113">fill</span></span>|[<span data-ttu-id="576cb-114">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="576cb-114">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="576cb-p101">Representa o formato de preenchimento de uma série do gráfico, que inclui informações sobre a formatação da tela de fundo. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="576cb-p101">Represents the fill format of a chart series, which includes background formating information. Read-only.</span></span>|
|<span data-ttu-id="576cb-117">line</span><span class="sxs-lookup"><span data-stu-id="576cb-117">line</span></span>|[<span data-ttu-id="576cb-118">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="576cb-118">WorkbookChartLineFormat</span></span>](chartlineformat.md)|<span data-ttu-id="576cb-p102">Representa a formatação de linha. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="576cb-p102">Represents line formatting. Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="576cb-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="576cb-121">JSON representation</span></span>

<span data-ttu-id="576cb-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="576cb-122">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartSeriesFormat"
}-->

```json
{
  "fill": {"@odata.type": "microsoft.graph.workbookChartFill"},
  "line": {"@odata.type": "microsoft.graph.workbookChartLineFormat"}
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ChartSeriesFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chartseriesformat.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
