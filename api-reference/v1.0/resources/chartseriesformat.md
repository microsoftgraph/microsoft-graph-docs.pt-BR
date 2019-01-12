---
title: Tipo de recurso ChartSeriesFormat
description: Abrange as propriedades de formatação da série do gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: fd342e55524d51b6a0382df8ca9310ea162308d2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27961432"
---
# <a name="chartseriesformat-resource-type"></a><span data-ttu-id="56763-103">Tipo de recurso ChartSeriesFormat</span><span class="sxs-lookup"><span data-stu-id="56763-103">ChartSeriesFormat resource type</span></span>

<span data-ttu-id="56763-104">Abrange as propriedades de formatação da série do gráfico.</span><span class="sxs-lookup"><span data-stu-id="56763-104">encapsulates the format properties for the chart series</span></span>


## <a name="methods"></a><span data-ttu-id="56763-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="56763-105">Methods</span></span>
<span data-ttu-id="56763-106">Nenhum</span><span class="sxs-lookup"><span data-stu-id="56763-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="56763-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="56763-107">Properties</span></span>
<span data-ttu-id="56763-108">Nenhum</span><span class="sxs-lookup"><span data-stu-id="56763-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="56763-109">Relações</span><span class="sxs-lookup"><span data-stu-id="56763-109">Relationships</span></span>
| <span data-ttu-id="56763-110">Relação</span><span class="sxs-lookup"><span data-stu-id="56763-110">Relationship</span></span> | <span data-ttu-id="56763-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="56763-111">Type</span></span>   |<span data-ttu-id="56763-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="56763-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="56763-113">fill</span><span class="sxs-lookup"><span data-stu-id="56763-113">fill</span></span>|[<span data-ttu-id="56763-114">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="56763-114">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="56763-p101">Representa o formato de preenchimento de uma série do gráfico, que inclui informações sobre a formatação da tela de fundo. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="56763-p101">Represents the fill format of a chart series, which includes background formating information. Read-only.</span></span>|
|<span data-ttu-id="56763-117">line</span><span class="sxs-lookup"><span data-stu-id="56763-117">line</span></span>|[<span data-ttu-id="56763-118">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="56763-118">WorkbookChartLineFormat</span></span>](chartlineformat.md)|<span data-ttu-id="56763-p102">Representa a formatação de linha. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="56763-p102">Represents line formatting. Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="56763-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="56763-121">JSON representation</span></span>

<span data-ttu-id="56763-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="56763-122">Here is a JSON representation of the resource.</span></span>

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
