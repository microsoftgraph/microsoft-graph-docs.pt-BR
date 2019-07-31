---
title: tipo de recurso workbookChartDataLabelFormat
description: Encapsula as propriedades de formato dos rótulos de dados do gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: bd60187d5bc62675b53b4a0a254afa3632e9c1d6
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35963991"
---
# <a name="workbookchartdatalabelformat-resource-type"></a><span data-ttu-id="03eba-103">tipo de recurso workbookChartDataLabelFormat</span><span class="sxs-lookup"><span data-stu-id="03eba-103">workbookChartDataLabelFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="03eba-104">Encapsula as propriedades de formato dos rótulos de dados do gráfico.</span><span class="sxs-lookup"><span data-stu-id="03eba-104">Encapsulates the format properties for the chart data labels.</span></span>


## <a name="methods"></a><span data-ttu-id="03eba-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="03eba-105">Methods</span></span>
<span data-ttu-id="03eba-106">Nenhum</span><span class="sxs-lookup"><span data-stu-id="03eba-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="03eba-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="03eba-107">Properties</span></span>
<span data-ttu-id="03eba-108">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="03eba-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="03eba-109">Relações</span><span class="sxs-lookup"><span data-stu-id="03eba-109">Relationships</span></span>
| <span data-ttu-id="03eba-110">Relação</span><span class="sxs-lookup"><span data-stu-id="03eba-110">Relationship</span></span> | <span data-ttu-id="03eba-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="03eba-111">Type</span></span>   |<span data-ttu-id="03eba-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="03eba-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="03eba-113">fill</span><span class="sxs-lookup"><span data-stu-id="03eba-113">fill</span></span>|[<span data-ttu-id="03eba-114">workbookChartFill</span><span class="sxs-lookup"><span data-stu-id="03eba-114">workbookChartFill</span></span>](workbookchartfill.md)|<span data-ttu-id="03eba-p101">Representa o formato de preenchimento do rótulo de dados atual do gráfico. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="03eba-p101">Represents the fill format of the current chart data label. Read-only.</span></span>|
|<span data-ttu-id="03eba-117">font</span><span class="sxs-lookup"><span data-stu-id="03eba-117">font</span></span>|[<span data-ttu-id="03eba-118">workbookChartFont</span><span class="sxs-lookup"><span data-stu-id="03eba-118">workbookChartFont</span></span>](workbookchartfont.md)|<span data-ttu-id="03eba-119">Representa os atributos de fonte do rótulo de dados do gráfico, como nome, tamanho, cor, dentre outros.</span><span class="sxs-lookup"><span data-stu-id="03eba-119">Represents the font attributes (font name, font size, color, etc.) for a chart data label.</span></span> <span data-ttu-id="03eba-120">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="03eba-120">Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="03eba-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="03eba-121">JSON representation</span></span>

<span data-ttu-id="03eba-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="03eba-122">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "fill",
    "font"
    ],
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
<!--
{
  "type": "#page.annotation",
  "description": "ChartDataLabelFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
