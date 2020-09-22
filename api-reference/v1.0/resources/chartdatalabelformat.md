---
title: Tipo de recurso ChartDataLabelFormat
description: Encapsula as propriedades de formato dos rótulos de dados do gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: a1fbb911a546f1ee8fb48f3337d99e3ebe0fcd8d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47988447"
---
# <a name="chartdatalabelformat-resource-type"></a><span data-ttu-id="31ab8-103">Tipo de recurso ChartDataLabelFormat</span><span class="sxs-lookup"><span data-stu-id="31ab8-103">ChartDataLabelFormat resource type</span></span>

<span data-ttu-id="31ab8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="31ab8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="31ab8-105">Encapsula as propriedades de formato dos rótulos de dados do gráfico.</span><span class="sxs-lookup"><span data-stu-id="31ab8-105">Encapsulates the format properties for the chart data labels.</span></span>


## <a name="methods"></a><span data-ttu-id="31ab8-106">Methods</span><span class="sxs-lookup"><span data-stu-id="31ab8-106">Methods</span></span>
<span data-ttu-id="31ab8-107">Nenhum</span><span class="sxs-lookup"><span data-stu-id="31ab8-107">None</span></span>

## <a name="properties"></a><span data-ttu-id="31ab8-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="31ab8-108">Properties</span></span>
<span data-ttu-id="31ab8-109">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="31ab8-109">None</span></span>

## <a name="relationships"></a><span data-ttu-id="31ab8-110">Relações</span><span class="sxs-lookup"><span data-stu-id="31ab8-110">Relationships</span></span>
| <span data-ttu-id="31ab8-111">Relação</span><span class="sxs-lookup"><span data-stu-id="31ab8-111">Relationship</span></span> | <span data-ttu-id="31ab8-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="31ab8-112">Type</span></span>   |<span data-ttu-id="31ab8-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="31ab8-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="31ab8-114">fill</span><span class="sxs-lookup"><span data-stu-id="31ab8-114">fill</span></span>|[<span data-ttu-id="31ab8-115">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="31ab8-115">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="31ab8-p101">Representa o formato de preenchimento do rótulo de dados atual do gráfico. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="31ab8-p101">Represents the fill format of the current chart data label. Read-only.</span></span>|
|<span data-ttu-id="31ab8-118">font</span><span class="sxs-lookup"><span data-stu-id="31ab8-118">font</span></span>|[<span data-ttu-id="31ab8-119">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="31ab8-119">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="31ab8-120">Representa os atributos de fonte do rótulo de dados do gráfico, como nome, tamanho, cor, dentre outros.</span><span class="sxs-lookup"><span data-stu-id="31ab8-120">Represents the font attributes (font name, font size, color, etc.) for a chart data label.</span></span> <span data-ttu-id="31ab8-121">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="31ab8-121">Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="31ab8-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="31ab8-122">JSON representation</span></span>

<span data-ttu-id="31ab8-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="31ab8-123">Here is a JSON representation of the resource.</span></span>

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

