---
title: Tipo de recurso ChartLegendFormat
description: Encapsula as propriedades de formato de uma legenda de gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: d3d7d9a0a74a56a6e0ae99aa7431779dc7164265
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531843"
---
# <a name="chartlegendformat-resource-type"></a><span data-ttu-id="c144a-103">Tipo de recurso ChartLegendFormat</span><span class="sxs-lookup"><span data-stu-id="c144a-103">ChartLegendFormat resource type</span></span>

<span data-ttu-id="c144a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c144a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c144a-105">Encapsula as propriedades de formato de uma legenda de gráfico.</span><span class="sxs-lookup"><span data-stu-id="c144a-105">Encapsulates the format properties of a chart legend.</span></span>


## <a name="methods"></a><span data-ttu-id="c144a-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="c144a-106">Methods</span></span>
<span data-ttu-id="c144a-107">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c144a-107">None</span></span>

## <a name="properties"></a><span data-ttu-id="c144a-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c144a-108">Properties</span></span>
<span data-ttu-id="c144a-109">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="c144a-109">None</span></span>

## <a name="relationships"></a><span data-ttu-id="c144a-110">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="c144a-110">Relationships</span></span>
| <span data-ttu-id="c144a-111">Relação</span><span class="sxs-lookup"><span data-stu-id="c144a-111">Relationship</span></span> | <span data-ttu-id="c144a-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="c144a-112">Type</span></span>   |<span data-ttu-id="c144a-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="c144a-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c144a-114">fill</span><span class="sxs-lookup"><span data-stu-id="c144a-114">fill</span></span>|[<span data-ttu-id="c144a-115">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="c144a-115">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="c144a-p101">Representa o formato de preenchimento de um objeto, que inclui informações sobre a formatação da tela de fundo. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c144a-p101">Represents the fill format of an object, which includes background formating information. Read-only.</span></span>|
|<span data-ttu-id="c144a-118">fonte</span><span class="sxs-lookup"><span data-stu-id="c144a-118">font</span></span>|[<span data-ttu-id="c144a-119">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="c144a-119">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="c144a-120">Representa os atributos de fonte, como nome da fonte, tamanho da fonte, cor, etc. de uma legenda do gráfico.</span><span class="sxs-lookup"><span data-stu-id="c144a-120">Represents the font attributes such as font name, font size, color, etc. of a chart legend.</span></span> <span data-ttu-id="c144a-121">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c144a-121">Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="c144a-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c144a-122">JSON representation</span></span>

<span data-ttu-id="c144a-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c144a-123">Here is a JSON representation of the resource.</span></span>

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
