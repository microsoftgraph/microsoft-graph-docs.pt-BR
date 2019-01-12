---
title: Tipo de recurso ChartTitle
description: Representa um objeto de título de gráfico de um gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: f6c843e24839b51da67bda5ed3484a32c868ae54
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27986912"
---
# <a name="charttitle-resource-type"></a><span data-ttu-id="1921b-103">Tipo de recurso ChartTitle</span><span class="sxs-lookup"><span data-stu-id="1921b-103">ChartTitle resource type</span></span>

<span data-ttu-id="1921b-104">Representa um objeto de título de gráfico de um gráfico.</span><span class="sxs-lookup"><span data-stu-id="1921b-104">Represents a chart title object of a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="1921b-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="1921b-105">Methods</span></span>

| <span data-ttu-id="1921b-106">Método</span><span class="sxs-lookup"><span data-stu-id="1921b-106">Method</span></span>           | <span data-ttu-id="1921b-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="1921b-107">Return Type</span></span>    |<span data-ttu-id="1921b-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="1921b-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1921b-109">Get ChartTitle</span><span class="sxs-lookup"><span data-stu-id="1921b-109">Get ChartTitle</span></span>](../api/charttitle-get.md) | [<span data-ttu-id="1921b-110">WorkbookChartTitle</span><span class="sxs-lookup"><span data-stu-id="1921b-110">WorkbookChartTitle</span></span>](charttitle.md) |<span data-ttu-id="1921b-111">Leia as propriedades e os relacionamentos do objeto chartTitle.</span><span class="sxs-lookup"><span data-stu-id="1921b-111">Read properties and relationships of chartTitle object.</span></span>|
|[<span data-ttu-id="1921b-112">Update</span><span class="sxs-lookup"><span data-stu-id="1921b-112">Update</span></span>](../api/charttitle-update.md) | [<span data-ttu-id="1921b-113">WorkbookChartTitle</span><span class="sxs-lookup"><span data-stu-id="1921b-113">WorkbookChartTitle</span></span>](charttitle.md)    |<span data-ttu-id="1921b-114">Atualize o objeto ChartTitle.</span><span class="sxs-lookup"><span data-stu-id="1921b-114">Update ChartTitle object.</span></span> |

## <a name="properties"></a><span data-ttu-id="1921b-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1921b-115">Properties</span></span>
| <span data-ttu-id="1921b-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1921b-116">Property</span></span>     | <span data-ttu-id="1921b-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="1921b-117">Type</span></span>   |<span data-ttu-id="1921b-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="1921b-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1921b-119">overlay</span><span class="sxs-lookup"><span data-stu-id="1921b-119">overlay</span></span>|<span data-ttu-id="1921b-120">booliano</span><span class="sxs-lookup"><span data-stu-id="1921b-120">boolean</span></span>|<span data-ttu-id="1921b-121">Valor booliano que determina se o título do gráfico deve se sobrepor ao gráfico ou não.</span><span class="sxs-lookup"><span data-stu-id="1921b-121">Boolean value representing if the chart title will overlay the chart or not.</span></span>|
|<span data-ttu-id="1921b-122">texto</span><span class="sxs-lookup"><span data-stu-id="1921b-122">text</span></span>|<span data-ttu-id="1921b-123">string</span><span class="sxs-lookup"><span data-stu-id="1921b-123">string</span></span>|<span data-ttu-id="1921b-124">Representa o texto do título de um gráfico.</span><span class="sxs-lookup"><span data-stu-id="1921b-124">Represents the title text of a chart.</span></span>|
|<span data-ttu-id="1921b-125">visible</span><span class="sxs-lookup"><span data-stu-id="1921b-125">visible</span></span>|<span data-ttu-id="1921b-126">booliano</span><span class="sxs-lookup"><span data-stu-id="1921b-126">boolean</span></span>|<span data-ttu-id="1921b-127">Um valor booliano que representa a visibilidade de um objeto de título de gráfico.</span><span class="sxs-lookup"><span data-stu-id="1921b-127">A boolean value the represents the visibility of a chart title object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1921b-128">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="1921b-128">Relationships</span></span>
| <span data-ttu-id="1921b-129">Relação</span><span class="sxs-lookup"><span data-stu-id="1921b-129">Relationship</span></span> | <span data-ttu-id="1921b-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="1921b-130">Type</span></span>   |<span data-ttu-id="1921b-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="1921b-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1921b-132">formato</span><span class="sxs-lookup"><span data-stu-id="1921b-132">format</span></span>|[<span data-ttu-id="1921b-133">WorkbookChartTitleFormat</span><span class="sxs-lookup"><span data-stu-id="1921b-133">WorkbookChartTitleFormat</span></span>](charttitleformat.md)|<span data-ttu-id="1921b-p101">Representa a formatação de um título do gráfico, que inclui a formatação de fonte e de preenchimento. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1921b-p101">Represents the formatting of a chart title, which includes fill and font formatting. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1921b-136">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1921b-136">JSON representation</span></span>

<span data-ttu-id="1921b-137">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1921b-137">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookChartTitle"
}-->

```json
{
  "overlay": true,
  "text": "string",
  "visible": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartTitle resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
