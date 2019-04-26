---
title: Tipo de recurso ChartDataLabelFormat
description: Encapsula as propriedades de formato dos rótulos de dados do gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 645267fd595a4b8e83090d9d6b2179e8c6112a78
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32569071"
---
# <a name="chartdatalabelformat-resource-type"></a><span data-ttu-id="0c602-103">Tipo de recurso ChartDataLabelFormat</span><span class="sxs-lookup"><span data-stu-id="0c602-103">ChartDataLabelFormat resource type</span></span>

<span data-ttu-id="0c602-104">Encapsula as propriedades de formato dos rótulos de dados do gráfico.</span><span class="sxs-lookup"><span data-stu-id="0c602-104">Encapsulates the format properties for the chart data labels.</span></span>


## <a name="methods"></a><span data-ttu-id="0c602-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="0c602-105">Methods</span></span>
<span data-ttu-id="0c602-106">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0c602-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="0c602-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0c602-107">Properties</span></span>
<span data-ttu-id="0c602-108">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="0c602-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="0c602-109">Relações</span><span class="sxs-lookup"><span data-stu-id="0c602-109">Relationships</span></span>
| <span data-ttu-id="0c602-110">Relação</span><span class="sxs-lookup"><span data-stu-id="0c602-110">Relationship</span></span> | <span data-ttu-id="0c602-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="0c602-111">Type</span></span>   |<span data-ttu-id="0c602-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="0c602-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0c602-113">fill</span><span class="sxs-lookup"><span data-stu-id="0c602-113">fill</span></span>|[<span data-ttu-id="0c602-114">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="0c602-114">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="0c602-p101">Representa o formato de preenchimento do rótulo de dados atual do gráfico. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0c602-p101">Represents the fill format of the current chart data label. Read-only.</span></span>|
|<span data-ttu-id="0c602-117">font</span><span class="sxs-lookup"><span data-stu-id="0c602-117">font</span></span>|[<span data-ttu-id="0c602-118">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="0c602-118">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="0c602-119">Representa os atributos de fonte do rótulo de dados do gráfico, como nome, tamanho, cor, dentre outros.</span><span class="sxs-lookup"><span data-stu-id="0c602-119">Represents the font attributes (font name, font size, color, etc.) for a chart data label.</span></span> <span data-ttu-id="0c602-120">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0c602-120">Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="0c602-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0c602-121">JSON representation</span></span>

<span data-ttu-id="0c602-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0c602-122">Here is a JSON representation of the resource.</span></span>

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
