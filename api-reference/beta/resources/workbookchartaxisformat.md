---
title: tipo de recurso workbookChartAxisFormat
description: Encapsula as propriedades de formato do eixo do gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 8c152971dde5efb188cfde30c30b54a1266b44fb
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348464"
---
# <a name="workbookchartaxisformat-resource-type"></a><span data-ttu-id="cdc61-103">tipo de recurso workbookChartAxisFormat</span><span class="sxs-lookup"><span data-stu-id="cdc61-103">workbookChartAxisFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cdc61-104">Encapsula as propriedades de formato do eixo do gráfico.</span><span class="sxs-lookup"><span data-stu-id="cdc61-104">Encapsulates the format properties for the chart axis.</span></span>


## <a name="methods"></a><span data-ttu-id="cdc61-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="cdc61-105">Methods</span></span>
<span data-ttu-id="cdc61-106">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cdc61-106">None</span></span>
## <a name="properties"></a><span data-ttu-id="cdc61-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cdc61-107">Properties</span></span>
<span data-ttu-id="cdc61-108">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="cdc61-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="cdc61-109">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="cdc61-109">Relationships</span></span>
| <span data-ttu-id="cdc61-110">Relação</span><span class="sxs-lookup"><span data-stu-id="cdc61-110">Relationship</span></span> | <span data-ttu-id="cdc61-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="cdc61-111">Type</span></span>   |<span data-ttu-id="cdc61-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="cdc61-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cdc61-113">font</span><span class="sxs-lookup"><span data-stu-id="cdc61-113">font</span></span>|[<span data-ttu-id="cdc61-114">workbookChartFont</span><span class="sxs-lookup"><span data-stu-id="cdc61-114">workbookChartFont</span></span>](workbookchartfont.md)|<span data-ttu-id="cdc61-p101">Representa os atributos de fonte de um elemento do eixo do gráfico, como nome, tamanho, cor, etc. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cdc61-p101">Represents the font attributes (font name, font size, color, etc.) for a chart axis element. Read-only.</span></span>|
|<span data-ttu-id="cdc61-117">line</span><span class="sxs-lookup"><span data-stu-id="cdc61-117">line</span></span>|[<span data-ttu-id="cdc61-118">workbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="cdc61-118">workbookChartLineFormat</span></span>](workbookchartlineformat.md)|<span data-ttu-id="cdc61-119">Representa a formatação de linha do gráfico.</span><span class="sxs-lookup"><span data-stu-id="cdc61-119">Represents chart line formatting.</span></span> <span data-ttu-id="cdc61-120">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cdc61-120">Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="cdc61-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cdc61-121">JSON representation</span></span>

<span data-ttu-id="cdc61-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cdc61-122">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartAxisFormat"
}-->

```json
{
  "font": {"@odata.type": "microsoft.graph.workbookChartFont"},
  "line": {"@odata.type": "microsoft.graph.workbookChartLineFormat"}
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ChartAxisFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
