---
title: Tipo de recurso ChartLegend
description: Representa a legenda de um gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 13c054403eb93afce03775138c151e67bc2f57d7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543736"
---
# <a name="chartlegend-resource-type"></a><span data-ttu-id="5ef13-103">Tipo de recurso ChartLegend</span><span class="sxs-lookup"><span data-stu-id="5ef13-103">ChartLegend resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5ef13-104">Representa a legenda de um gráfico.</span><span class="sxs-lookup"><span data-stu-id="5ef13-104">Represents the legend in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="5ef13-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="5ef13-105">Methods</span></span>

| <span data-ttu-id="5ef13-106">Método</span><span class="sxs-lookup"><span data-stu-id="5ef13-106">Method</span></span>           | <span data-ttu-id="5ef13-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="5ef13-107">Return Type</span></span>    |<span data-ttu-id="5ef13-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="5ef13-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5ef13-109">Get ChartLegend</span><span class="sxs-lookup"><span data-stu-id="5ef13-109">Get ChartLegend</span></span>](../api/chartlegend-get.md) | [<span data-ttu-id="5ef13-110">ChartLegend</span><span class="sxs-lookup"><span data-stu-id="5ef13-110">ChartLegend</span></span>](chartlegend.md) |<span data-ttu-id="5ef13-111">Leia as propriedades e os relacionamentos do objeto chartLegend.</span><span class="sxs-lookup"><span data-stu-id="5ef13-111">Read properties and relationships of chartLegend object.</span></span>|
|[<span data-ttu-id="5ef13-112">Update</span><span class="sxs-lookup"><span data-stu-id="5ef13-112">Update</span></span>](../api/chartlegend-update.md) | [<span data-ttu-id="5ef13-113">ChartLegend</span><span class="sxs-lookup"><span data-stu-id="5ef13-113">ChartLegend</span></span>](chartlegend.md) |<span data-ttu-id="5ef13-114">Atualize o objeto ChartLegend.</span><span class="sxs-lookup"><span data-stu-id="5ef13-114">Update ChartLegend object.</span></span> |

## <a name="properties"></a><span data-ttu-id="5ef13-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5ef13-115">Properties</span></span>
| <span data-ttu-id="5ef13-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5ef13-116">Property</span></span>     | <span data-ttu-id="5ef13-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="5ef13-117">Type</span></span>   |<span data-ttu-id="5ef13-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="5ef13-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5ef13-119">overlay</span><span class="sxs-lookup"><span data-stu-id="5ef13-119">overlay</span></span>|<span data-ttu-id="5ef13-120">booliano</span><span class="sxs-lookup"><span data-stu-id="5ef13-120">boolean</span></span>|<span data-ttu-id="5ef13-121">Valor booliano para determinar se a legenda do gráfico deve se sobrepor ao corpo principal do gráfico.</span><span class="sxs-lookup"><span data-stu-id="5ef13-121">Boolean value for whether the chart legend should overlap with the main body of the chart.</span></span>|
|<span data-ttu-id="5ef13-122">position</span><span class="sxs-lookup"><span data-stu-id="5ef13-122">position</span></span>|<span data-ttu-id="5ef13-123">string</span><span class="sxs-lookup"><span data-stu-id="5ef13-123">string</span></span>|<span data-ttu-id="5ef13-p101">Representa a posição da legenda no gráfico. Os valores possíveis são: `Top`, `Bottom`, `Left`, `Right`, `Corner` e `Custom`.</span><span class="sxs-lookup"><span data-stu-id="5ef13-p101">Represents the position of the legend on the chart. Possible values are: `Top`, `Bottom`, `Left`, `Right`, `Corner`, `Custom`.</span></span>|
|<span data-ttu-id="5ef13-126">visible</span><span class="sxs-lookup"><span data-stu-id="5ef13-126">visible</span></span>|<span data-ttu-id="5ef13-127">booliano</span><span class="sxs-lookup"><span data-stu-id="5ef13-127">boolean</span></span>|<span data-ttu-id="5ef13-128">Um valor booliano que representa a visibilidade de um objeto ChartLegend.</span><span class="sxs-lookup"><span data-stu-id="5ef13-128">A boolean value the represents the visibility of a ChartLegend object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5ef13-129">Relações</span><span class="sxs-lookup"><span data-stu-id="5ef13-129">Relationships</span></span>
| <span data-ttu-id="5ef13-130">Relação</span><span class="sxs-lookup"><span data-stu-id="5ef13-130">Relationship</span></span> | <span data-ttu-id="5ef13-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="5ef13-131">Type</span></span>   |<span data-ttu-id="5ef13-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="5ef13-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5ef13-133">format</span><span class="sxs-lookup"><span data-stu-id="5ef13-133">format</span></span>|[<span data-ttu-id="5ef13-134">ChartLegendFormat</span><span class="sxs-lookup"><span data-stu-id="5ef13-134">ChartLegendFormat</span></span>](chartlegendformat.md)|<span data-ttu-id="5ef13-p102">Representa a formatação de uma legenda de gráfico, que inclui a formatação de fonte e de preenchimento. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5ef13-p102">Represents the formatting of a chart legend, which includes fill and font formatting. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5ef13-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5ef13-137">JSON representation</span></span>

<span data-ttu-id="5ef13-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5ef13-138">Here is a JSON representation of the resource.</span></span>

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
