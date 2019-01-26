---
title: Tipo de recurso ChartAxisFormat
description: Abrange as propriedades de formatação do eixo do gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 587c35f0bf28d695f67e61a8eefa1593317a8d5d
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29577106"
---
# <a name="chartaxisformat-resource-type"></a><span data-ttu-id="094f7-103">Tipo de recurso ChartAxisFormat</span><span class="sxs-lookup"><span data-stu-id="094f7-103">ChartAxisFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="094f7-104">Abrange as propriedades de formatação do eixo do gráfico.</span><span class="sxs-lookup"><span data-stu-id="094f7-104">Encapsulates the format properties for the chart axis.</span></span>


## <a name="methods"></a><span data-ttu-id="094f7-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="094f7-105">Methods</span></span>
<span data-ttu-id="094f7-106">Nenhum</span><span class="sxs-lookup"><span data-stu-id="094f7-106">None</span></span>
## <a name="properties"></a><span data-ttu-id="094f7-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="094f7-107">Properties</span></span>
<span data-ttu-id="094f7-108">Nenhum</span><span class="sxs-lookup"><span data-stu-id="094f7-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="094f7-109">Relações</span><span class="sxs-lookup"><span data-stu-id="094f7-109">Relationships</span></span>
| <span data-ttu-id="094f7-110">Relação</span><span class="sxs-lookup"><span data-stu-id="094f7-110">Relationship</span></span> | <span data-ttu-id="094f7-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="094f7-111">Type</span></span>   |<span data-ttu-id="094f7-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="094f7-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="094f7-113">font</span><span class="sxs-lookup"><span data-stu-id="094f7-113">font</span></span>|[<span data-ttu-id="094f7-114">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="094f7-114">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="094f7-p101">Representa os atributos de fonte de um elemento do eixo do gráfico, como nome, tamanho, cor, etc. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="094f7-p101">Represents the font attributes (font name, font size, color, etc.) for a chart axis element. Read-only.</span></span>|
|<span data-ttu-id="094f7-117">line</span><span class="sxs-lookup"><span data-stu-id="094f7-117">line</span></span>|[<span data-ttu-id="094f7-118">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="094f7-118">WorkbookChartLineFormat</span></span>](chartlineformat.md)|<span data-ttu-id="094f7-p102">Representa a formatação de linha do gráfico. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="094f7-p102">Represents chart line formatting. Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="094f7-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="094f7-121">JSON representation</span></span>

<span data-ttu-id="094f7-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="094f7-122">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartAxisFormat"
}-->

```json
{
  "font": {"@odata.type": "microsoft.graph.workbookChartFont"},
  "line": {"@odata.type": "microsoft.graph.workbookChartLineFormat"}
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ChartAxisFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chartaxisformat.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
