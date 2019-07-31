---
title: tipo de recurso workbookChartPointFormat
description: Representa um objeto de formatação para os pontos do gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 9c3d968c4d36b8220d505edb6b7503a2b1206416
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007232"
---
# <a name="workbookchartpointformat-resource-type"></a><span data-ttu-id="c36d8-103">tipo de recurso workbookChartPointFormat</span><span class="sxs-lookup"><span data-stu-id="c36d8-103">workbookChartPointFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c36d8-104">Representa um objeto de formatação para os pontos do gráfico.</span><span class="sxs-lookup"><span data-stu-id="c36d8-104">Represents formatting object for chart points.</span></span>


## <a name="methods"></a><span data-ttu-id="c36d8-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="c36d8-105">Methods</span></span>
<span data-ttu-id="c36d8-106">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c36d8-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="c36d8-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c36d8-107">Properties</span></span>
<span data-ttu-id="c36d8-108">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="c36d8-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="c36d8-109">Relações</span><span class="sxs-lookup"><span data-stu-id="c36d8-109">Relationships</span></span>
| <span data-ttu-id="c36d8-110">Relação</span><span class="sxs-lookup"><span data-stu-id="c36d8-110">Relationship</span></span> | <span data-ttu-id="c36d8-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="c36d8-111">Type</span></span>   |<span data-ttu-id="c36d8-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="c36d8-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c36d8-113">fill</span><span class="sxs-lookup"><span data-stu-id="c36d8-113">fill</span></span>|[<span data-ttu-id="c36d8-114">workbookChartFill</span><span class="sxs-lookup"><span data-stu-id="c36d8-114">workbookChartFill</span></span>](workbookchartfill.md)|<span data-ttu-id="c36d8-115">Representa o formato de preenchimento de um gráfico, que inclui informações sobre a formatação da tela de fundo.</span><span class="sxs-lookup"><span data-stu-id="c36d8-115">Represents the fill format of a chart, which includes background formating information.</span></span> <span data-ttu-id="c36d8-116">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c36d8-116">Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="c36d8-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c36d8-117">JSON representation</span></span>

<span data-ttu-id="c36d8-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c36d8-118">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "fill"
    ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartPointFormat"
}-->

```json
{
  "fill": {"@odata.type": "microsoft.graph.workbookChartFill"}
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ChartPointFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
