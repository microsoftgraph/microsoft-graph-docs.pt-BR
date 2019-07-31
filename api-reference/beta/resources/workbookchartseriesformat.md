---
title: tipo de recurso workbookChartSeriesFormat
description: Abrange as propriedades de formatação da série do gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 739a874545047c2ed6927cb4e31d2e006f4e6ba4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007162"
---
# <a name="workbookchartseriesformat-resource-type"></a><span data-ttu-id="d5852-103">tipo de recurso workbookChartSeriesFormat</span><span class="sxs-lookup"><span data-stu-id="d5852-103">workbookChartSeriesFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d5852-104">Encapsula as propriedades de formato da série do gráfico.</span><span class="sxs-lookup"><span data-stu-id="d5852-104">Encapsulates the format properties for the chart series.</span></span>


## <a name="methods"></a><span data-ttu-id="d5852-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="d5852-105">Methods</span></span>
<span data-ttu-id="d5852-106">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d5852-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="d5852-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d5852-107">Properties</span></span>
<span data-ttu-id="d5852-108">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="d5852-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="d5852-109">Relações</span><span class="sxs-lookup"><span data-stu-id="d5852-109">Relationships</span></span>
| <span data-ttu-id="d5852-110">Relação</span><span class="sxs-lookup"><span data-stu-id="d5852-110">Relationship</span></span> | <span data-ttu-id="d5852-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="d5852-111">Type</span></span>   |<span data-ttu-id="d5852-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5852-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d5852-113">fill</span><span class="sxs-lookup"><span data-stu-id="d5852-113">fill</span></span>|[<span data-ttu-id="d5852-114">workbookChartFill</span><span class="sxs-lookup"><span data-stu-id="d5852-114">workbookChartFill</span></span>](workbookchartfill.md)|<span data-ttu-id="d5852-p101">Representa o formato de preenchimento de uma série do gráfico, que inclui informações sobre a formatação da tela de fundo. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d5852-p101">Represents the fill format of a chart series, which includes background formating information. Read-only.</span></span>|
|<span data-ttu-id="d5852-117">line</span><span class="sxs-lookup"><span data-stu-id="d5852-117">line</span></span>|[<span data-ttu-id="d5852-118">workbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="d5852-118">workbookChartLineFormat</span></span>](workbookchartlineformat.md)|<span data-ttu-id="d5852-119">Representa a formatação de linha.</span><span class="sxs-lookup"><span data-stu-id="d5852-119">Represents line formatting.</span></span> <span data-ttu-id="d5852-120">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d5852-120">Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="d5852-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d5852-121">JSON representation</span></span>

<span data-ttu-id="d5852-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d5852-122">Here is a JSON representation of the resource.</span></span>

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
