---
title: tipo de recurso workbookChartLegendFormat
description: Encapsula as propriedades de formato de uma legenda de gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 987753588beeec62ded346d2f2ff8611c0436e48
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007260"
---
# <a name="workbookchartlegendformat-resource-type"></a><span data-ttu-id="80c84-103">tipo de recurso workbookChartLegendFormat</span><span class="sxs-lookup"><span data-stu-id="80c84-103">workbookChartLegendFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="80c84-104">Encapsula as propriedades de formato de uma legenda de gráfico.</span><span class="sxs-lookup"><span data-stu-id="80c84-104">Encapsulates the format properties of a chart legend.</span></span>

## <a name="methods"></a><span data-ttu-id="80c84-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="80c84-105">Methods</span></span>
<span data-ttu-id="80c84-106">Nenhum</span><span class="sxs-lookup"><span data-stu-id="80c84-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="80c84-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="80c84-107">Properties</span></span>
<span data-ttu-id="80c84-108">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="80c84-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="80c84-109">Relações</span><span class="sxs-lookup"><span data-stu-id="80c84-109">Relationships</span></span>
| <span data-ttu-id="80c84-110">Relação</span><span class="sxs-lookup"><span data-stu-id="80c84-110">Relationship</span></span> | <span data-ttu-id="80c84-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="80c84-111">Type</span></span>   |<span data-ttu-id="80c84-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="80c84-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="80c84-113">fill</span><span class="sxs-lookup"><span data-stu-id="80c84-113">fill</span></span>|[<span data-ttu-id="80c84-114">workbookChartFill</span><span class="sxs-lookup"><span data-stu-id="80c84-114">workbookChartFill</span></span>](workbookchartfill.md)|<span data-ttu-id="80c84-p101">Representa o formato de preenchimento de um objeto, que inclui informações sobre a formatação da tela de fundo. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="80c84-p101">Represents the fill format of an object, which includes background formating information. Read-only.</span></span>|
|<span data-ttu-id="80c84-117">fonte</span><span class="sxs-lookup"><span data-stu-id="80c84-117">font</span></span>|[<span data-ttu-id="80c84-118">workbookChartFont</span><span class="sxs-lookup"><span data-stu-id="80c84-118">workbookChartFont</span></span>](workbookchartfont.md)|<span data-ttu-id="80c84-119">Representa os atributos de fonte, como nome da fonte, tamanho da fonte, cor, etc. de uma legenda do gráfico.</span><span class="sxs-lookup"><span data-stu-id="80c84-119">Represents the font attributes such as font name, font size, color, etc. of a chart legend.</span></span> <span data-ttu-id="80c84-120">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="80c84-120">Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="80c84-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="80c84-121">JSON representation</span></span>

<span data-ttu-id="80c84-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="80c84-122">Here is a JSON representation of the resource.</span></span>

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
