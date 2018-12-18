---
title: Tipo de recurso ChartDataLabelFormat
description: Abrange as propriedades de formatação dos rótulos de dados do gráfico.
author: lumine2008
ms.openlocfilehash: 4c8961eb884a5ab603feda368934795cb73915d0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27356473"
---
# <a name="chartdatalabelformat-resource-type"></a><span data-ttu-id="51875-103">Tipo de recurso ChartDataLabelFormat</span><span class="sxs-lookup"><span data-stu-id="51875-103">ChartDataLabelFormat resource type</span></span>

<span data-ttu-id="51875-104">Abrange as propriedades de formatação dos rótulos de dados do gráfico.</span><span class="sxs-lookup"><span data-stu-id="51875-104">Encapsulates the format properties for the chart data labels.</span></span>


## <a name="methods"></a><span data-ttu-id="51875-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="51875-105">Methods</span></span>
<span data-ttu-id="51875-106">Nenhum</span><span class="sxs-lookup"><span data-stu-id="51875-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="51875-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="51875-107">Properties</span></span>
<span data-ttu-id="51875-108">Nenhum</span><span class="sxs-lookup"><span data-stu-id="51875-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="51875-109">Relações</span><span class="sxs-lookup"><span data-stu-id="51875-109">Relationships</span></span>
| <span data-ttu-id="51875-110">Relação</span><span class="sxs-lookup"><span data-stu-id="51875-110">Relationship</span></span> | <span data-ttu-id="51875-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="51875-111">Type</span></span>   |<span data-ttu-id="51875-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="51875-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="51875-113">fill</span><span class="sxs-lookup"><span data-stu-id="51875-113">fill</span></span>|[<span data-ttu-id="51875-114">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="51875-114">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="51875-p101">Representa o formato de preenchimento do rótulo de dados atual do gráfico. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="51875-p101">Represents the fill format of the current chart data label. Read-only.</span></span>|
|<span data-ttu-id="51875-117">font</span><span class="sxs-lookup"><span data-stu-id="51875-117">font</span></span>|[<span data-ttu-id="51875-118">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="51875-118">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="51875-p102">Representa os atributos de fonte do rótulo de dados do gráfico, como nome, tamanho, cor, dentre outros. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="51875-p102">Represents the font attributes (font name, font size, color, etc.) for a chart data label. Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="51875-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="51875-121">JSON representation</span></span>

<span data-ttu-id="51875-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="51875-122">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "ChartDataLabelFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->