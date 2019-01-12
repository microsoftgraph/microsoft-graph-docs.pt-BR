---
title: Tipo de recurso ChartPoint
description: Representa um ponto de uma série do gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 66c58e08063bd9757ad9c174e81f35328dd2722b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912754"
---
# <a name="chartpoint-resource-type"></a><span data-ttu-id="1f449-103">Tipo de recurso ChartPoint</span><span class="sxs-lookup"><span data-stu-id="1f449-103">ChartPoint resource type</span></span>

> <span data-ttu-id="1f449-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="1f449-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1f449-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="1f449-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1f449-106">Representa um ponto de uma série do gráfico.</span><span class="sxs-lookup"><span data-stu-id="1f449-106">Represents a point of a series in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="1f449-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="1f449-107">Methods</span></span>

| <span data-ttu-id="1f449-108">Método</span><span class="sxs-lookup"><span data-stu-id="1f449-108">Method</span></span>           | <span data-ttu-id="1f449-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="1f449-109">Return Type</span></span>    |<span data-ttu-id="1f449-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="1f449-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1f449-111">Get ChartPoint</span><span class="sxs-lookup"><span data-stu-id="1f449-111">Get ChartPoint</span></span>](../api/chartpoint-get.md) | [<span data-ttu-id="1f449-112">ChartPoint</span><span class="sxs-lookup"><span data-stu-id="1f449-112">ChartPoint</span></span>](chartpoint.md) |<span data-ttu-id="1f449-113">Leia as propriedades e os relacionamentos do objeto chartPoint.</span><span class="sxs-lookup"><span data-stu-id="1f449-113">Read properties and relationships of chartPoint object.</span></span>|
|[<span data-ttu-id="1f449-114">List</span><span class="sxs-lookup"><span data-stu-id="1f449-114">List</span></span>](../api/chartpoint-list.md) | <span data-ttu-id="1f449-115">Coleção [ChartPoint](chartpoint.md)</span><span class="sxs-lookup"><span data-stu-id="1f449-115">[ChartPoint](chartpoint.md) collection</span></span> |<span data-ttu-id="1f449-116">Obtenha a coleção de objetos chartPoint.</span><span class="sxs-lookup"><span data-stu-id="1f449-116">Get chartPoint object collection.</span></span> |
|[<span data-ttu-id="1f449-117">Itemat</span><span class="sxs-lookup"><span data-stu-id="1f449-117">Itemat</span></span>](../api/chartpointscollection-itemat.md)|[<span data-ttu-id="1f449-118">ChartPoint</span><span class="sxs-lookup"><span data-stu-id="1f449-118">ChartPoint</span></span>](chartpoint.md)|<span data-ttu-id="1f449-119">Recupera um ponto com base na respectiva posição dentro da série.</span><span class="sxs-lookup"><span data-stu-id="1f449-119">Retrieve a point based on its position within the series.</span></span>|

## <a name="properties"></a><span data-ttu-id="1f449-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1f449-120">Properties</span></span>
| <span data-ttu-id="1f449-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1f449-121">Property</span></span>     | <span data-ttu-id="1f449-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="1f449-122">Type</span></span>   |<span data-ttu-id="1f449-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="1f449-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1f449-124">valor</span><span class="sxs-lookup"><span data-stu-id="1f449-124">value</span></span>|<span data-ttu-id="1f449-125">object</span><span class="sxs-lookup"><span data-stu-id="1f449-125">object</span></span>|<span data-ttu-id="1f449-p102">Retorna o valor de um ponto do gráfico. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1f449-p102">Returns the value of a chart point. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1f449-128">Relações</span><span class="sxs-lookup"><span data-stu-id="1f449-128">Relationships</span></span>
| <span data-ttu-id="1f449-129">Relação</span><span class="sxs-lookup"><span data-stu-id="1f449-129">Relationship</span></span> | <span data-ttu-id="1f449-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="1f449-130">Type</span></span>   |<span data-ttu-id="1f449-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="1f449-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1f449-132">formato</span><span class="sxs-lookup"><span data-stu-id="1f449-132">format</span></span>|[<span data-ttu-id="1f449-133">ChartPointFormat</span><span class="sxs-lookup"><span data-stu-id="1f449-133">ChartPointFormat</span></span>](chartpointformat.md)|<span data-ttu-id="1f449-p103">Encapsula as propriedades de formato de um ponto do gráfico. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1f449-p103">Encapsulates the format properties chart point. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1f449-136">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1f449-136">JSON representation</span></span>

<span data-ttu-id="1f449-137">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1f449-137">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartPoint"
}-->

```json
{
  "value": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartPoint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
