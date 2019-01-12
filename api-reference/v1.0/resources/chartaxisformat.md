---
title: Tipo de recurso ChartAxisFormat
description: Abrange as propriedades de formatação do eixo do gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 92258887c9646890ee63d14aebcd32ada7a8aaa6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27952108"
---
# <a name="chartaxisformat-resource-type"></a><span data-ttu-id="b9da6-103">Tipo de recurso ChartAxisFormat</span><span class="sxs-lookup"><span data-stu-id="b9da6-103">ChartAxisFormat resource type</span></span>

<span data-ttu-id="b9da6-104">Abrange as propriedades de formatação do eixo do gráfico.</span><span class="sxs-lookup"><span data-stu-id="b9da6-104">Encapsulates the format properties for the chart axis.</span></span>


## <a name="methods"></a><span data-ttu-id="b9da6-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="b9da6-105">Methods</span></span>
<span data-ttu-id="b9da6-106">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b9da6-106">None</span></span>
## <a name="properties"></a><span data-ttu-id="b9da6-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b9da6-107">Properties</span></span>
<span data-ttu-id="b9da6-108">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b9da6-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="b9da6-109">Relações</span><span class="sxs-lookup"><span data-stu-id="b9da6-109">Relationships</span></span>
| <span data-ttu-id="b9da6-110">Relação</span><span class="sxs-lookup"><span data-stu-id="b9da6-110">Relationship</span></span> | <span data-ttu-id="b9da6-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="b9da6-111">Type</span></span>   |<span data-ttu-id="b9da6-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="b9da6-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b9da6-113">font</span><span class="sxs-lookup"><span data-stu-id="b9da6-113">font</span></span>|[<span data-ttu-id="b9da6-114">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="b9da6-114">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="b9da6-p101">Representa os atributos de fonte de um elemento do eixo do gráfico, como nome, tamanho, cor, etc. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b9da6-p101">Represents the font attributes (font name, font size, color, etc.) for a chart axis element. Read-only.</span></span>|
|<span data-ttu-id="b9da6-117">line</span><span class="sxs-lookup"><span data-stu-id="b9da6-117">line</span></span>|[<span data-ttu-id="b9da6-118">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="b9da6-118">WorkbookChartLineFormat</span></span>](chartlineformat.md)|<span data-ttu-id="b9da6-p102">Representa a formatação de linha do gráfico. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b9da6-p102">Represents chart line formatting. Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="b9da6-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b9da6-121">JSON representation</span></span>

<span data-ttu-id="b9da6-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b9da6-122">Here is a JSON representation of the resource.</span></span>

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
