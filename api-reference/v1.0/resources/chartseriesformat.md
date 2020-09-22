---
title: Tipo de recurso ChartSeriesFormat
description: Abrange as propriedades de formatação da série do gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 3b6003df060fbb657dc3c67375f2c942ad8cff57
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48059226"
---
# <a name="chartseriesformat-resource-type"></a><span data-ttu-id="3b32f-103">Tipo de recurso ChartSeriesFormat</span><span class="sxs-lookup"><span data-stu-id="3b32f-103">ChartSeriesFormat resource type</span></span>

<span data-ttu-id="3b32f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3b32f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3b32f-105">Abrange as propriedades de formatação da série do gráfico.</span><span class="sxs-lookup"><span data-stu-id="3b32f-105">encapsulates the format properties for the chart series</span></span>


## <a name="methods"></a><span data-ttu-id="3b32f-106">Methods</span><span class="sxs-lookup"><span data-stu-id="3b32f-106">Methods</span></span>
<span data-ttu-id="3b32f-107">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3b32f-107">None</span></span>

## <a name="properties"></a><span data-ttu-id="3b32f-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3b32f-108">Properties</span></span>
<span data-ttu-id="3b32f-109">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="3b32f-109">None</span></span>

## <a name="relationships"></a><span data-ttu-id="3b32f-110">Relações</span><span class="sxs-lookup"><span data-stu-id="3b32f-110">Relationships</span></span>
| <span data-ttu-id="3b32f-111">Relação</span><span class="sxs-lookup"><span data-stu-id="3b32f-111">Relationship</span></span> | <span data-ttu-id="3b32f-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="3b32f-112">Type</span></span>   |<span data-ttu-id="3b32f-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="3b32f-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3b32f-114">fill</span><span class="sxs-lookup"><span data-stu-id="3b32f-114">fill</span></span>|[<span data-ttu-id="3b32f-115">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="3b32f-115">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="3b32f-p101">Representa o formato de preenchimento de uma série do gráfico, que inclui informações sobre a formatação da tela de fundo. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3b32f-p101">Represents the fill format of a chart series, which includes background formating information. Read-only.</span></span>|
|<span data-ttu-id="3b32f-118">line</span><span class="sxs-lookup"><span data-stu-id="3b32f-118">line</span></span>|[<span data-ttu-id="3b32f-119">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="3b32f-119">WorkbookChartLineFormat</span></span>](chartlineformat.md)|<span data-ttu-id="3b32f-120">Representa a formatação de linha.</span><span class="sxs-lookup"><span data-stu-id="3b32f-120">Represents line formatting.</span></span> <span data-ttu-id="3b32f-121">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3b32f-121">Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="3b32f-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3b32f-122">JSON representation</span></span>

<span data-ttu-id="3b32f-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3b32f-123">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "ChartSeriesFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

