---
title: Tipo de recurso ChartTitleFormat
description: Abrange as propriedades de formatação do título do gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 632b3a165a5f2f3a4216868bf440099610cdc800
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48059212"
---
# <a name="charttitleformat-resource-type"></a><span data-ttu-id="c7fc5-103">Tipo de recurso ChartTitleFormat</span><span class="sxs-lookup"><span data-stu-id="c7fc5-103">ChartTitleFormat resource type</span></span>

<span data-ttu-id="c7fc5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c7fc5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c7fc5-105">Abrange as propriedades de formatação do título do gráfico.</span><span class="sxs-lookup"><span data-stu-id="c7fc5-105">Encapsulates the format properties for the chart title.</span></span>


## <a name="methods"></a><span data-ttu-id="c7fc5-106">Methods</span><span class="sxs-lookup"><span data-stu-id="c7fc5-106">Methods</span></span>
<span data-ttu-id="c7fc5-107">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c7fc5-107">None</span></span>

## <a name="properties"></a><span data-ttu-id="c7fc5-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c7fc5-108">Properties</span></span>
<span data-ttu-id="c7fc5-109">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="c7fc5-109">None</span></span>

## <a name="relationships"></a><span data-ttu-id="c7fc5-110">Relações</span><span class="sxs-lookup"><span data-stu-id="c7fc5-110">Relationships</span></span>
| <span data-ttu-id="c7fc5-111">Relação</span><span class="sxs-lookup"><span data-stu-id="c7fc5-111">Relationship</span></span> | <span data-ttu-id="c7fc5-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="c7fc5-112">Type</span></span>   |<span data-ttu-id="c7fc5-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="c7fc5-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c7fc5-114">fill</span><span class="sxs-lookup"><span data-stu-id="c7fc5-114">fill</span></span>|[<span data-ttu-id="c7fc5-115">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="c7fc5-115">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="c7fc5-p101">Representa o formato de preenchimento de um objeto, que inclui informações sobre a formatação da tela de fundo. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c7fc5-p101">Represents the fill format of an object, which includes background formatting information. Read-only.</span></span>|
|<span data-ttu-id="c7fc5-118">font</span><span class="sxs-lookup"><span data-stu-id="c7fc5-118">font</span></span>|[<span data-ttu-id="c7fc5-119">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="c7fc5-119">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="c7fc5-120">Representa os atributos de fonte do objeto atual, como nome, tamanho, cor, dentre outros.</span><span class="sxs-lookup"><span data-stu-id="c7fc5-120">Represents the font attributes (font name, font size, color, etc.) for the current object.</span></span> <span data-ttu-id="c7fc5-121">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c7fc5-121">Read-only.</span></span>|



## <a name="json-representation"></a><span data-ttu-id="c7fc5-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c7fc5-122">JSON representation</span></span>

<span data-ttu-id="c7fc5-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c7fc5-123">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartTitleFormat"
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
  "description": "ChartAreaFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

