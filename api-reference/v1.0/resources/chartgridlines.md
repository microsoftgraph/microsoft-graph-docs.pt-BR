---
title: Tipo de recurso ChartGridlines
description: Representa linhas de grade principais ou secundárias em um eixo do gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: b37bbc2b746d3dc2de4b55fa363b7b67f30f7191
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48069180"
---
# <a name="chartgridlines-resource-type"></a><span data-ttu-id="92f8e-103">Tipo de recurso ChartGridlines</span><span class="sxs-lookup"><span data-stu-id="92f8e-103">ChartGridlines resource type</span></span>

<span data-ttu-id="92f8e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="92f8e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="92f8e-105">Representa linhas de grade principais ou secundárias em um eixo do gráfico.</span><span class="sxs-lookup"><span data-stu-id="92f8e-105">Represents major or minor gridlines on a chart axis.</span></span>


## <a name="methods"></a><span data-ttu-id="92f8e-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="92f8e-106">Methods</span></span>

| <span data-ttu-id="92f8e-107">Método</span><span class="sxs-lookup"><span data-stu-id="92f8e-107">Method</span></span>           | <span data-ttu-id="92f8e-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="92f8e-108">Return Type</span></span>    |<span data-ttu-id="92f8e-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="92f8e-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="92f8e-110">Get ChartGridlines</span><span class="sxs-lookup"><span data-stu-id="92f8e-110">Get ChartGridlines</span></span>](../api/chartgridlines-get.md) | [<span data-ttu-id="92f8e-111">WorkbookChartGridlines</span><span class="sxs-lookup"><span data-stu-id="92f8e-111">WorkbookChartGridlines</span></span>](chartgridlines.md) |<span data-ttu-id="92f8e-112">Leia as propriedades e os relacionamentos do objeto chartGridlines.</span><span class="sxs-lookup"><span data-stu-id="92f8e-112">Read properties and relationships of chartGridlines object.</span></span>|
|[<span data-ttu-id="92f8e-113">Update</span><span class="sxs-lookup"><span data-stu-id="92f8e-113">Update</span></span>](../api/chartgridlines-update.md) | [<span data-ttu-id="92f8e-114">WorkbookChartGridlines</span><span class="sxs-lookup"><span data-stu-id="92f8e-114">WorkbookChartGridlines</span></span>](chartgridlines.md)    |<span data-ttu-id="92f8e-115">Atualize o objeto ChartGridlines.</span><span class="sxs-lookup"><span data-stu-id="92f8e-115">Update ChartGridlines object.</span></span> |

## <a name="properties"></a><span data-ttu-id="92f8e-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="92f8e-116">Properties</span></span>
| <span data-ttu-id="92f8e-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="92f8e-117">Property</span></span>     | <span data-ttu-id="92f8e-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="92f8e-118">Type</span></span>   |<span data-ttu-id="92f8e-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="92f8e-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="92f8e-120">visible</span><span class="sxs-lookup"><span data-stu-id="92f8e-120">visible</span></span>|<span data-ttu-id="92f8e-121">booliano</span><span class="sxs-lookup"><span data-stu-id="92f8e-121">boolean</span></span>|<span data-ttu-id="92f8e-122">Valor booliano que determina se as linhas de grade do eixo ficam visíveis ou não.</span><span class="sxs-lookup"><span data-stu-id="92f8e-122">Boolean value representing if the axis gridlines are visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="92f8e-123">Relações</span><span class="sxs-lookup"><span data-stu-id="92f8e-123">Relationships</span></span>
| <span data-ttu-id="92f8e-124">Relação</span><span class="sxs-lookup"><span data-stu-id="92f8e-124">Relationship</span></span> | <span data-ttu-id="92f8e-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="92f8e-125">Type</span></span>   |<span data-ttu-id="92f8e-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="92f8e-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="92f8e-127">formato</span><span class="sxs-lookup"><span data-stu-id="92f8e-127">format</span></span>|[<span data-ttu-id="92f8e-128">WorkbookChartGridlinesFormat</span><span class="sxs-lookup"><span data-stu-id="92f8e-128">WorkbookChartGridlinesFormat</span></span>](chartgridlinesformat.md)|<span data-ttu-id="92f8e-129">Representa a formatação de linhas de grade do gráfico.</span><span class="sxs-lookup"><span data-stu-id="92f8e-129">Represents the formatting of chart gridlines.</span></span> <span data-ttu-id="92f8e-130">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="92f8e-130">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="92f8e-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="92f8e-131">JSON representation</span></span>

<span data-ttu-id="92f8e-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="92f8e-132">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookChartGridlines"
}-->

```json
{
  "visible": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartGridlines resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

