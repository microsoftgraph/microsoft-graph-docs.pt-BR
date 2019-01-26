---
title: Tipo de recurso ChartDataLabelFormat
description: Abrange as propriedades de formatação dos rótulos de dados do gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: a82e88bd8ba083271a821dc86435b0ce55364cec
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572602"
---
# <a name="chartdatalabelformat-resource-type"></a><span data-ttu-id="aee19-103">Tipo de recurso ChartDataLabelFormat</span><span class="sxs-lookup"><span data-stu-id="aee19-103">ChartDataLabelFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aee19-104">Abrange as propriedades de formatação dos rótulos de dados do gráfico.</span><span class="sxs-lookup"><span data-stu-id="aee19-104">Encapsulates the format properties for the chart data labels.</span></span>


## <a name="methods"></a><span data-ttu-id="aee19-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="aee19-105">Methods</span></span>
<span data-ttu-id="aee19-106">Nenhum</span><span class="sxs-lookup"><span data-stu-id="aee19-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="aee19-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="aee19-107">Properties</span></span>
<span data-ttu-id="aee19-108">Nenhum</span><span class="sxs-lookup"><span data-stu-id="aee19-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="aee19-109">Relações</span><span class="sxs-lookup"><span data-stu-id="aee19-109">Relationships</span></span>
| <span data-ttu-id="aee19-110">Relação</span><span class="sxs-lookup"><span data-stu-id="aee19-110">Relationship</span></span> | <span data-ttu-id="aee19-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="aee19-111">Type</span></span>   |<span data-ttu-id="aee19-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="aee19-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aee19-113">fill</span><span class="sxs-lookup"><span data-stu-id="aee19-113">fill</span></span>|[<span data-ttu-id="aee19-114">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="aee19-114">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="aee19-p101">Representa o formato de preenchimento do rótulo de dados atual do gráfico. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="aee19-p101">Represents the fill format of the current chart data label. Read-only.</span></span>|
|<span data-ttu-id="aee19-117">font</span><span class="sxs-lookup"><span data-stu-id="aee19-117">font</span></span>|[<span data-ttu-id="aee19-118">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="aee19-118">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="aee19-p102">Representa os atributos de fonte do rótulo de dados do gráfico, como nome, tamanho, cor, dentre outros. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="aee19-p102">Represents the font attributes (font name, font size, color, etc.) for a chart data label. Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="aee19-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="aee19-121">JSON representation</span></span>

<span data-ttu-id="aee19-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="aee19-122">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartDataLabelFormat"
}-->

```json
{
  "fill": {"@odata.type": "microsoft.graph.workbookChartFill"},
  "font": {"@odata.type": "microsoft.graph.workbookChartFont"}
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ChartDataLabelFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chartdatalabelformat.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
