---
title: Tipo de recurso ChartLegendFormat
description: Abrange as propriedades de formato de uma legenda de gráfico.
author: lumine2008
ms.openlocfilehash: 6ef6f2d26ade1d8d93489fbc560d4e0eb511bc86
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27334374"
---
# <a name="chartlegendformat-resource-type"></a><span data-ttu-id="70d60-103">Tipo de recurso ChartLegendFormat</span><span class="sxs-lookup"><span data-stu-id="70d60-103">ChartLegendFormat resource type</span></span>

<span data-ttu-id="70d60-104">Abrange as propriedades de formato de uma legenda de gráfico.</span><span class="sxs-lookup"><span data-stu-id="70d60-104">Encapsulates the format properties of a chart legend.</span></span>


## <a name="methods"></a><span data-ttu-id="70d60-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="70d60-105">Methods</span></span>
<span data-ttu-id="70d60-106">Nenhum</span><span class="sxs-lookup"><span data-stu-id="70d60-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="70d60-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="70d60-107">Properties</span></span>
<span data-ttu-id="70d60-108">Nenhum</span><span class="sxs-lookup"><span data-stu-id="70d60-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="70d60-109">Relações</span><span class="sxs-lookup"><span data-stu-id="70d60-109">Relationships</span></span>
| <span data-ttu-id="70d60-110">Relação</span><span class="sxs-lookup"><span data-stu-id="70d60-110">Relationship</span></span> | <span data-ttu-id="70d60-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="70d60-111">Type</span></span>   |<span data-ttu-id="70d60-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="70d60-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="70d60-113">fill</span><span class="sxs-lookup"><span data-stu-id="70d60-113">fill</span></span>|[<span data-ttu-id="70d60-114">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="70d60-114">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="70d60-p101">Representa o formato de preenchimento de um objeto, que inclui informações sobre a formatação da tela de fundo. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="70d60-p101">Represents the fill format of an object, which includes background formating information. Read-only.</span></span>|
|<span data-ttu-id="70d60-117">font</span><span class="sxs-lookup"><span data-stu-id="70d60-117">font</span></span>|[<span data-ttu-id="70d60-118">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="70d60-118">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="70d60-p102">Representa os atributos de fonte, como nome, tamanho, cor, etc. de uma legenda de gráfico. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="70d60-p102">Represents the font attributes such as font name, font size, color, etc. of a chart legend. Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="70d60-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="70d60-121">JSON representation</span></span>

<span data-ttu-id="70d60-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="70d60-122">Here is a JSON representation of the resource.</span></span>

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