---
title: Tipo de recurso ChartLineFormat
description: Abrange as opções de formatação dos elementos de linha.
author: lumine2008
ms.openlocfilehash: 1940b5dfe09c2895fbf1b8eb6bf4e5227194367c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27357299"
---
# <a name="chartlineformat-resource-type"></a><span data-ttu-id="ad3b1-103">Tipo de recurso ChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="ad3b1-103">ChartLineFormat resource type</span></span>

<span data-ttu-id="ad3b1-104">Abrange as opções de formatação dos elementos de linha.</span><span class="sxs-lookup"><span data-stu-id="ad3b1-104">Enapsulates the formatting options for line elements.</span></span>


## <a name="methods"></a><span data-ttu-id="ad3b1-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="ad3b1-105">Methods</span></span>

| <span data-ttu-id="ad3b1-106">Método</span><span class="sxs-lookup"><span data-stu-id="ad3b1-106">Method</span></span>           | <span data-ttu-id="ad3b1-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ad3b1-107">Return Type</span></span>    |<span data-ttu-id="ad3b1-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="ad3b1-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ad3b1-109">Get ChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="ad3b1-109">Get ChartLineFormat</span></span>](../api/chartlineformat-get.md) | [<span data-ttu-id="ad3b1-110">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="ad3b1-110">WorkbookChartLineFormat</span></span>](chartlineformat.md) |<span data-ttu-id="ad3b1-111">Leia as propriedades e os relacionamentos do objeto chartLineFormat.</span><span class="sxs-lookup"><span data-stu-id="ad3b1-111">Read properties and relationships of chartLineFormat object.</span></span>|
|[<span data-ttu-id="ad3b1-112">Update</span><span class="sxs-lookup"><span data-stu-id="ad3b1-112">Update</span></span>](../api/chartlineformat-update.md) | [<span data-ttu-id="ad3b1-113">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="ad3b1-113">WorkbookChartLineFormat</span></span>](chartlineformat.md) |<span data-ttu-id="ad3b1-114">Atualize o objeto ChartLineFormat.</span><span class="sxs-lookup"><span data-stu-id="ad3b1-114">Update ChartLineFormat object.</span></span> |
|[<span data-ttu-id="ad3b1-115">Clear</span><span class="sxs-lookup"><span data-stu-id="ad3b1-115">Clear</span></span>](../api/chartlineformat-clear.md)|<span data-ttu-id="ad3b1-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ad3b1-116">None</span></span>|<span data-ttu-id="ad3b1-117">Limpe a formatação da linha de um elemento do gráfico.</span><span class="sxs-lookup"><span data-stu-id="ad3b1-117">Clear the line format of a chart element.</span></span>|

## <a name="properties"></a><span data-ttu-id="ad3b1-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ad3b1-118">Properties</span></span>
| <span data-ttu-id="ad3b1-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ad3b1-119">Property</span></span>     | <span data-ttu-id="ad3b1-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="ad3b1-120">Type</span></span>   |<span data-ttu-id="ad3b1-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="ad3b1-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ad3b1-122">color</span><span class="sxs-lookup"><span data-stu-id="ad3b1-122">color</span></span>|<span data-ttu-id="ad3b1-123">string</span><span class="sxs-lookup"><span data-stu-id="ad3b1-123">string</span></span>|<span data-ttu-id="ad3b1-124">Código de cor HTML que representa a cor das linhas no gráfico.</span><span class="sxs-lookup"><span data-stu-id="ad3b1-124">HTML color code representing the color of lines in the chart.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ad3b1-125">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="ad3b1-125">Relationships</span></span>
<span data-ttu-id="ad3b1-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ad3b1-126">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="ad3b1-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ad3b1-127">JSON representation</span></span>

<span data-ttu-id="ad3b1-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ad3b1-128">Here is a JSON representation of the resource.</span></span>

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