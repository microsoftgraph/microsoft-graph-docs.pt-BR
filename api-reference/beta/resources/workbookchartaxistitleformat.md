---
title: tipo de recurso workbookChartAxisTitleFormat
description: Representa a formatação do título do eixo do gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: c585fc426474fe0a7790874331a2ae53227fc1a7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48039046"
---
# <a name="workbookchartaxistitleformat-resource-type"></a><span data-ttu-id="70a5e-103">tipo de recurso workbookChartAxisTitleFormat</span><span class="sxs-lookup"><span data-stu-id="70a5e-103">workbookChartAxisTitleFormat resource type</span></span>

<span data-ttu-id="70a5e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="70a5e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="70a5e-105">Representa a formatação do título do eixo do gráfico.</span><span class="sxs-lookup"><span data-stu-id="70a5e-105">Represents the chart axis title formatting.</span></span>


## <a name="methods"></a><span data-ttu-id="70a5e-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="70a5e-106">Methods</span></span>
<span data-ttu-id="70a5e-107">Nenhum</span><span class="sxs-lookup"><span data-stu-id="70a5e-107">None</span></span>

## <a name="properties"></a><span data-ttu-id="70a5e-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="70a5e-108">Properties</span></span>
<span data-ttu-id="70a5e-109">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="70a5e-109">None</span></span>

## <a name="relationships"></a><span data-ttu-id="70a5e-110">Relações</span><span class="sxs-lookup"><span data-stu-id="70a5e-110">Relationships</span></span>
| <span data-ttu-id="70a5e-111">Relação</span><span class="sxs-lookup"><span data-stu-id="70a5e-111">Relationship</span></span> | <span data-ttu-id="70a5e-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="70a5e-112">Type</span></span>   |<span data-ttu-id="70a5e-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="70a5e-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="70a5e-114">font</span><span class="sxs-lookup"><span data-stu-id="70a5e-114">font</span></span>|[<span data-ttu-id="70a5e-115">workbookChartFont</span><span class="sxs-lookup"><span data-stu-id="70a5e-115">workbookChartFont</span></span>](workbookchartfont.md)|<span data-ttu-id="70a5e-116">Representa os atributos de fonte, como nome, tamanho, cor, etc., do objeto do eixo do gráfico.</span><span class="sxs-lookup"><span data-stu-id="70a5e-116">Represents the font attributes, such as font name, font size, color, etc. of chart axis title object.</span></span> <span data-ttu-id="70a5e-117">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="70a5e-117">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="70a5e-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="70a5e-118">JSON representation</span></span>

<span data-ttu-id="70a5e-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="70a5e-119">Here is a JSON representation of the resource.</span></span>

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


