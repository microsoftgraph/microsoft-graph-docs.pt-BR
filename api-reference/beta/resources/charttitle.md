---
title: Tipo de recurso ChartTitle
description: Representa um objeto de título de gráfico de um gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: a71aed2da93c2121492f1eb29826470b797768ed
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643311"
---
# <a name="charttitle-resource-type"></a><span data-ttu-id="b0306-103">Tipo de recurso ChartTitle</span><span class="sxs-lookup"><span data-stu-id="b0306-103">ChartTitle resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b0306-104">Representa um objeto de título de gráfico de um gráfico.</span><span class="sxs-lookup"><span data-stu-id="b0306-104">Represents a chart title object of a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="b0306-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="b0306-105">Methods</span></span>

| <span data-ttu-id="b0306-106">Método</span><span class="sxs-lookup"><span data-stu-id="b0306-106">Method</span></span>           | <span data-ttu-id="b0306-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b0306-107">Return Type</span></span>    |<span data-ttu-id="b0306-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="b0306-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b0306-109">Get ChartTitle</span><span class="sxs-lookup"><span data-stu-id="b0306-109">Get ChartTitle</span></span>](../api/charttitle-get.md) | [<span data-ttu-id="b0306-110">ChartTitle</span><span class="sxs-lookup"><span data-stu-id="b0306-110">ChartTitle</span></span>](charttitle.md) |<span data-ttu-id="b0306-111">Leia as propriedades e os relacionamentos do objeto chartTitle.</span><span class="sxs-lookup"><span data-stu-id="b0306-111">Read properties and relationships of chartTitle object.</span></span>|
|[<span data-ttu-id="b0306-112">Update</span><span class="sxs-lookup"><span data-stu-id="b0306-112">Update</span></span>](../api/charttitle-update.md) | [<span data-ttu-id="b0306-113">ChartTitle</span><span class="sxs-lookup"><span data-stu-id="b0306-113">ChartTitle</span></span>](charttitle.md)    |<span data-ttu-id="b0306-114">Atualize o objeto ChartTitle.</span><span class="sxs-lookup"><span data-stu-id="b0306-114">Update ChartTitle object.</span></span> |

## <a name="properties"></a><span data-ttu-id="b0306-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b0306-115">Properties</span></span>
| <span data-ttu-id="b0306-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b0306-116">Property</span></span>     | <span data-ttu-id="b0306-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="b0306-117">Type</span></span>   |<span data-ttu-id="b0306-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="b0306-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b0306-119">overlay</span><span class="sxs-lookup"><span data-stu-id="b0306-119">overlay</span></span>|<span data-ttu-id="b0306-120">booliano</span><span class="sxs-lookup"><span data-stu-id="b0306-120">boolean</span></span>|<span data-ttu-id="b0306-121">Valor booliano que determina se o título do gráfico deve se sobrepor ao gráfico ou não.</span><span class="sxs-lookup"><span data-stu-id="b0306-121">Boolean value representing if the chart title will overlay the chart or not.</span></span>|
|<span data-ttu-id="b0306-122">texto</span><span class="sxs-lookup"><span data-stu-id="b0306-122">text</span></span>|<span data-ttu-id="b0306-123">string</span><span class="sxs-lookup"><span data-stu-id="b0306-123">string</span></span>|<span data-ttu-id="b0306-124">Representa o texto do título de um gráfico.</span><span class="sxs-lookup"><span data-stu-id="b0306-124">Represents the title text of a chart.</span></span>|
|<span data-ttu-id="b0306-125">visible</span><span class="sxs-lookup"><span data-stu-id="b0306-125">visible</span></span>|<span data-ttu-id="b0306-126">booliano</span><span class="sxs-lookup"><span data-stu-id="b0306-126">boolean</span></span>|<span data-ttu-id="b0306-127">Um valor booliano que representa a visibilidade de um objeto de título de gráfico.</span><span class="sxs-lookup"><span data-stu-id="b0306-127">A boolean value the represents the visibility of a chart title object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b0306-128">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="b0306-128">Relationships</span></span>
| <span data-ttu-id="b0306-129">Relação</span><span class="sxs-lookup"><span data-stu-id="b0306-129">Relationship</span></span> | <span data-ttu-id="b0306-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="b0306-130">Type</span></span>   |<span data-ttu-id="b0306-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="b0306-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b0306-132">formato</span><span class="sxs-lookup"><span data-stu-id="b0306-132">format</span></span>|[<span data-ttu-id="b0306-133">ChartTitleFormat</span><span class="sxs-lookup"><span data-stu-id="b0306-133">ChartTitleFormat</span></span>](charttitleformat.md)|<span data-ttu-id="b0306-p101">Representa a formatação de um título do gráfico, que inclui a formatação de fonte e de preenchimento. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b0306-p101">Represents the formatting of a chart title, which includes fill and font formatting. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b0306-136">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b0306-136">JSON representation</span></span>

<span data-ttu-id="b0306-137">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b0306-137">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartTitle"
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
<!--
{
  "type": "#page.annotation",
  "description": "ChartTitle resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/charttitle.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
