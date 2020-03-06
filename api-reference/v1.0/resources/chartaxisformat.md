---
title: Tipo de recurso ChartAxisFormat
description: Encapsula as propriedades de formato do eixo do gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: d08f9fea825cb9d7a3f0bee735204cbf797e968d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531905"
---
# <a name="chartaxisformat-resource-type"></a><span data-ttu-id="058f9-103">Tipo de recurso ChartAxisFormat</span><span class="sxs-lookup"><span data-stu-id="058f9-103">ChartAxisFormat resource type</span></span>

<span data-ttu-id="058f9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="058f9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="058f9-105">Encapsula as propriedades de formato do eixo do gráfico.</span><span class="sxs-lookup"><span data-stu-id="058f9-105">Encapsulates the format properties for the chart axis.</span></span>


## <a name="methods"></a><span data-ttu-id="058f9-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="058f9-106">Methods</span></span>
<span data-ttu-id="058f9-107">Nenhum</span><span class="sxs-lookup"><span data-stu-id="058f9-107">None</span></span>
## <a name="properties"></a><span data-ttu-id="058f9-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="058f9-108">Properties</span></span>
<span data-ttu-id="058f9-109">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="058f9-109">None</span></span>

## <a name="relationships"></a><span data-ttu-id="058f9-110">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="058f9-110">Relationships</span></span>
| <span data-ttu-id="058f9-111">Relação</span><span class="sxs-lookup"><span data-stu-id="058f9-111">Relationship</span></span> | <span data-ttu-id="058f9-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="058f9-112">Type</span></span>   |<span data-ttu-id="058f9-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="058f9-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="058f9-114">font</span><span class="sxs-lookup"><span data-stu-id="058f9-114">font</span></span>|[<span data-ttu-id="058f9-115">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="058f9-115">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="058f9-p101">Representa os atributos de fonte de um elemento do eixo do gráfico, como nome, tamanho, cor, etc. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="058f9-p101">Represents the font attributes (font name, font size, color, etc.) for a chart axis element. Read-only.</span></span>|
|<span data-ttu-id="058f9-118">line</span><span class="sxs-lookup"><span data-stu-id="058f9-118">line</span></span>|[<span data-ttu-id="058f9-119">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="058f9-119">WorkbookChartLineFormat</span></span>](chartlineformat.md)|<span data-ttu-id="058f9-120">Representa a formatação de linha do gráfico.</span><span class="sxs-lookup"><span data-stu-id="058f9-120">Represents chart line formatting.</span></span> <span data-ttu-id="058f9-121">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="058f9-121">Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="058f9-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="058f9-122">JSON representation</span></span>

<span data-ttu-id="058f9-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="058f9-123">Here is a JSON representation of the resource.</span></span>

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
