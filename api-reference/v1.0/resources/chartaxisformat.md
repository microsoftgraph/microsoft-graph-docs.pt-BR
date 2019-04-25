---
title: Tipo de recurso ChartAxisFormat
description: Encapsula as propriedades de formato do eixo do gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 92258887c9646890ee63d14aebcd32ada7a8aaa6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32569246"
---
# <a name="chartaxisformat-resource-type"></a><span data-ttu-id="e91ff-103">Tipo de recurso ChartAxisFormat</span><span class="sxs-lookup"><span data-stu-id="e91ff-103">ChartAxisFormat resource type</span></span>

<span data-ttu-id="e91ff-104">Encapsula as propriedades de formato do eixo do gráfico.</span><span class="sxs-lookup"><span data-stu-id="e91ff-104">Encapsulates the format properties for the chart axis.</span></span>


## <a name="methods"></a><span data-ttu-id="e91ff-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="e91ff-105">Methods</span></span>
<span data-ttu-id="e91ff-106">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e91ff-106">None</span></span>
## <a name="properties"></a><span data-ttu-id="e91ff-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e91ff-107">Properties</span></span>
<span data-ttu-id="e91ff-108">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="e91ff-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="e91ff-109">Relações</span><span class="sxs-lookup"><span data-stu-id="e91ff-109">Relationships</span></span>
| <span data-ttu-id="e91ff-110">Relação</span><span class="sxs-lookup"><span data-stu-id="e91ff-110">Relationship</span></span> | <span data-ttu-id="e91ff-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="e91ff-111">Type</span></span>   |<span data-ttu-id="e91ff-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="e91ff-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e91ff-113">font</span><span class="sxs-lookup"><span data-stu-id="e91ff-113">font</span></span>|[<span data-ttu-id="e91ff-114">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="e91ff-114">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="e91ff-p101">Representa os atributos de fonte de um elemento do eixo do gráfico, como nome, tamanho, cor, etc. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e91ff-p101">Represents the font attributes (font name, font size, color, etc.) for a chart axis element. Read-only.</span></span>|
|<span data-ttu-id="e91ff-117">line</span><span class="sxs-lookup"><span data-stu-id="e91ff-117">line</span></span>|[<span data-ttu-id="e91ff-118">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="e91ff-118">WorkbookChartLineFormat</span></span>](chartlineformat.md)|<span data-ttu-id="e91ff-119">Representa a formatação de linha do gráfico.</span><span class="sxs-lookup"><span data-stu-id="e91ff-119">Represents chart line formatting.</span></span> <span data-ttu-id="e91ff-120">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e91ff-120">Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="e91ff-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e91ff-121">JSON representation</span></span>

<span data-ttu-id="e91ff-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e91ff-122">Here is a JSON representation of the resource.</span></span>

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
