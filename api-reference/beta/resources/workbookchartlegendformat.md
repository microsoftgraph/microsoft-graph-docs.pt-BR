---
title: tipo de recurso workbookChartLegendFormat
description: Encapsula as propriedades de formato de uma legenda de gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 32f9fcec2002039c9ccee399c90f1a26048c71cc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519299"
---
# <a name="workbookchartlegendformat-resource-type"></a><span data-ttu-id="c588e-103">tipo de recurso workbookChartLegendFormat</span><span class="sxs-lookup"><span data-stu-id="c588e-103">workbookChartLegendFormat resource type</span></span>

<span data-ttu-id="c588e-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="c588e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c588e-105">Encapsula as propriedades de formato de uma legenda de gráfico.</span><span class="sxs-lookup"><span data-stu-id="c588e-105">Encapsulates the format properties of a chart legend.</span></span>

## <a name="methods"></a><span data-ttu-id="c588e-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="c588e-106">Methods</span></span>
<span data-ttu-id="c588e-107">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c588e-107">None</span></span>

## <a name="properties"></a><span data-ttu-id="c588e-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c588e-108">Properties</span></span>
<span data-ttu-id="c588e-109">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="c588e-109">None</span></span>

## <a name="relationships"></a><span data-ttu-id="c588e-110">Relações</span><span class="sxs-lookup"><span data-stu-id="c588e-110">Relationships</span></span>
| <span data-ttu-id="c588e-111">Relação</span><span class="sxs-lookup"><span data-stu-id="c588e-111">Relationship</span></span> | <span data-ttu-id="c588e-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="c588e-112">Type</span></span>   |<span data-ttu-id="c588e-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="c588e-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c588e-114">fill</span><span class="sxs-lookup"><span data-stu-id="c588e-114">fill</span></span>|[<span data-ttu-id="c588e-115">workbookChartFill</span><span class="sxs-lookup"><span data-stu-id="c588e-115">workbookChartFill</span></span>](workbookchartfill.md)|<span data-ttu-id="c588e-p101">Representa o formato de preenchimento de um objeto, que inclui informações sobre a formatação da tela de fundo. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c588e-p101">Represents the fill format of an object, which includes background formating information. Read-only.</span></span>|
|<span data-ttu-id="c588e-118">fonte</span><span class="sxs-lookup"><span data-stu-id="c588e-118">font</span></span>|[<span data-ttu-id="c588e-119">workbookChartFont</span><span class="sxs-lookup"><span data-stu-id="c588e-119">workbookChartFont</span></span>](workbookchartfont.md)|<span data-ttu-id="c588e-120">Representa os atributos de fonte, como nome da fonte, tamanho da fonte, cor, etc. de uma legenda do gráfico.</span><span class="sxs-lookup"><span data-stu-id="c588e-120">Represents the font attributes such as font name, font size, color, etc. of a chart legend.</span></span> <span data-ttu-id="c588e-121">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c588e-121">Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="c588e-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c588e-122">JSON representation</span></span>

<span data-ttu-id="c588e-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c588e-123">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "fill",
    "font"
    ],
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
<!--
{
  "type": "#page.annotation",
  "description": "workbookChartLegendFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
