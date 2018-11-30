---
title: Tipo de recurso ChartLineFormat
description: Abrange as opções de formatação dos elementos de linha.
ms.openlocfilehash: 6e43818bc55972585deff5aa2add1d513f031360
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27004263"
---
# <a name="chartlineformat-resource-type"></a><span data-ttu-id="7e451-103">Tipo de recurso ChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="7e451-103">ChartLineFormat resource type</span></span>

<span data-ttu-id="7e451-104">Abrange as opções de formatação dos elementos de linha.</span><span class="sxs-lookup"><span data-stu-id="7e451-104">Enapsulates the formatting options for line elements.</span></span>


## <a name="methods"></a><span data-ttu-id="7e451-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="7e451-105">Methods</span></span>

| <span data-ttu-id="7e451-106">Método</span><span class="sxs-lookup"><span data-stu-id="7e451-106">Method</span></span>           | <span data-ttu-id="7e451-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="7e451-107">Return Type</span></span>    |<span data-ttu-id="7e451-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="7e451-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7e451-109">Get ChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="7e451-109">Get ChartLineFormat</span></span>](../api/chartlineformat-get.md) | [<span data-ttu-id="7e451-110">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="7e451-110">WorkbookChartLineFormat</span></span>](chartlineformat.md) |<span data-ttu-id="7e451-111">Leia as propriedades e os relacionamentos do objeto chartLineFormat.</span><span class="sxs-lookup"><span data-stu-id="7e451-111">Read properties and relationships of chartLineFormat object.</span></span>|
|[<span data-ttu-id="7e451-112">Update</span><span class="sxs-lookup"><span data-stu-id="7e451-112">Update</span></span>](../api/chartlineformat-update.md) | [<span data-ttu-id="7e451-113">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="7e451-113">WorkbookChartLineFormat</span></span>](chartlineformat.md) |<span data-ttu-id="7e451-114">Atualize o objeto ChartLineFormat.</span><span class="sxs-lookup"><span data-stu-id="7e451-114">Update ChartLineFormat object.</span></span> |
|[<span data-ttu-id="7e451-115">Clear</span><span class="sxs-lookup"><span data-stu-id="7e451-115">Clear</span></span>](../api/chartlineformat-clear.md)|<span data-ttu-id="7e451-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7e451-116">None</span></span>|<span data-ttu-id="7e451-117">Limpe a formatação da linha de um elemento do gráfico.</span><span class="sxs-lookup"><span data-stu-id="7e451-117">Clear the line format of a chart element.</span></span>|

## <a name="properties"></a><span data-ttu-id="7e451-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7e451-118">Properties</span></span>
| <span data-ttu-id="7e451-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7e451-119">Property</span></span>     | <span data-ttu-id="7e451-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="7e451-120">Type</span></span>   |<span data-ttu-id="7e451-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="7e451-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7e451-122">color</span><span class="sxs-lookup"><span data-stu-id="7e451-122">color</span></span>|<span data-ttu-id="7e451-123">string</span><span class="sxs-lookup"><span data-stu-id="7e451-123">string</span></span>|<span data-ttu-id="7e451-124">Código de cor HTML que representa a cor das linhas no gráfico.</span><span class="sxs-lookup"><span data-stu-id="7e451-124">HTML color code representing the color of lines in the chart.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7e451-125">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="7e451-125">Relationships</span></span>
<span data-ttu-id="7e451-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7e451-126">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="7e451-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7e451-127">JSON representation</span></span>

<span data-ttu-id="7e451-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7e451-128">Here is a JSON representation of the resource.</span></span>

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