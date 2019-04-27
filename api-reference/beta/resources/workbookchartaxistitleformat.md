---
title: tipo de recurso workbookChartAxisTitleFormat
description: Representa a formatação do título do eixo do gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: c98cfee5c776f761c4e84479bb6a4b3f2814bb06
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348457"
---
# <a name="workbookchartaxistitleformat-resource-type"></a><span data-ttu-id="fd043-103">tipo de recurso workbookChartAxisTitleFormat</span><span class="sxs-lookup"><span data-stu-id="fd043-103">workbookChartAxisTitleFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fd043-104">Representa a formatação do título do eixo do gráfico.</span><span class="sxs-lookup"><span data-stu-id="fd043-104">Represents the chart axis title formatting.</span></span>


## <a name="methods"></a><span data-ttu-id="fd043-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="fd043-105">Methods</span></span>
<span data-ttu-id="fd043-106">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fd043-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="fd043-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fd043-107">Properties</span></span>
<span data-ttu-id="fd043-108">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="fd043-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="fd043-109">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="fd043-109">Relationships</span></span>
| <span data-ttu-id="fd043-110">Relação</span><span class="sxs-lookup"><span data-stu-id="fd043-110">Relationship</span></span> | <span data-ttu-id="fd043-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="fd043-111">Type</span></span>   |<span data-ttu-id="fd043-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="fd043-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fd043-113">font</span><span class="sxs-lookup"><span data-stu-id="fd043-113">font</span></span>|[<span data-ttu-id="fd043-114">workbookChartFont</span><span class="sxs-lookup"><span data-stu-id="fd043-114">workbookChartFont</span></span>](workbookchartfont.md)|<span data-ttu-id="fd043-115">Representa os atributos de fonte, como nome, tamanho, cor, etc., do objeto do eixo do gráfico.</span><span class="sxs-lookup"><span data-stu-id="fd043-115">Represents the font attributes, such as font name, font size, color, etc. of chart axis title object.</span></span> <span data-ttu-id="fd043-116">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fd043-116">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fd043-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fd043-117">JSON representation</span></span>

<span data-ttu-id="fd043-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fd043-118">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "font"
    ],
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
<!--
{
  "type": "#page.annotation",
  "description": "ChartAxisTitleFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
