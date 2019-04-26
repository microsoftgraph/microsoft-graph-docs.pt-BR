---
title: Tipo de recurso ChartLegend
description: Representa a legenda de um gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 8eea71707d622f0dc28cc8072fa984de64a8427f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32569099"
---
# <a name="chartlegend-resource-type"></a><span data-ttu-id="52cb9-103">Tipo de recurso ChartLegend</span><span class="sxs-lookup"><span data-stu-id="52cb9-103">ChartLegend resource type</span></span>

<span data-ttu-id="52cb9-104">Representa a legenda de um gráfico.</span><span class="sxs-lookup"><span data-stu-id="52cb9-104">Represents the legend in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="52cb9-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="52cb9-105">Methods</span></span>

| <span data-ttu-id="52cb9-106">Método</span><span class="sxs-lookup"><span data-stu-id="52cb9-106">Method</span></span>           | <span data-ttu-id="52cb9-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="52cb9-107">Return Type</span></span>    |<span data-ttu-id="52cb9-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="52cb9-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="52cb9-109">Get ChartLegend</span><span class="sxs-lookup"><span data-stu-id="52cb9-109">Get ChartLegend</span></span>](../api/chartlegend-get.md) | [<span data-ttu-id="52cb9-110">WorkbookChartLegend</span><span class="sxs-lookup"><span data-stu-id="52cb9-110">WorkbookChartLegend</span></span>](chartlegend.md) |<span data-ttu-id="52cb9-111">Leia as propriedades e os relacionamentos do objeto chartLegend.</span><span class="sxs-lookup"><span data-stu-id="52cb9-111">Read properties and relationships of chartLegend object.</span></span>|
|[<span data-ttu-id="52cb9-112">Update</span><span class="sxs-lookup"><span data-stu-id="52cb9-112">Update</span></span>](../api/chartlegend-update.md) | [<span data-ttu-id="52cb9-113">WorkbookChartLegend</span><span class="sxs-lookup"><span data-stu-id="52cb9-113">WorkbookChartLegend</span></span>](chartlegend.md) |<span data-ttu-id="52cb9-114">Atualize o objeto ChartLegend.</span><span class="sxs-lookup"><span data-stu-id="52cb9-114">Update ChartLegend object.</span></span> |

## <a name="properties"></a><span data-ttu-id="52cb9-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="52cb9-115">Properties</span></span>
| <span data-ttu-id="52cb9-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="52cb9-116">Property</span></span>     | <span data-ttu-id="52cb9-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="52cb9-117">Type</span></span>   |<span data-ttu-id="52cb9-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="52cb9-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="52cb9-119">overlay</span><span class="sxs-lookup"><span data-stu-id="52cb9-119">overlay</span></span>|<span data-ttu-id="52cb9-120">booliano</span><span class="sxs-lookup"><span data-stu-id="52cb9-120">boolean</span></span>|<span data-ttu-id="52cb9-121">Valor booliano para determinar se a legenda do gráfico deve se sobrepor ao corpo principal do gráfico.</span><span class="sxs-lookup"><span data-stu-id="52cb9-121">Boolean value for whether the chart legend should overlap with the main body of the chart.</span></span>|
|<span data-ttu-id="52cb9-122">position</span><span class="sxs-lookup"><span data-stu-id="52cb9-122">position</span></span>|<span data-ttu-id="52cb9-123">string</span><span class="sxs-lookup"><span data-stu-id="52cb9-123">string</span></span>|<span data-ttu-id="52cb9-124">Representa a posição da legenda no gráfico.</span><span class="sxs-lookup"><span data-stu-id="52cb9-124">Represents the position of the legend on the chart.</span></span> <span data-ttu-id="52cb9-125">Os valores possíveis são: `Top`, `Bottom`, `Left`, `Right`, `Corner`, `Custom`.</span><span class="sxs-lookup"><span data-stu-id="52cb9-125">The possible values are: `Top`, `Bottom`, `Left`, `Right`, `Corner`, `Custom`.</span></span>|
|<span data-ttu-id="52cb9-126">visible</span><span class="sxs-lookup"><span data-stu-id="52cb9-126">visible</span></span>|<span data-ttu-id="52cb9-127">booliano</span><span class="sxs-lookup"><span data-stu-id="52cb9-127">boolean</span></span>|<span data-ttu-id="52cb9-128">Um valor booliano que representa a visibilidade de um objeto ChartLegend.</span><span class="sxs-lookup"><span data-stu-id="52cb9-128">A boolean value the represents the visibility of a ChartLegend object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="52cb9-129">Relações</span><span class="sxs-lookup"><span data-stu-id="52cb9-129">Relationships</span></span>
| <span data-ttu-id="52cb9-130">Relação</span><span class="sxs-lookup"><span data-stu-id="52cb9-130">Relationship</span></span> | <span data-ttu-id="52cb9-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="52cb9-131">Type</span></span>   |<span data-ttu-id="52cb9-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="52cb9-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="52cb9-133">format</span><span class="sxs-lookup"><span data-stu-id="52cb9-133">format</span></span>|[<span data-ttu-id="52cb9-134">WorkbookChartLegendFormat</span><span class="sxs-lookup"><span data-stu-id="52cb9-134">WorkbookChartLegendFormat</span></span>](chartlegendformat.md)|<span data-ttu-id="52cb9-135">Representa a formatação de uma legenda de gráfico, que inclui a formatação de fonte e de preenchimento.</span><span class="sxs-lookup"><span data-stu-id="52cb9-135">Represents the formatting of a chart legend, which includes fill and font formatting.</span></span> <span data-ttu-id="52cb9-136">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="52cb9-136">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="52cb9-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="52cb9-137">JSON representation</span></span>

<span data-ttu-id="52cb9-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="52cb9-138">Here is a JSON representation of the resource.</span></span>

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
