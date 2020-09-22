---
title: Tipo de recurso ChartAxisFormat
description: Encapsula as propriedades de formato do eixo do gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 18021b2776ccd749538ba5a94e7af9b1518a9bb6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47988440"
---
# <a name="chartaxisformat-resource-type"></a><span data-ttu-id="397ae-103">Tipo de recurso ChartAxisFormat</span><span class="sxs-lookup"><span data-stu-id="397ae-103">ChartAxisFormat resource type</span></span>

<span data-ttu-id="397ae-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="397ae-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="397ae-105">Encapsula as propriedades de formato do eixo do gráfico.</span><span class="sxs-lookup"><span data-stu-id="397ae-105">Encapsulates the format properties for the chart axis.</span></span>


## <a name="methods"></a><span data-ttu-id="397ae-106">Methods</span><span class="sxs-lookup"><span data-stu-id="397ae-106">Methods</span></span>
<span data-ttu-id="397ae-107">Nenhum</span><span class="sxs-lookup"><span data-stu-id="397ae-107">None</span></span>
## <a name="properties"></a><span data-ttu-id="397ae-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="397ae-108">Properties</span></span>
<span data-ttu-id="397ae-109">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="397ae-109">None</span></span>

## <a name="relationships"></a><span data-ttu-id="397ae-110">Relações</span><span class="sxs-lookup"><span data-stu-id="397ae-110">Relationships</span></span>
| <span data-ttu-id="397ae-111">Relação</span><span class="sxs-lookup"><span data-stu-id="397ae-111">Relationship</span></span> | <span data-ttu-id="397ae-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="397ae-112">Type</span></span>   |<span data-ttu-id="397ae-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="397ae-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="397ae-114">font</span><span class="sxs-lookup"><span data-stu-id="397ae-114">font</span></span>|[<span data-ttu-id="397ae-115">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="397ae-115">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="397ae-p101">Representa os atributos de fonte de um elemento do eixo do gráfico, como nome, tamanho, cor, etc. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="397ae-p101">Represents the font attributes (font name, font size, color, etc.) for a chart axis element. Read-only.</span></span>|
|<span data-ttu-id="397ae-118">line</span><span class="sxs-lookup"><span data-stu-id="397ae-118">line</span></span>|[<span data-ttu-id="397ae-119">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="397ae-119">WorkbookChartLineFormat</span></span>](chartlineformat.md)|<span data-ttu-id="397ae-120">Representa a formatação de linha do gráfico.</span><span class="sxs-lookup"><span data-stu-id="397ae-120">Represents chart line formatting.</span></span> <span data-ttu-id="397ae-121">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="397ae-121">Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="397ae-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="397ae-122">JSON representation</span></span>

<span data-ttu-id="397ae-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="397ae-123">Here is a JSON representation of the resource.</span></span>

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

