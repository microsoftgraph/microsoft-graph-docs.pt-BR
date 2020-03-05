---
title: tipo de recurso workbookChartSeriesFormat
description: Abrange as propriedades de formatação da série do gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 2558d242e18fa8bf7d220ba5bc4dd8aef6cd2865
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519264"
---
# <a name="workbookchartseriesformat-resource-type"></a><span data-ttu-id="7df7b-103">tipo de recurso workbookChartSeriesFormat</span><span class="sxs-lookup"><span data-stu-id="7df7b-103">workbookChartSeriesFormat resource type</span></span>

<span data-ttu-id="7df7b-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="7df7b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7df7b-105">Encapsula as propriedades de formato da série do gráfico.</span><span class="sxs-lookup"><span data-stu-id="7df7b-105">Encapsulates the format properties for the chart series.</span></span>


## <a name="methods"></a><span data-ttu-id="7df7b-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="7df7b-106">Methods</span></span>
<span data-ttu-id="7df7b-107">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7df7b-107">None</span></span>

## <a name="properties"></a><span data-ttu-id="7df7b-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7df7b-108">Properties</span></span>
<span data-ttu-id="7df7b-109">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="7df7b-109">None</span></span>

## <a name="relationships"></a><span data-ttu-id="7df7b-110">Relações</span><span class="sxs-lookup"><span data-stu-id="7df7b-110">Relationships</span></span>
| <span data-ttu-id="7df7b-111">Relação</span><span class="sxs-lookup"><span data-stu-id="7df7b-111">Relationship</span></span> | <span data-ttu-id="7df7b-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="7df7b-112">Type</span></span>   |<span data-ttu-id="7df7b-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="7df7b-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7df7b-114">fill</span><span class="sxs-lookup"><span data-stu-id="7df7b-114">fill</span></span>|[<span data-ttu-id="7df7b-115">workbookChartFill</span><span class="sxs-lookup"><span data-stu-id="7df7b-115">workbookChartFill</span></span>](workbookchartfill.md)|<span data-ttu-id="7df7b-p101">Representa o formato de preenchimento de uma série do gráfico, que inclui informações sobre a formatação da tela de fundo. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7df7b-p101">Represents the fill format of a chart series, which includes background formating information. Read-only.</span></span>|
|<span data-ttu-id="7df7b-118">line</span><span class="sxs-lookup"><span data-stu-id="7df7b-118">line</span></span>|[<span data-ttu-id="7df7b-119">workbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="7df7b-119">workbookChartLineFormat</span></span>](workbookchartlineformat.md)|<span data-ttu-id="7df7b-120">Representa a formatação de linha.</span><span class="sxs-lookup"><span data-stu-id="7df7b-120">Represents line formatting.</span></span> <span data-ttu-id="7df7b-121">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7df7b-121">Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="7df7b-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7df7b-122">JSON representation</span></span>

<span data-ttu-id="7df7b-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7df7b-123">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
