---
title: tipo de recurso workbookChartLegend
description: Representa a legenda de um gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 60d37ab606668fbe6828293112997980c7e4580c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519306"
---
# <a name="workbookchartlegend-resource-type"></a><span data-ttu-id="40129-103">tipo de recurso workbookChartLegend</span><span class="sxs-lookup"><span data-stu-id="40129-103">workbookChartLegend resource type</span></span>

<span data-ttu-id="40129-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="40129-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="40129-105">Representa a legenda de um gráfico.</span><span class="sxs-lookup"><span data-stu-id="40129-105">Represents the legend in a chart.</span></span>

## <a name="methods"></a><span data-ttu-id="40129-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="40129-106">Methods</span></span>

| <span data-ttu-id="40129-107">Método</span><span class="sxs-lookup"><span data-stu-id="40129-107">Method</span></span>           | <span data-ttu-id="40129-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="40129-108">Return Type</span></span>    |<span data-ttu-id="40129-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="40129-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="40129-110">Obter workbookChartLegend</span><span class="sxs-lookup"><span data-stu-id="40129-110">Get workbookChartLegend</span></span>](../api/chartlegend-get.md) | [<span data-ttu-id="40129-111">workbookChartLegend</span><span class="sxs-lookup"><span data-stu-id="40129-111">workbookChartLegend</span></span>](workbookchartlegend.md) |<span data-ttu-id="40129-112">Leia as propriedades e os relacionamentos do objeto chartLegend.</span><span class="sxs-lookup"><span data-stu-id="40129-112">Read properties and relationships of chartLegend object.</span></span>|
|[<span data-ttu-id="40129-113">Update</span><span class="sxs-lookup"><span data-stu-id="40129-113">Update</span></span>](../api/chartlegend-update.md) | [<span data-ttu-id="40129-114">workbookChartLegend</span><span class="sxs-lookup"><span data-stu-id="40129-114">workbookChartLegend</span></span>](workbookchartlegend.md) |<span data-ttu-id="40129-115">Atualize o objeto ChartLegend.</span><span class="sxs-lookup"><span data-stu-id="40129-115">Update ChartLegend object.</span></span> |

## <a name="properties"></a><span data-ttu-id="40129-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="40129-116">Properties</span></span>
| <span data-ttu-id="40129-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="40129-117">Property</span></span>     | <span data-ttu-id="40129-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="40129-118">Type</span></span>   |<span data-ttu-id="40129-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="40129-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="40129-120">overlay</span><span class="sxs-lookup"><span data-stu-id="40129-120">overlay</span></span>|<span data-ttu-id="40129-121">booliano</span><span class="sxs-lookup"><span data-stu-id="40129-121">boolean</span></span>|<span data-ttu-id="40129-122">Valor booliano para determinar se a legenda do gráfico deve se sobrepor ao corpo principal do gráfico.</span><span class="sxs-lookup"><span data-stu-id="40129-122">Boolean value for whether the chart legend should overlap with the main body of the chart.</span></span>|
|<span data-ttu-id="40129-123">position</span><span class="sxs-lookup"><span data-stu-id="40129-123">position</span></span>|<span data-ttu-id="40129-124">string</span><span class="sxs-lookup"><span data-stu-id="40129-124">string</span></span>|<span data-ttu-id="40129-125">Representa a posição da legenda no gráfico.</span><span class="sxs-lookup"><span data-stu-id="40129-125">Represents the position of the legend on the chart.</span></span> <span data-ttu-id="40129-126">Os valores possíveis são: `Top`, `Bottom`, `Left`, `Right`, `Corner`, `Custom`.</span><span class="sxs-lookup"><span data-stu-id="40129-126">The possible values are: `Top`, `Bottom`, `Left`, `Right`, `Corner`, `Custom`.</span></span>|
|<span data-ttu-id="40129-127">visible</span><span class="sxs-lookup"><span data-stu-id="40129-127">visible</span></span>|<span data-ttu-id="40129-128">booliano</span><span class="sxs-lookup"><span data-stu-id="40129-128">boolean</span></span>|<span data-ttu-id="40129-129">Um valor booliano que representa a visibilidade de um objeto ChartLegend.</span><span class="sxs-lookup"><span data-stu-id="40129-129">A boolean value the represents the visibility of a ChartLegend object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="40129-130">Relações</span><span class="sxs-lookup"><span data-stu-id="40129-130">Relationships</span></span>
| <span data-ttu-id="40129-131">Relação</span><span class="sxs-lookup"><span data-stu-id="40129-131">Relationship</span></span> | <span data-ttu-id="40129-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="40129-132">Type</span></span>   |<span data-ttu-id="40129-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="40129-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="40129-134">formato</span><span class="sxs-lookup"><span data-stu-id="40129-134">format</span></span>|[<span data-ttu-id="40129-135">workbookChartLegendFormat</span><span class="sxs-lookup"><span data-stu-id="40129-135">workbookChartLegendFormat</span></span>](workbookchartlegendformat.md)|<span data-ttu-id="40129-136">Representa a formatação de uma legenda de gráfico, que inclui a formatação de fonte e de preenchimento.</span><span class="sxs-lookup"><span data-stu-id="40129-136">Represents the formatting of a chart legend, which includes fill and font formatting.</span></span> <span data-ttu-id="40129-137">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="40129-137">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="40129-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="40129-138">JSON representation</span></span>

<span data-ttu-id="40129-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="40129-139">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [
    "format"        
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
<!--
{
  "type": "#page.annotation",
  "description": "ChartLegend resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
