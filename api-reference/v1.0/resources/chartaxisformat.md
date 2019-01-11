---
title: Tipo de recurso ChartAxisFormat
description: Abrange as propriedades de formatação do eixo do gráfico.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: a219122141da1f384279d0ff4c612f62226612c9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27821263"
---
# <a name="chartaxisformat-resource-type"></a><span data-ttu-id="966c4-103">Tipo de recurso ChartAxisFormat</span><span class="sxs-lookup"><span data-stu-id="966c4-103">ChartAxisFormat resource type</span></span>

<span data-ttu-id="966c4-104">Abrange as propriedades de formatação do eixo do gráfico.</span><span class="sxs-lookup"><span data-stu-id="966c4-104">Encapsulates the format properties for the chart axis.</span></span>


## <a name="methods"></a><span data-ttu-id="966c4-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="966c4-105">Methods</span></span>
<span data-ttu-id="966c4-106">Nenhum</span><span class="sxs-lookup"><span data-stu-id="966c4-106">None</span></span>
## <a name="properties"></a><span data-ttu-id="966c4-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="966c4-107">Properties</span></span>
<span data-ttu-id="966c4-108">Nenhum</span><span class="sxs-lookup"><span data-stu-id="966c4-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="966c4-109">Relações</span><span class="sxs-lookup"><span data-stu-id="966c4-109">Relationships</span></span>
| <span data-ttu-id="966c4-110">Relação</span><span class="sxs-lookup"><span data-stu-id="966c4-110">Relationship</span></span> | <span data-ttu-id="966c4-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="966c4-111">Type</span></span>   |<span data-ttu-id="966c4-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="966c4-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="966c4-113">font</span><span class="sxs-lookup"><span data-stu-id="966c4-113">font</span></span>|[<span data-ttu-id="966c4-114">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="966c4-114">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="966c4-p101">Representa os atributos de fonte de um elemento do eixo do gráfico, como nome, tamanho, cor, etc. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="966c4-p101">Represents the font attributes (font name, font size, color, etc.) for a chart axis element. Read-only.</span></span>|
|<span data-ttu-id="966c4-117">line</span><span class="sxs-lookup"><span data-stu-id="966c4-117">line</span></span>|[<span data-ttu-id="966c4-118">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="966c4-118">WorkbookChartLineFormat</span></span>](chartlineformat.md)|<span data-ttu-id="966c4-p102">Representa a formatação de linha do gráfico. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="966c4-p102">Represents chart line formatting. Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="966c4-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="966c4-121">JSON representation</span></span>

<span data-ttu-id="966c4-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="966c4-122">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "ChartAxisFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
