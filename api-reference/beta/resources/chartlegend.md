---
title: Tipo de recurso ChartLegend
description: Representa a legenda de um gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: c76fd21700616ec6c353644de93bddd0a47ac7dd
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27980875"
---
# <a name="chartlegend-resource-type"></a><span data-ttu-id="ce286-103">Tipo de recurso ChartLegend</span><span class="sxs-lookup"><span data-stu-id="ce286-103">ChartLegend resource type</span></span>

> <span data-ttu-id="ce286-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ce286-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ce286-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ce286-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ce286-106">Representa a legenda de um gráfico.</span><span class="sxs-lookup"><span data-stu-id="ce286-106">Represents the legend in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="ce286-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="ce286-107">Methods</span></span>

| <span data-ttu-id="ce286-108">Método</span><span class="sxs-lookup"><span data-stu-id="ce286-108">Method</span></span>           | <span data-ttu-id="ce286-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ce286-109">Return Type</span></span>    |<span data-ttu-id="ce286-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="ce286-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ce286-111">Get ChartLegend</span><span class="sxs-lookup"><span data-stu-id="ce286-111">Get ChartLegend</span></span>](../api/chartlegend-get.md) | [<span data-ttu-id="ce286-112">ChartLegend</span><span class="sxs-lookup"><span data-stu-id="ce286-112">ChartLegend</span></span>](chartlegend.md) |<span data-ttu-id="ce286-113">Leia as propriedades e os relacionamentos do objeto chartLegend.</span><span class="sxs-lookup"><span data-stu-id="ce286-113">Read properties and relationships of chartLegend object.</span></span>|
|[<span data-ttu-id="ce286-114">Update</span><span class="sxs-lookup"><span data-stu-id="ce286-114">Update</span></span>](../api/chartlegend-update.md) | [<span data-ttu-id="ce286-115">ChartLegend</span><span class="sxs-lookup"><span data-stu-id="ce286-115">ChartLegend</span></span>](chartlegend.md) |<span data-ttu-id="ce286-116">Atualize o objeto ChartLegend.</span><span class="sxs-lookup"><span data-stu-id="ce286-116">Update ChartLegend object.</span></span> |

## <a name="properties"></a><span data-ttu-id="ce286-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ce286-117">Properties</span></span>
| <span data-ttu-id="ce286-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ce286-118">Property</span></span>     | <span data-ttu-id="ce286-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="ce286-119">Type</span></span>   |<span data-ttu-id="ce286-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="ce286-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ce286-121">overlay</span><span class="sxs-lookup"><span data-stu-id="ce286-121">overlay</span></span>|<span data-ttu-id="ce286-122">booliano</span><span class="sxs-lookup"><span data-stu-id="ce286-122">boolean</span></span>|<span data-ttu-id="ce286-123">Valor booliano para determinar se a legenda do gráfico deve se sobrepor ao corpo principal do gráfico.</span><span class="sxs-lookup"><span data-stu-id="ce286-123">Boolean value for whether the chart legend should overlap with the main body of the chart.</span></span>|
|<span data-ttu-id="ce286-124">position</span><span class="sxs-lookup"><span data-stu-id="ce286-124">position</span></span>|<span data-ttu-id="ce286-125">string</span><span class="sxs-lookup"><span data-stu-id="ce286-125">string</span></span>|<span data-ttu-id="ce286-p102">Representa a posição da legenda no gráfico. Os valores possíveis são: `Top`, `Bottom`, `Left`, `Right`, `Corner` e `Custom`.</span><span class="sxs-lookup"><span data-stu-id="ce286-p102">Represents the position of the legend on the chart. Possible values are: `Top`, `Bottom`, `Left`, `Right`, `Corner`, `Custom`.</span></span>|
|<span data-ttu-id="ce286-128">visible</span><span class="sxs-lookup"><span data-stu-id="ce286-128">visible</span></span>|<span data-ttu-id="ce286-129">booliano</span><span class="sxs-lookup"><span data-stu-id="ce286-129">boolean</span></span>|<span data-ttu-id="ce286-130">Um valor booliano que representa a visibilidade de um objeto ChartLegend.</span><span class="sxs-lookup"><span data-stu-id="ce286-130">A boolean value the represents the visibility of a ChartLegend object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ce286-131">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="ce286-131">Relationships</span></span>
| <span data-ttu-id="ce286-132">Relação</span><span class="sxs-lookup"><span data-stu-id="ce286-132">Relationship</span></span> | <span data-ttu-id="ce286-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="ce286-133">Type</span></span>   |<span data-ttu-id="ce286-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="ce286-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ce286-135">formato</span><span class="sxs-lookup"><span data-stu-id="ce286-135">format</span></span>|[<span data-ttu-id="ce286-136">ChartLegendFormat</span><span class="sxs-lookup"><span data-stu-id="ce286-136">ChartLegendFormat</span></span>](chartlegendformat.md)|<span data-ttu-id="ce286-p103">Representa a formatação de uma legenda de gráfico, que inclui a formatação de fonte e de preenchimento. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ce286-p103">Represents the formatting of a chart legend, which includes fill and font formatting. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ce286-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ce286-139">JSON representation</span></span>

<span data-ttu-id="ce286-140">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ce286-140">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "ChartLegend resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
