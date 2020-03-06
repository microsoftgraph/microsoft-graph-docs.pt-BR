---
title: Tipo de recurso ChartSeriesFormat
description: Abrange as propriedades de formatação da série do gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: a44392eb718c157f6422228405f7bb2a4b411733
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533097"
---
# <a name="chartseriesformat-resource-type"></a><span data-ttu-id="161cb-103">Tipo de recurso ChartSeriesFormat</span><span class="sxs-lookup"><span data-stu-id="161cb-103">ChartSeriesFormat resource type</span></span>

<span data-ttu-id="161cb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="161cb-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="161cb-105">Abrange as propriedades de formatação da série do gráfico.</span><span class="sxs-lookup"><span data-stu-id="161cb-105">encapsulates the format properties for the chart series</span></span>


## <a name="methods"></a><span data-ttu-id="161cb-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="161cb-106">Methods</span></span>
<span data-ttu-id="161cb-107">Nenhum</span><span class="sxs-lookup"><span data-stu-id="161cb-107">None</span></span>

## <a name="properties"></a><span data-ttu-id="161cb-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="161cb-108">Properties</span></span>
<span data-ttu-id="161cb-109">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="161cb-109">None</span></span>

## <a name="relationships"></a><span data-ttu-id="161cb-110">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="161cb-110">Relationships</span></span>
| <span data-ttu-id="161cb-111">Relação</span><span class="sxs-lookup"><span data-stu-id="161cb-111">Relationship</span></span> | <span data-ttu-id="161cb-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="161cb-112">Type</span></span>   |<span data-ttu-id="161cb-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="161cb-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="161cb-114">fill</span><span class="sxs-lookup"><span data-stu-id="161cb-114">fill</span></span>|[<span data-ttu-id="161cb-115">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="161cb-115">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="161cb-p101">Representa o formato de preenchimento de uma série do gráfico, que inclui informações sobre a formatação da tela de fundo. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="161cb-p101">Represents the fill format of a chart series, which includes background formating information. Read-only.</span></span>|
|<span data-ttu-id="161cb-118">line</span><span class="sxs-lookup"><span data-stu-id="161cb-118">line</span></span>|[<span data-ttu-id="161cb-119">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="161cb-119">WorkbookChartLineFormat</span></span>](chartlineformat.md)|<span data-ttu-id="161cb-120">Representa a formatação de linha.</span><span class="sxs-lookup"><span data-stu-id="161cb-120">Represents line formatting.</span></span> <span data-ttu-id="161cb-121">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="161cb-121">Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="161cb-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="161cb-122">JSON representation</span></span>

<span data-ttu-id="161cb-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="161cb-123">Here is a JSON representation of the resource.</span></span>

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
