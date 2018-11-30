---
title: Tipo de recurso ChartSeriesFormat
description: Abrange as propriedades de formatação da série do gráfico.
ms.openlocfilehash: 81b79331580c2d7edbc52f19d1c4c9cfd57db0cf
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27004824"
---
# <a name="chartseriesformat-resource-type"></a><span data-ttu-id="17923-103">Tipo de recurso ChartSeriesFormat</span><span class="sxs-lookup"><span data-stu-id="17923-103">ChartSeriesFormat resource type</span></span>

<span data-ttu-id="17923-104">Abrange as propriedades de formatação da série do gráfico.</span><span class="sxs-lookup"><span data-stu-id="17923-104">encapsulates the format properties for the chart series</span></span>


## <a name="methods"></a><span data-ttu-id="17923-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="17923-105">Methods</span></span>
<span data-ttu-id="17923-106">Nenhum</span><span class="sxs-lookup"><span data-stu-id="17923-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="17923-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="17923-107">Properties</span></span>
<span data-ttu-id="17923-108">Nenhum</span><span class="sxs-lookup"><span data-stu-id="17923-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="17923-109">Relações</span><span class="sxs-lookup"><span data-stu-id="17923-109">Relationships</span></span>
| <span data-ttu-id="17923-110">Relação</span><span class="sxs-lookup"><span data-stu-id="17923-110">Relationship</span></span> | <span data-ttu-id="17923-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="17923-111">Type</span></span>   |<span data-ttu-id="17923-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="17923-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="17923-113">fill</span><span class="sxs-lookup"><span data-stu-id="17923-113">fill</span></span>|[<span data-ttu-id="17923-114">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="17923-114">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="17923-p101">Representa o formato de preenchimento de uma série do gráfico, que inclui informações sobre a formatação da tela de fundo. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="17923-p101">Represents the fill format of a chart series, which includes background formating information. Read-only.</span></span>|
|<span data-ttu-id="17923-117">line</span><span class="sxs-lookup"><span data-stu-id="17923-117">line</span></span>|[<span data-ttu-id="17923-118">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="17923-118">WorkbookChartLineFormat</span></span>](chartlineformat.md)|<span data-ttu-id="17923-p102">Representa a formatação de linha. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="17923-p102">Represents line formatting. Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="17923-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="17923-121">JSON representation</span></span>

<span data-ttu-id="17923-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="17923-122">Here is a JSON representation of the resource.</span></span>

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