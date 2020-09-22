---
title: Tipo de recurso ChartLegend
description: Representa a legenda de um gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 8b05e4c130eebe3ffc23af2389feb2846ef1474e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48069173"
---
# <a name="chartlegend-resource-type"></a><span data-ttu-id="0b9e5-103">Tipo de recurso ChartLegend</span><span class="sxs-lookup"><span data-stu-id="0b9e5-103">ChartLegend resource type</span></span>

<span data-ttu-id="0b9e5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0b9e5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0b9e5-105">Representa a legenda de um gráfico.</span><span class="sxs-lookup"><span data-stu-id="0b9e5-105">Represents the legend in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="0b9e5-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="0b9e5-106">Methods</span></span>

| <span data-ttu-id="0b9e5-107">Método</span><span class="sxs-lookup"><span data-stu-id="0b9e5-107">Method</span></span>           | <span data-ttu-id="0b9e5-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="0b9e5-108">Return Type</span></span>    |<span data-ttu-id="0b9e5-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="0b9e5-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0b9e5-110">Get ChartLegend</span><span class="sxs-lookup"><span data-stu-id="0b9e5-110">Get ChartLegend</span></span>](../api/chartlegend-get.md) | [<span data-ttu-id="0b9e5-111">WorkbookChartLegend</span><span class="sxs-lookup"><span data-stu-id="0b9e5-111">WorkbookChartLegend</span></span>](chartlegend.md) |<span data-ttu-id="0b9e5-112">Leia as propriedades e os relacionamentos do objeto chartLegend.</span><span class="sxs-lookup"><span data-stu-id="0b9e5-112">Read properties and relationships of chartLegend object.</span></span>|
|[<span data-ttu-id="0b9e5-113">Update</span><span class="sxs-lookup"><span data-stu-id="0b9e5-113">Update</span></span>](../api/chartlegend-update.md) | [<span data-ttu-id="0b9e5-114">WorkbookChartLegend</span><span class="sxs-lookup"><span data-stu-id="0b9e5-114">WorkbookChartLegend</span></span>](chartlegend.md) |<span data-ttu-id="0b9e5-115">Atualize o objeto ChartLegend.</span><span class="sxs-lookup"><span data-stu-id="0b9e5-115">Update ChartLegend object.</span></span> |

## <a name="properties"></a><span data-ttu-id="0b9e5-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0b9e5-116">Properties</span></span>
| <span data-ttu-id="0b9e5-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0b9e5-117">Property</span></span>     | <span data-ttu-id="0b9e5-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="0b9e5-118">Type</span></span>   |<span data-ttu-id="0b9e5-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="0b9e5-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0b9e5-120">overlay</span><span class="sxs-lookup"><span data-stu-id="0b9e5-120">overlay</span></span>|<span data-ttu-id="0b9e5-121">booliano</span><span class="sxs-lookup"><span data-stu-id="0b9e5-121">boolean</span></span>|<span data-ttu-id="0b9e5-122">Valor booliano para determinar se a legenda do gráfico deve se sobrepor ao corpo principal do gráfico.</span><span class="sxs-lookup"><span data-stu-id="0b9e5-122">Boolean value for whether the chart legend should overlap with the main body of the chart.</span></span>|
|<span data-ttu-id="0b9e5-123">position</span><span class="sxs-lookup"><span data-stu-id="0b9e5-123">position</span></span>|<span data-ttu-id="0b9e5-124">string</span><span class="sxs-lookup"><span data-stu-id="0b9e5-124">string</span></span>|<span data-ttu-id="0b9e5-125">Representa a posição da legenda no gráfico.</span><span class="sxs-lookup"><span data-stu-id="0b9e5-125">Represents the position of the legend on the chart.</span></span> <span data-ttu-id="0b9e5-126">Os valores possíveis são: `Top`, `Bottom`, `Left`, `Right`, `Corner`, `Custom`.</span><span class="sxs-lookup"><span data-stu-id="0b9e5-126">The possible values are: `Top`, `Bottom`, `Left`, `Right`, `Corner`, `Custom`.</span></span>|
|<span data-ttu-id="0b9e5-127">visible</span><span class="sxs-lookup"><span data-stu-id="0b9e5-127">visible</span></span>|<span data-ttu-id="0b9e5-128">booliano</span><span class="sxs-lookup"><span data-stu-id="0b9e5-128">boolean</span></span>|<span data-ttu-id="0b9e5-129">Um valor booliano que representa a visibilidade de um objeto ChartLegend.</span><span class="sxs-lookup"><span data-stu-id="0b9e5-129">A boolean value the represents the visibility of a ChartLegend object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0b9e5-130">Relações</span><span class="sxs-lookup"><span data-stu-id="0b9e5-130">Relationships</span></span>
| <span data-ttu-id="0b9e5-131">Relação</span><span class="sxs-lookup"><span data-stu-id="0b9e5-131">Relationship</span></span> | <span data-ttu-id="0b9e5-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="0b9e5-132">Type</span></span>   |<span data-ttu-id="0b9e5-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="0b9e5-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0b9e5-134">formato</span><span class="sxs-lookup"><span data-stu-id="0b9e5-134">format</span></span>|[<span data-ttu-id="0b9e5-135">WorkbookChartLegendFormat</span><span class="sxs-lookup"><span data-stu-id="0b9e5-135">WorkbookChartLegendFormat</span></span>](chartlegendformat.md)|<span data-ttu-id="0b9e5-136">Representa a formatação de uma legenda de gráfico, que inclui a formatação de fonte e de preenchimento.</span><span class="sxs-lookup"><span data-stu-id="0b9e5-136">Represents the formatting of a chart legend, which includes fill and font formatting.</span></span> <span data-ttu-id="0b9e5-137">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0b9e5-137">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0b9e5-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0b9e5-138">JSON representation</span></span>

<span data-ttu-id="0b9e5-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0b9e5-139">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookChartLegend"
}-->

```json
{
  "overlay": true,
  "position": "string",
  "visible": true,
  "format": {"@odata.type":"microsoft.graph.workbookChartLegendFormat"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartLegend resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

