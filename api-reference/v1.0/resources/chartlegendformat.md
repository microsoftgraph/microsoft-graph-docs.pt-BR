---
title: Tipo de recurso ChartLegendFormat
description: Abrange as propriedades de formato de uma legenda de gráfico.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 7d57ad66da6e5f280684cf364ac7890bcc3ed259
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27811064"
---
# <a name="chartlegendformat-resource-type"></a><span data-ttu-id="f60a5-103">Tipo de recurso ChartLegendFormat</span><span class="sxs-lookup"><span data-stu-id="f60a5-103">ChartLegendFormat resource type</span></span>

<span data-ttu-id="f60a5-104">Abrange as propriedades de formato de uma legenda de gráfico.</span><span class="sxs-lookup"><span data-stu-id="f60a5-104">Encapsulates the format properties of a chart legend.</span></span>


## <a name="methods"></a><span data-ttu-id="f60a5-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="f60a5-105">Methods</span></span>
<span data-ttu-id="f60a5-106">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f60a5-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="f60a5-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f60a5-107">Properties</span></span>
<span data-ttu-id="f60a5-108">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f60a5-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="f60a5-109">Relações</span><span class="sxs-lookup"><span data-stu-id="f60a5-109">Relationships</span></span>
| <span data-ttu-id="f60a5-110">Relação</span><span class="sxs-lookup"><span data-stu-id="f60a5-110">Relationship</span></span> | <span data-ttu-id="f60a5-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="f60a5-111">Type</span></span>   |<span data-ttu-id="f60a5-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="f60a5-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f60a5-113">fill</span><span class="sxs-lookup"><span data-stu-id="f60a5-113">fill</span></span>|[<span data-ttu-id="f60a5-114">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="f60a5-114">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="f60a5-p101">Representa o formato de preenchimento de um objeto, que inclui informações sobre a formatação da tela de fundo. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f60a5-p101">Represents the fill format of an object, which includes background formating information. Read-only.</span></span>|
|<span data-ttu-id="f60a5-117">font</span><span class="sxs-lookup"><span data-stu-id="f60a5-117">font</span></span>|[<span data-ttu-id="f60a5-118">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="f60a5-118">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="f60a5-p102">Representa os atributos de fonte, como nome, tamanho, cor, etc. de uma legenda de gráfico. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f60a5-p102">Represents the font attributes such as font name, font size, color, etc. of a chart legend. Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="f60a5-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f60a5-121">JSON representation</span></span>

<span data-ttu-id="f60a5-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f60a5-122">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartLegendFormat"
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
  "description": "ChartLegendFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
