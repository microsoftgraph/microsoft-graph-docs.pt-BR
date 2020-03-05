---
title: tipo de recurso workbookChartLineFormat
description: Encapsula as opções de formatação dos elementos de linha.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 6900b961608ff29c503dc355dfb8876d3e273feb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519292"
---
# <a name="workbookchartlineformat-resource-type"></a><span data-ttu-id="e1a74-103">tipo de recurso workbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="e1a74-103">workbookChartLineFormat resource type</span></span>

<span data-ttu-id="e1a74-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="e1a74-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e1a74-105">Encapsula as opções de formatação dos elementos de linha.</span><span class="sxs-lookup"><span data-stu-id="e1a74-105">Enapsulates the formatting options for line elements.</span></span>


## <a name="methods"></a><span data-ttu-id="e1a74-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="e1a74-106">Methods</span></span>

| <span data-ttu-id="e1a74-107">Método</span><span class="sxs-lookup"><span data-stu-id="e1a74-107">Method</span></span>           | <span data-ttu-id="e1a74-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e1a74-108">Return Type</span></span>    |<span data-ttu-id="e1a74-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="e1a74-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e1a74-110">Obter workbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="e1a74-110">Get workbookChartLineFormat</span></span>](../api/chartlineformat-get.md) | [<span data-ttu-id="e1a74-111">workbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="e1a74-111">workbookChartLineFormat</span></span>](workbookchartlineformat.md) |<span data-ttu-id="e1a74-112">Leia as propriedades e os relacionamentos do objeto chartLineFormat.</span><span class="sxs-lookup"><span data-stu-id="e1a74-112">Read properties and relationships of chartLineFormat object.</span></span>|
|[<span data-ttu-id="e1a74-113">Update</span><span class="sxs-lookup"><span data-stu-id="e1a74-113">Update</span></span>](../api/chartlineformat-update.md) | [<span data-ttu-id="e1a74-114">workbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="e1a74-114">workbookChartLineFormat</span></span>](workbookchartlineformat.md) |<span data-ttu-id="e1a74-115">Atualize o objeto ChartLineFormat.</span><span class="sxs-lookup"><span data-stu-id="e1a74-115">Update ChartLineFormat object.</span></span> |
|[<span data-ttu-id="e1a74-116">Clear</span><span class="sxs-lookup"><span data-stu-id="e1a74-116">Clear</span></span>](../api/chartlineformat-clear.md)|<span data-ttu-id="e1a74-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e1a74-117">None</span></span>|<span data-ttu-id="e1a74-118">Limpe a formatação da linha de um elemento do gráfico.</span><span class="sxs-lookup"><span data-stu-id="e1a74-118">Clear the line format of a chart element.</span></span>|

## <a name="properties"></a><span data-ttu-id="e1a74-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e1a74-119">Properties</span></span>
| <span data-ttu-id="e1a74-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e1a74-120">Property</span></span>     | <span data-ttu-id="e1a74-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="e1a74-121">Type</span></span>   |<span data-ttu-id="e1a74-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="e1a74-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e1a74-123">color</span><span class="sxs-lookup"><span data-stu-id="e1a74-123">color</span></span>|<span data-ttu-id="e1a74-124">string</span><span class="sxs-lookup"><span data-stu-id="e1a74-124">string</span></span>|<span data-ttu-id="e1a74-125">Código de cores HTML que representa a cor das linhas no gráfico.</span><span class="sxs-lookup"><span data-stu-id="e1a74-125">HTML color code representing the color of lines in the chart.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e1a74-126">Relações</span><span class="sxs-lookup"><span data-stu-id="e1a74-126">Relationships</span></span>
<span data-ttu-id="e1a74-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e1a74-127">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="e1a74-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e1a74-128">JSON representation</span></span>

<span data-ttu-id="e1a74-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e1a74-129">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "workbookChartLineFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
