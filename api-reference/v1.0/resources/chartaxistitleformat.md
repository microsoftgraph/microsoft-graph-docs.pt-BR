---
title: Tipo de recurso ChartAxisTitleFormat
description: Representa a formatação do título do eixo do gráfico.
ms.openlocfilehash: 417c594096ae19c0a223eaeaa543827f91306e8c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006051"
---
# <a name="chartaxistitleformat-resource-type"></a><span data-ttu-id="531d5-103">Tipo de recurso ChartAxisTitleFormat</span><span class="sxs-lookup"><span data-stu-id="531d5-103">ChartAxisTitleFormat resource type</span></span>

<span data-ttu-id="531d5-104">Representa a formatação do título do eixo do gráfico.</span><span class="sxs-lookup"><span data-stu-id="531d5-104">Represents the chart axis title formatting.</span></span>


## <a name="methods"></a><span data-ttu-id="531d5-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="531d5-105">Methods</span></span>
<span data-ttu-id="531d5-106">Nenhum</span><span class="sxs-lookup"><span data-stu-id="531d5-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="531d5-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="531d5-107">Properties</span></span>
<span data-ttu-id="531d5-108">Nenhum</span><span class="sxs-lookup"><span data-stu-id="531d5-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="531d5-109">Relações</span><span class="sxs-lookup"><span data-stu-id="531d5-109">Relationships</span></span>
| <span data-ttu-id="531d5-110">Relação</span><span class="sxs-lookup"><span data-stu-id="531d5-110">Relationship</span></span> | <span data-ttu-id="531d5-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="531d5-111">Type</span></span>   |<span data-ttu-id="531d5-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="531d5-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="531d5-113">font</span><span class="sxs-lookup"><span data-stu-id="531d5-113">font</span></span>|[<span data-ttu-id="531d5-114">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="531d5-114">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="531d5-p101">Representa os atributos de fonte, como nome, tamanho, cor, etc., do objeto do eixo do gráfico. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="531d5-p101">Represents the font attributes, such as font name, font size, color, etc. of chart axis title object. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="531d5-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="531d5-117">JSON representation</span></span>

<span data-ttu-id="531d5-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="531d5-118">Here is a JSON representation of the resource.</span></span>

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