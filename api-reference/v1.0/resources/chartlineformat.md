---
title: Tipo de recurso ChartLineFormat
description: Encapsula as opções de formatação dos elementos de linha.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 505e6d88e0c1b19ea33d475b6d8edf3485e29cea
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032960"
---
# <a name="chartlineformat-resource-type"></a><span data-ttu-id="daeee-103">Tipo de recurso ChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="daeee-103">ChartLineFormat resource type</span></span>

<span data-ttu-id="daeee-104">Encapsula as opções de formatação dos elementos de linha.</span><span class="sxs-lookup"><span data-stu-id="daeee-104">Enapsulates the formatting options for line elements.</span></span>


## <a name="methods"></a><span data-ttu-id="daeee-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="daeee-105">Methods</span></span>

| <span data-ttu-id="daeee-106">Método</span><span class="sxs-lookup"><span data-stu-id="daeee-106">Method</span></span>           | <span data-ttu-id="daeee-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="daeee-107">Return Type</span></span>    |<span data-ttu-id="daeee-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="daeee-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="daeee-109">Get ChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="daeee-109">Get ChartLineFormat</span></span>](../api/chartlineformat-get.md) | [<span data-ttu-id="daeee-110">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="daeee-110">WorkbookChartLineFormat</span></span>](chartlineformat.md) |<span data-ttu-id="daeee-111">Leia as propriedades e os relacionamentos do objeto chartLineFormat.</span><span class="sxs-lookup"><span data-stu-id="daeee-111">Read properties and relationships of chartLineFormat object.</span></span>|
|[<span data-ttu-id="daeee-112">Update</span><span class="sxs-lookup"><span data-stu-id="daeee-112">Update</span></span>](../api/chartlineformat-update.md) | [<span data-ttu-id="daeee-113">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="daeee-113">WorkbookChartLineFormat</span></span>](chartlineformat.md) |<span data-ttu-id="daeee-114">Atualize o objeto ChartLineFormat.</span><span class="sxs-lookup"><span data-stu-id="daeee-114">Update ChartLineFormat object.</span></span> |
|[<span data-ttu-id="daeee-115">Clear</span><span class="sxs-lookup"><span data-stu-id="daeee-115">Clear</span></span>](../api/chartlineformat-clear.md)|<span data-ttu-id="daeee-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="daeee-116">None</span></span>|<span data-ttu-id="daeee-117">Limpe a formatação da linha de um elemento do gráfico.</span><span class="sxs-lookup"><span data-stu-id="daeee-117">Clear the line format of a chart element.</span></span>|

## <a name="properties"></a><span data-ttu-id="daeee-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="daeee-118">Properties</span></span>
| <span data-ttu-id="daeee-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="daeee-119">Property</span></span>     | <span data-ttu-id="daeee-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="daeee-120">Type</span></span>   |<span data-ttu-id="daeee-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="daeee-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="daeee-122">color</span><span class="sxs-lookup"><span data-stu-id="daeee-122">color</span></span>|<span data-ttu-id="daeee-123">string</span><span class="sxs-lookup"><span data-stu-id="daeee-123">string</span></span>|<span data-ttu-id="daeee-124">Código de cores HTML que representa a cor das linhas no gráfico.</span><span class="sxs-lookup"><span data-stu-id="daeee-124">HTML color code representing the color of lines in the chart.</span></span>|

## <a name="relationships"></a><span data-ttu-id="daeee-125">Relações</span><span class="sxs-lookup"><span data-stu-id="daeee-125">Relationships</span></span>
<span data-ttu-id="daeee-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="daeee-126">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="daeee-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="daeee-127">JSON representation</span></span>

<span data-ttu-id="daeee-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="daeee-128">Here is a JSON representation of the resource.</span></span>

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
