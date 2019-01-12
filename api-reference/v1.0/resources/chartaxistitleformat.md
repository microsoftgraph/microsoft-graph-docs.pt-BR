---
title: Tipo de recurso ChartAxisTitleFormat
description: Representa a formatação do título do eixo do gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 26d305d8bd4a0059123f77bd86cbbf5fd01dcea7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27959479"
---
# <a name="chartaxistitleformat-resource-type"></a><span data-ttu-id="a7841-103">Tipo de recurso ChartAxisTitleFormat</span><span class="sxs-lookup"><span data-stu-id="a7841-103">ChartAxisTitleFormat resource type</span></span>

<span data-ttu-id="a7841-104">Representa a formatação do título do eixo do gráfico.</span><span class="sxs-lookup"><span data-stu-id="a7841-104">Represents the chart axis title formatting.</span></span>


## <a name="methods"></a><span data-ttu-id="a7841-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="a7841-105">Methods</span></span>
<span data-ttu-id="a7841-106">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a7841-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="a7841-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a7841-107">Properties</span></span>
<span data-ttu-id="a7841-108">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a7841-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="a7841-109">Relações</span><span class="sxs-lookup"><span data-stu-id="a7841-109">Relationships</span></span>
| <span data-ttu-id="a7841-110">Relação</span><span class="sxs-lookup"><span data-stu-id="a7841-110">Relationship</span></span> | <span data-ttu-id="a7841-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="a7841-111">Type</span></span>   |<span data-ttu-id="a7841-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="a7841-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a7841-113">font</span><span class="sxs-lookup"><span data-stu-id="a7841-113">font</span></span>|[<span data-ttu-id="a7841-114">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="a7841-114">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="a7841-p101">Representa os atributos de fonte, como nome, tamanho, cor, etc., do objeto do eixo do gráfico. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a7841-p101">Represents the font attributes, such as font name, font size, color, etc. of chart axis title object. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a7841-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a7841-117">JSON representation</span></span>

<span data-ttu-id="a7841-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a7841-118">Here is a JSON representation of the resource.</span></span>

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
