---
title: Tipo de recurso ChartLineFormat
description: Abrange as opções de formatação dos elementos de linha.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 70e4e3d5c88fccd2a34c3fa17d5fe4bf5dcf1e5b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27805737"
---
# <a name="chartlineformat-resource-type"></a><span data-ttu-id="42c13-103">Tipo de recurso ChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="42c13-103">ChartLineFormat resource type</span></span>

<span data-ttu-id="42c13-104">Abrange as opções de formatação dos elementos de linha.</span><span class="sxs-lookup"><span data-stu-id="42c13-104">Enapsulates the formatting options for line elements.</span></span>


## <a name="methods"></a><span data-ttu-id="42c13-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="42c13-105">Methods</span></span>

| <span data-ttu-id="42c13-106">Método</span><span class="sxs-lookup"><span data-stu-id="42c13-106">Method</span></span>           | <span data-ttu-id="42c13-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="42c13-107">Return Type</span></span>    |<span data-ttu-id="42c13-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="42c13-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="42c13-109">Get ChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="42c13-109">Get ChartLineFormat</span></span>](../api/chartlineformat-get.md) | [<span data-ttu-id="42c13-110">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="42c13-110">WorkbookChartLineFormat</span></span>](chartlineformat.md) |<span data-ttu-id="42c13-111">Leia as propriedades e os relacionamentos do objeto chartLineFormat.</span><span class="sxs-lookup"><span data-stu-id="42c13-111">Read properties and relationships of chartLineFormat object.</span></span>|
|[<span data-ttu-id="42c13-112">Update</span><span class="sxs-lookup"><span data-stu-id="42c13-112">Update</span></span>](../api/chartlineformat-update.md) | [<span data-ttu-id="42c13-113">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="42c13-113">WorkbookChartLineFormat</span></span>](chartlineformat.md) |<span data-ttu-id="42c13-114">Atualize o objeto ChartLineFormat.</span><span class="sxs-lookup"><span data-stu-id="42c13-114">Update ChartLineFormat object.</span></span> |
|[<span data-ttu-id="42c13-115">Clear</span><span class="sxs-lookup"><span data-stu-id="42c13-115">Clear</span></span>](../api/chartlineformat-clear.md)|<span data-ttu-id="42c13-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="42c13-116">None</span></span>|<span data-ttu-id="42c13-117">Limpe a formatação da linha de um elemento do gráfico.</span><span class="sxs-lookup"><span data-stu-id="42c13-117">Clear the line format of a chart element.</span></span>|

## <a name="properties"></a><span data-ttu-id="42c13-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="42c13-118">Properties</span></span>
| <span data-ttu-id="42c13-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="42c13-119">Property</span></span>     | <span data-ttu-id="42c13-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="42c13-120">Type</span></span>   |<span data-ttu-id="42c13-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="42c13-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="42c13-122">color</span><span class="sxs-lookup"><span data-stu-id="42c13-122">color</span></span>|<span data-ttu-id="42c13-123">string</span><span class="sxs-lookup"><span data-stu-id="42c13-123">string</span></span>|<span data-ttu-id="42c13-124">Código de cor HTML que representa a cor das linhas no gráfico.</span><span class="sxs-lookup"><span data-stu-id="42c13-124">HTML color code representing the color of lines in the chart.</span></span>|

## <a name="relationships"></a><span data-ttu-id="42c13-125">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="42c13-125">Relationships</span></span>
<span data-ttu-id="42c13-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="42c13-126">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="42c13-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="42c13-127">JSON representation</span></span>

<span data-ttu-id="42c13-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="42c13-128">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.workbookChartLineFormat"
}-->

```json
{
  "color": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartLineFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
