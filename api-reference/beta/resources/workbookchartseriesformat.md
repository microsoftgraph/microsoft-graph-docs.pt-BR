---
title: tipo de recurso workbookChartSeriesFormat
description: Abrange as propriedades de formatação da série do gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: fd69add38af420b1ac2393a71d1dd490ed3a481d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48089270"
---
# <a name="workbookchartseriesformat-resource-type"></a><span data-ttu-id="6e55d-103">tipo de recurso workbookChartSeriesFormat</span><span class="sxs-lookup"><span data-stu-id="6e55d-103">workbookChartSeriesFormat resource type</span></span>

<span data-ttu-id="6e55d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6e55d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6e55d-105">Encapsula as propriedades de formato da série do gráfico.</span><span class="sxs-lookup"><span data-stu-id="6e55d-105">Encapsulates the format properties for the chart series.</span></span>


## <a name="methods"></a><span data-ttu-id="6e55d-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="6e55d-106">Methods</span></span>
<span data-ttu-id="6e55d-107">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6e55d-107">None</span></span>

## <a name="properties"></a><span data-ttu-id="6e55d-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6e55d-108">Properties</span></span>
<span data-ttu-id="6e55d-109">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="6e55d-109">None</span></span>

## <a name="relationships"></a><span data-ttu-id="6e55d-110">Relações</span><span class="sxs-lookup"><span data-stu-id="6e55d-110">Relationships</span></span>
| <span data-ttu-id="6e55d-111">Relação</span><span class="sxs-lookup"><span data-stu-id="6e55d-111">Relationship</span></span> | <span data-ttu-id="6e55d-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="6e55d-112">Type</span></span>   |<span data-ttu-id="6e55d-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="6e55d-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6e55d-114">fill</span><span class="sxs-lookup"><span data-stu-id="6e55d-114">fill</span></span>|[<span data-ttu-id="6e55d-115">workbookChartFill</span><span class="sxs-lookup"><span data-stu-id="6e55d-115">workbookChartFill</span></span>](workbookchartfill.md)|<span data-ttu-id="6e55d-p101">Representa o formato de preenchimento de uma série do gráfico, que inclui informações sobre a formatação da tela de fundo. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6e55d-p101">Represents the fill format of a chart series, which includes background formating information. Read-only.</span></span>|
|<span data-ttu-id="6e55d-118">line</span><span class="sxs-lookup"><span data-stu-id="6e55d-118">line</span></span>|[<span data-ttu-id="6e55d-119">workbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="6e55d-119">workbookChartLineFormat</span></span>](workbookchartlineformat.md)|<span data-ttu-id="6e55d-120">Representa a formatação de linha.</span><span class="sxs-lookup"><span data-stu-id="6e55d-120">Represents line formatting.</span></span> <span data-ttu-id="6e55d-121">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6e55d-121">Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="6e55d-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6e55d-122">JSON representation</span></span>

<span data-ttu-id="6e55d-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6e55d-123">Here is a JSON representation of the resource.</span></span>

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


