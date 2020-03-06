---
title: Tipo de recurso ChartAxisTitleFormat
description: Representa a formatação do título do eixo do gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 62522cee67684141911511de26731879936b4f2b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531878"
---
# <a name="chartaxistitleformat-resource-type"></a><span data-ttu-id="272d5-103">Tipo de recurso ChartAxisTitleFormat</span><span class="sxs-lookup"><span data-stu-id="272d5-103">ChartAxisTitleFormat resource type</span></span>

<span data-ttu-id="272d5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="272d5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="272d5-105">Representa a formatação do título do eixo do gráfico.</span><span class="sxs-lookup"><span data-stu-id="272d5-105">Represents the chart axis title formatting.</span></span>


## <a name="methods"></a><span data-ttu-id="272d5-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="272d5-106">Methods</span></span>
<span data-ttu-id="272d5-107">Nenhum</span><span class="sxs-lookup"><span data-stu-id="272d5-107">None</span></span>

## <a name="properties"></a><span data-ttu-id="272d5-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="272d5-108">Properties</span></span>
<span data-ttu-id="272d5-109">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="272d5-109">None</span></span>

## <a name="relationships"></a><span data-ttu-id="272d5-110">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="272d5-110">Relationships</span></span>
| <span data-ttu-id="272d5-111">Relação</span><span class="sxs-lookup"><span data-stu-id="272d5-111">Relationship</span></span> | <span data-ttu-id="272d5-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="272d5-112">Type</span></span>   |<span data-ttu-id="272d5-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="272d5-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="272d5-114">font</span><span class="sxs-lookup"><span data-stu-id="272d5-114">font</span></span>|[<span data-ttu-id="272d5-115">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="272d5-115">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="272d5-116">Representa os atributos de fonte, como nome, tamanho, cor, etc., do objeto do eixo do gráfico.</span><span class="sxs-lookup"><span data-stu-id="272d5-116">Represents the font attributes, such as font name, font size, color, etc. of chart axis title object.</span></span> <span data-ttu-id="272d5-117">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="272d5-117">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="272d5-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="272d5-118">JSON representation</span></span>

<span data-ttu-id="272d5-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="272d5-119">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartAxisTitleFormat"
}-->

```json
{
  "font": {"@odata.type": "microsoft.graph.workbookChartFont"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartAxisTitleFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
