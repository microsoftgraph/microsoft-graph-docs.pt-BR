---
title: Tipo de recurso ChartAxisTitleFormat
description: Representa a formatação do título do eixo do gráfico.
author: lumine2008
ms.openlocfilehash: 7a160f02f06c74edeee09f91b2b117ea437291e8
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27343016"
---
# <a name="chartaxistitleformat-resource-type"></a><span data-ttu-id="4e834-103">Tipo de recurso ChartAxisTitleFormat</span><span class="sxs-lookup"><span data-stu-id="4e834-103">ChartAxisTitleFormat resource type</span></span>

<span data-ttu-id="4e834-104">Representa a formatação do título do eixo do gráfico.</span><span class="sxs-lookup"><span data-stu-id="4e834-104">Represents the chart axis title formatting.</span></span>


## <a name="methods"></a><span data-ttu-id="4e834-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="4e834-105">Methods</span></span>
<span data-ttu-id="4e834-106">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4e834-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="4e834-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4e834-107">Properties</span></span>
<span data-ttu-id="4e834-108">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4e834-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="4e834-109">Relações</span><span class="sxs-lookup"><span data-stu-id="4e834-109">Relationships</span></span>
| <span data-ttu-id="4e834-110">Relação</span><span class="sxs-lookup"><span data-stu-id="4e834-110">Relationship</span></span> | <span data-ttu-id="4e834-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="4e834-111">Type</span></span>   |<span data-ttu-id="4e834-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="4e834-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4e834-113">font</span><span class="sxs-lookup"><span data-stu-id="4e834-113">font</span></span>|[<span data-ttu-id="4e834-114">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="4e834-114">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="4e834-p101">Representa os atributos de fonte, como nome, tamanho, cor, etc., do objeto do eixo do gráfico. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4e834-p101">Represents the font attributes, such as font name, font size, color, etc. of chart axis title object. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4e834-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4e834-117">JSON representation</span></span>

<span data-ttu-id="4e834-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4e834-118">Here is a JSON representation of the resource.</span></span>

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