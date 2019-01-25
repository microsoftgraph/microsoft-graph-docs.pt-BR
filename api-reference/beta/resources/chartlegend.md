---
title: Tipo de recurso ChartLegend
description: Representa a legenda de um gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 13c054403eb93afce03775138c151e67bc2f57d7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528183"
---
# <a name="chartlegend-resource-type"></a><span data-ttu-id="34cf5-103">Tipo de recurso ChartLegend</span><span class="sxs-lookup"><span data-stu-id="34cf5-103">ChartLegend resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="34cf5-104">Representa a legenda de um gráfico.</span><span class="sxs-lookup"><span data-stu-id="34cf5-104">Represents the legend in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="34cf5-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="34cf5-105">Methods</span></span>

| <span data-ttu-id="34cf5-106">Método</span><span class="sxs-lookup"><span data-stu-id="34cf5-106">Method</span></span>           | <span data-ttu-id="34cf5-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="34cf5-107">Return Type</span></span>    |<span data-ttu-id="34cf5-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="34cf5-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="34cf5-109">Get ChartLegend</span><span class="sxs-lookup"><span data-stu-id="34cf5-109">[Get ChartLegend](../api/chartlegend-get.md)</span></span> | [<span data-ttu-id="34cf5-110">ChartLegend</span><span class="sxs-lookup"><span data-stu-id="34cf5-110">ChartLegend</span></span>](chartlegend.md) |<span data-ttu-id="34cf5-111">Leia as propriedades e os relacionamentos do objeto chartLegend.</span><span class="sxs-lookup"><span data-stu-id="34cf5-111">Read properties and relationships of chartLegend object.</span></span>|
|[<span data-ttu-id="34cf5-112">Update</span><span class="sxs-lookup"><span data-stu-id="34cf5-112">Update</span></span>](../api/chartlegend-update.md) | [<span data-ttu-id="34cf5-113">ChartLegend</span><span class="sxs-lookup"><span data-stu-id="34cf5-113">ChartLegend</span></span>](chartlegend.md) |<span data-ttu-id="34cf5-114">Atualize o objeto ChartLegend.</span><span class="sxs-lookup"><span data-stu-id="34cf5-114">Update ChartLegend object.</span></span> |

## <a name="properties"></a><span data-ttu-id="34cf5-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="34cf5-115">Properties</span></span>
| <span data-ttu-id="34cf5-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="34cf5-116">Property</span></span>     | <span data-ttu-id="34cf5-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="34cf5-117">Type</span></span>   |<span data-ttu-id="34cf5-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="34cf5-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="34cf5-119">overlay</span><span class="sxs-lookup"><span data-stu-id="34cf5-119">overlay</span></span>|<span data-ttu-id="34cf5-120">booliano</span><span class="sxs-lookup"><span data-stu-id="34cf5-120">boolean</span></span>|<span data-ttu-id="34cf5-121">Valor booliano para determinar se a legenda do gráfico deve se sobrepor ao corpo principal do gráfico.</span><span class="sxs-lookup"><span data-stu-id="34cf5-121">Boolean value for whether the chart legend should overlap with the main body of the chart.</span></span>|
|<span data-ttu-id="34cf5-122">position</span><span class="sxs-lookup"><span data-stu-id="34cf5-122">position</span></span>|<span data-ttu-id="34cf5-123">string</span><span class="sxs-lookup"><span data-stu-id="34cf5-123">string</span></span>|<span data-ttu-id="34cf5-p101">Representa a posição da legenda no gráfico. Os valores possíveis são: `Top`, `Bottom`, `Left`, `Right`, `Corner` e `Custom`.</span><span class="sxs-lookup"><span data-stu-id="34cf5-p101">Represents the position of the legend on the chart. Possible values are: `Top`, `Bottom`, `Left`, `Right`, `Corner`, `Custom`.</span></span>|
|<span data-ttu-id="34cf5-126">visible</span><span class="sxs-lookup"><span data-stu-id="34cf5-126">visible</span></span>|<span data-ttu-id="34cf5-127">booliano</span><span class="sxs-lookup"><span data-stu-id="34cf5-127">boolean</span></span>|<span data-ttu-id="34cf5-128">Um valor booliano que representa a visibilidade de um objeto ChartLegend.</span><span class="sxs-lookup"><span data-stu-id="34cf5-128">A boolean value the represents the visibility of a ChartLegend object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="34cf5-129">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="34cf5-129">Relationships</span></span>
| <span data-ttu-id="34cf5-130">Relação</span><span class="sxs-lookup"><span data-stu-id="34cf5-130">Relationship</span></span> | <span data-ttu-id="34cf5-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="34cf5-131">Type</span></span>   |<span data-ttu-id="34cf5-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="34cf5-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="34cf5-133">formato</span><span class="sxs-lookup"><span data-stu-id="34cf5-133">format</span></span>|[<span data-ttu-id="34cf5-134">ChartLegendFormat</span><span class="sxs-lookup"><span data-stu-id="34cf5-134">ChartLegendFormat</span></span>](chartlegendformat.md)|<span data-ttu-id="34cf5-p102">Representa a formatação de uma legenda de gráfico, que inclui a formatação de fonte e de preenchimento. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="34cf5-p102">Represents the formatting of a chart legend, which includes fill and font formatting. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="34cf5-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="34cf5-137">JSON representation</span></span>

<span data-ttu-id="34cf5-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="34cf5-138">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartLegend"
}-->

```json
{
  "overlay": true,
  "position": "string",
  "visible": true
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
  "suppressions": [
    "Error: /api-reference/beta/resources/chartlegend.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
