---
title: tipo de recurso workbookChartAxisFormat
description: Encapsula as propriedades de formato do eixo do gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 0bb5375edc2a2e504b602d6b66720ac9aee9bc55
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519369"
---
# <a name="workbookchartaxisformat-resource-type"></a><span data-ttu-id="b6be1-103">tipo de recurso workbookChartAxisFormat</span><span class="sxs-lookup"><span data-stu-id="b6be1-103">workbookChartAxisFormat resource type</span></span>

<span data-ttu-id="b6be1-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="b6be1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b6be1-105">Encapsula as propriedades de formato do eixo do gráfico.</span><span class="sxs-lookup"><span data-stu-id="b6be1-105">Encapsulates the format properties for the chart axis.</span></span>


## <a name="methods"></a><span data-ttu-id="b6be1-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="b6be1-106">Methods</span></span>
<span data-ttu-id="b6be1-107">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b6be1-107">None</span></span>
## <a name="properties"></a><span data-ttu-id="b6be1-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b6be1-108">Properties</span></span>
<span data-ttu-id="b6be1-109">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="b6be1-109">None</span></span>

## <a name="relationships"></a><span data-ttu-id="b6be1-110">Relações</span><span class="sxs-lookup"><span data-stu-id="b6be1-110">Relationships</span></span>
| <span data-ttu-id="b6be1-111">Relação</span><span class="sxs-lookup"><span data-stu-id="b6be1-111">Relationship</span></span> | <span data-ttu-id="b6be1-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="b6be1-112">Type</span></span>   |<span data-ttu-id="b6be1-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="b6be1-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b6be1-114">font</span><span class="sxs-lookup"><span data-stu-id="b6be1-114">font</span></span>|[<span data-ttu-id="b6be1-115">workbookChartFont</span><span class="sxs-lookup"><span data-stu-id="b6be1-115">workbookChartFont</span></span>](workbookchartfont.md)|<span data-ttu-id="b6be1-p101">Representa os atributos de fonte de um elemento do eixo do gráfico, como nome, tamanho, cor, etc. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b6be1-p101">Represents the font attributes (font name, font size, color, etc.) for a chart axis element. Read-only.</span></span>|
|<span data-ttu-id="b6be1-118">line</span><span class="sxs-lookup"><span data-stu-id="b6be1-118">line</span></span>|[<span data-ttu-id="b6be1-119">workbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="b6be1-119">workbookChartLineFormat</span></span>](workbookchartlineformat.md)|<span data-ttu-id="b6be1-120">Representa a formatação de linha do gráfico.</span><span class="sxs-lookup"><span data-stu-id="b6be1-120">Represents chart line formatting.</span></span> <span data-ttu-id="b6be1-121">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b6be1-121">Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="b6be1-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b6be1-122">JSON representation</span></span>

<span data-ttu-id="b6be1-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b6be1-123">Here is a JSON representation of the resource.</span></span>

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
