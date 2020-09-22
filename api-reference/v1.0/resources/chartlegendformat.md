---
title: Tipo de recurso ChartLegendFormat
description: Encapsula as propriedades de formato de uma legenda de gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: f4d018fd01a9ad9899eefcb663b0860096567c84
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47988390"
---
# <a name="chartlegendformat-resource-type"></a><span data-ttu-id="afb24-103">Tipo de recurso ChartLegendFormat</span><span class="sxs-lookup"><span data-stu-id="afb24-103">ChartLegendFormat resource type</span></span>

<span data-ttu-id="afb24-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="afb24-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="afb24-105">Encapsula as propriedades de formato de uma legenda de gráfico.</span><span class="sxs-lookup"><span data-stu-id="afb24-105">Encapsulates the format properties of a chart legend.</span></span>


## <a name="methods"></a><span data-ttu-id="afb24-106">Methods</span><span class="sxs-lookup"><span data-stu-id="afb24-106">Methods</span></span>
<span data-ttu-id="afb24-107">Nenhum</span><span class="sxs-lookup"><span data-stu-id="afb24-107">None</span></span>

## <a name="properties"></a><span data-ttu-id="afb24-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="afb24-108">Properties</span></span>
<span data-ttu-id="afb24-109">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="afb24-109">None</span></span>

## <a name="relationships"></a><span data-ttu-id="afb24-110">Relações</span><span class="sxs-lookup"><span data-stu-id="afb24-110">Relationships</span></span>
| <span data-ttu-id="afb24-111">Relação</span><span class="sxs-lookup"><span data-stu-id="afb24-111">Relationship</span></span> | <span data-ttu-id="afb24-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="afb24-112">Type</span></span>   |<span data-ttu-id="afb24-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="afb24-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="afb24-114">fill</span><span class="sxs-lookup"><span data-stu-id="afb24-114">fill</span></span>|[<span data-ttu-id="afb24-115">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="afb24-115">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="afb24-p101">Representa o formato de preenchimento de um objeto, que inclui informações sobre a formatação da tela de fundo. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="afb24-p101">Represents the fill format of an object, which includes background formating information. Read-only.</span></span>|
|<span data-ttu-id="afb24-118">fonte</span><span class="sxs-lookup"><span data-stu-id="afb24-118">font</span></span>|[<span data-ttu-id="afb24-119">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="afb24-119">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="afb24-120">Representa os atributos de fonte, como nome da fonte, tamanho da fonte, cor, etc. de uma legenda do gráfico.</span><span class="sxs-lookup"><span data-stu-id="afb24-120">Represents the font attributes such as font name, font size, color, etc. of a chart legend.</span></span> <span data-ttu-id="afb24-121">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="afb24-121">Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="afb24-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="afb24-122">JSON representation</span></span>

<span data-ttu-id="afb24-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="afb24-123">Here is a JSON representation of the resource.</span></span>

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

