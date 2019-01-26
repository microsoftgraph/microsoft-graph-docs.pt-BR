---
title: Tipo de recurso ChartGridlinesFormat
description: Abrange as propriedades de formatação das linhas de grade do gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: cf2e9f1202774cc971cc09a2ce1904df2e1fb5a2
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573281"
---
# <a name="chartgridlinesformat-resource-type"></a><span data-ttu-id="df407-103">Tipo de recurso ChartGridlinesFormat</span><span class="sxs-lookup"><span data-stu-id="df407-103">ChartGridlinesFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="df407-104">Abrange as propriedades de formatação das linhas de grade do gráfico.</span><span class="sxs-lookup"><span data-stu-id="df407-104">Encapsulates the format properties for chart gridlines.</span></span>


## <a name="methods"></a><span data-ttu-id="df407-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="df407-105">Methods</span></span>
<span data-ttu-id="df407-106">Nenhum</span><span class="sxs-lookup"><span data-stu-id="df407-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="df407-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="df407-107">Properties</span></span>
<span data-ttu-id="df407-108">Nenhum</span><span class="sxs-lookup"><span data-stu-id="df407-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="df407-109">Relações</span><span class="sxs-lookup"><span data-stu-id="df407-109">Relationships</span></span>
| <span data-ttu-id="df407-110">Relação</span><span class="sxs-lookup"><span data-stu-id="df407-110">Relationship</span></span> | <span data-ttu-id="df407-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="df407-111">Type</span></span>   |<span data-ttu-id="df407-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="df407-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="df407-113">line</span><span class="sxs-lookup"><span data-stu-id="df407-113">line</span></span>|[<span data-ttu-id="df407-114">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="df407-114">WorkbookChartLineFormat</span></span>](chartlineformat.md)|<span data-ttu-id="df407-p101">Representa a formatação de linha do gráfico. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="df407-p101">Represents chart line formatting. Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="df407-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="df407-117">JSON representation</span></span>

<span data-ttu-id="df407-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="df407-118">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartGridlinesFormat"
}-->

```json
{
  "line": {"@odata.type": "microsoft.graph.workbookChartLineFormat"}
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ChartGridlinesFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chartgridlinesformat.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
