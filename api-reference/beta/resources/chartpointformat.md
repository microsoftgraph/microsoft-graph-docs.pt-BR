---
title: Tipo de recurso ChartPointFormat
description: Representa um objeto de formatação para os pontos do gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 3004577a5ca9687b4bef85f59cfcc8eb528c4a66
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573302"
---
# <a name="chartpointformat-resource-type"></a><span data-ttu-id="4836b-103">Tipo de recurso ChartPointFormat</span><span class="sxs-lookup"><span data-stu-id="4836b-103">ChartPointFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4836b-104">Representa um objeto de formatação para os pontos do gráfico.</span><span class="sxs-lookup"><span data-stu-id="4836b-104">Represents formatting object for chart points.</span></span>


## <a name="methods"></a><span data-ttu-id="4836b-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="4836b-105">Methods</span></span>
<span data-ttu-id="4836b-106">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4836b-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="4836b-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4836b-107">Properties</span></span>
<span data-ttu-id="4836b-108">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4836b-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="4836b-109">Relações</span><span class="sxs-lookup"><span data-stu-id="4836b-109">Relationships</span></span>
| <span data-ttu-id="4836b-110">Relação</span><span class="sxs-lookup"><span data-stu-id="4836b-110">Relationship</span></span> | <span data-ttu-id="4836b-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="4836b-111">Type</span></span>   |<span data-ttu-id="4836b-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="4836b-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4836b-113">fill</span><span class="sxs-lookup"><span data-stu-id="4836b-113">fill</span></span>|[<span data-ttu-id="4836b-114">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="4836b-114">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="4836b-p101">Representa o formato de preenchimento de um gráfico, que inclui informações sobre a formatação da tela de fundo. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4836b-p101">Represents the fill format of a chart, which includes background formating information. Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="4836b-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4836b-117">JSON representation</span></span>

<span data-ttu-id="4836b-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4836b-118">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartPointFormat"
}-->

```json
{
  "fill": {"@odata.type": "microsoft.graph.workbookChartFill"}
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ChartPointFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chartpointformat.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
