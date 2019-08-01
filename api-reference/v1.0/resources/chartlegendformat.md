---
title: Tipo de recurso ChartLegendFormat
description: Encapsula as propriedades de formato de uma legenda de gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 2148b6b5baf8bb680f85954d000da097bcf8f0b9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032952"
---
# <a name="chartlegendformat-resource-type"></a><span data-ttu-id="ce24a-103">Tipo de recurso ChartLegendFormat</span><span class="sxs-lookup"><span data-stu-id="ce24a-103">ChartLegendFormat resource type</span></span>

<span data-ttu-id="ce24a-104">Encapsula as propriedades de formato de uma legenda de gráfico.</span><span class="sxs-lookup"><span data-stu-id="ce24a-104">Encapsulates the format properties of a chart legend.</span></span>


## <a name="methods"></a><span data-ttu-id="ce24a-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="ce24a-105">Methods</span></span>
<span data-ttu-id="ce24a-106">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ce24a-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="ce24a-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ce24a-107">Properties</span></span>
<span data-ttu-id="ce24a-108">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="ce24a-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="ce24a-109">Relações</span><span class="sxs-lookup"><span data-stu-id="ce24a-109">Relationships</span></span>
| <span data-ttu-id="ce24a-110">Relação</span><span class="sxs-lookup"><span data-stu-id="ce24a-110">Relationship</span></span> | <span data-ttu-id="ce24a-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="ce24a-111">Type</span></span>   |<span data-ttu-id="ce24a-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="ce24a-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ce24a-113">fill</span><span class="sxs-lookup"><span data-stu-id="ce24a-113">fill</span></span>|[<span data-ttu-id="ce24a-114">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="ce24a-114">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="ce24a-p101">Representa o formato de preenchimento de um objeto, que inclui informações sobre a formatação da tela de fundo. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ce24a-p101">Represents the fill format of an object, which includes background formating information. Read-only.</span></span>|
|<span data-ttu-id="ce24a-117">fonte</span><span class="sxs-lookup"><span data-stu-id="ce24a-117">font</span></span>|[<span data-ttu-id="ce24a-118">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="ce24a-118">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="ce24a-119">Representa os atributos de fonte, como nome da fonte, tamanho da fonte, cor, etc. de uma legenda do gráfico.</span><span class="sxs-lookup"><span data-stu-id="ce24a-119">Represents the font attributes such as font name, font size, color, etc. of a chart legend.</span></span> <span data-ttu-id="ce24a-120">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ce24a-120">Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="ce24a-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ce24a-121">JSON representation</span></span>

<span data-ttu-id="ce24a-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ce24a-122">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartLegendFormat"
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
  "description": "ChartLegendFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
