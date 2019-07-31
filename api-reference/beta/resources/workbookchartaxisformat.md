---
title: tipo de recurso workbookChartAxisFormat
description: Encapsula as propriedades de formato do eixo do gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 91e749fd0f1449883eca261f5ef27c0f2a7ba5dc
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964082"
---
# <a name="workbookchartaxisformat-resource-type"></a><span data-ttu-id="889f0-103">tipo de recurso workbookChartAxisFormat</span><span class="sxs-lookup"><span data-stu-id="889f0-103">workbookChartAxisFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="889f0-104">Encapsula as propriedades de formato do eixo do gráfico.</span><span class="sxs-lookup"><span data-stu-id="889f0-104">Encapsulates the format properties for the chart axis.</span></span>


## <a name="methods"></a><span data-ttu-id="889f0-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="889f0-105">Methods</span></span>
<span data-ttu-id="889f0-106">Nenhum</span><span class="sxs-lookup"><span data-stu-id="889f0-106">None</span></span>
## <a name="properties"></a><span data-ttu-id="889f0-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="889f0-107">Properties</span></span>
<span data-ttu-id="889f0-108">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="889f0-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="889f0-109">Relações</span><span class="sxs-lookup"><span data-stu-id="889f0-109">Relationships</span></span>
| <span data-ttu-id="889f0-110">Relação</span><span class="sxs-lookup"><span data-stu-id="889f0-110">Relationship</span></span> | <span data-ttu-id="889f0-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="889f0-111">Type</span></span>   |<span data-ttu-id="889f0-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="889f0-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="889f0-113">font</span><span class="sxs-lookup"><span data-stu-id="889f0-113">font</span></span>|[<span data-ttu-id="889f0-114">workbookChartFont</span><span class="sxs-lookup"><span data-stu-id="889f0-114">workbookChartFont</span></span>](workbookchartfont.md)|<span data-ttu-id="889f0-p101">Representa os atributos de fonte de um elemento do eixo do gráfico, como nome, tamanho, cor, etc. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="889f0-p101">Represents the font attributes (font name, font size, color, etc.) for a chart axis element. Read-only.</span></span>|
|<span data-ttu-id="889f0-117">line</span><span class="sxs-lookup"><span data-stu-id="889f0-117">line</span></span>|[<span data-ttu-id="889f0-118">workbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="889f0-118">workbookChartLineFormat</span></span>](workbookchartlineformat.md)|<span data-ttu-id="889f0-119">Representa a formatação de linha do gráfico.</span><span class="sxs-lookup"><span data-stu-id="889f0-119">Represents chart line formatting.</span></span> <span data-ttu-id="889f0-120">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="889f0-120">Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="889f0-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="889f0-121">JSON representation</span></span>

<span data-ttu-id="889f0-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="889f0-122">Here is a JSON representation of the resource.</span></span>

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
