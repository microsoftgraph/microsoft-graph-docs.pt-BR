---
title: Tipo de recurso ChartLineFormat
description: Abrange as opções de formatação dos elementos de linha.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 6bede2e3e8eeb44dbac67832621a2b1586c6b319
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29577050"
---
# <a name="chartlineformat-resource-type"></a><span data-ttu-id="d50bc-103">Tipo de recurso ChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="d50bc-103">ChartLineFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d50bc-104">Abrange as opções de formatação dos elementos de linha.</span><span class="sxs-lookup"><span data-stu-id="d50bc-104">Enapsulates the formatting options for line elements.</span></span>


## <a name="methods"></a><span data-ttu-id="d50bc-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="d50bc-105">Methods</span></span>

| <span data-ttu-id="d50bc-106">Método</span><span class="sxs-lookup"><span data-stu-id="d50bc-106">Method</span></span>           | <span data-ttu-id="d50bc-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d50bc-107">Return Type</span></span>    |<span data-ttu-id="d50bc-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="d50bc-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d50bc-109">Get ChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="d50bc-109">Get ChartLineFormat</span></span>](../api/chartlineformat-get.md) | [<span data-ttu-id="d50bc-110">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="d50bc-110">WorkbookChartLineFormat</span></span>](chartlineformat.md) |<span data-ttu-id="d50bc-111">Leia as propriedades e os relacionamentos do objeto chartLineFormat.</span><span class="sxs-lookup"><span data-stu-id="d50bc-111">Read properties and relationships of chartLineFormat object.</span></span>|
|[<span data-ttu-id="d50bc-112">Update</span><span class="sxs-lookup"><span data-stu-id="d50bc-112">Update</span></span>](../api/chartlineformat-update.md) | [<span data-ttu-id="d50bc-113">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="d50bc-113">WorkbookChartLineFormat</span></span>](chartlineformat.md) |<span data-ttu-id="d50bc-114">Atualize o objeto ChartLineFormat.</span><span class="sxs-lookup"><span data-stu-id="d50bc-114">Update ChartLineFormat object.</span></span> |
|[<span data-ttu-id="d50bc-115">Clear</span><span class="sxs-lookup"><span data-stu-id="d50bc-115">Clear</span></span>](../api/chartlineformat-clear.md)|<span data-ttu-id="d50bc-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d50bc-116">None</span></span>|<span data-ttu-id="d50bc-117">Limpe a formatação da linha de um elemento do gráfico.</span><span class="sxs-lookup"><span data-stu-id="d50bc-117">Clear the line format of a chart element.</span></span>|

## <a name="properties"></a><span data-ttu-id="d50bc-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d50bc-118">Properties</span></span>
| <span data-ttu-id="d50bc-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d50bc-119">Property</span></span>     | <span data-ttu-id="d50bc-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="d50bc-120">Type</span></span>   |<span data-ttu-id="d50bc-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="d50bc-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d50bc-122">color</span><span class="sxs-lookup"><span data-stu-id="d50bc-122">color</span></span>|<span data-ttu-id="d50bc-123">string</span><span class="sxs-lookup"><span data-stu-id="d50bc-123">string</span></span>|<span data-ttu-id="d50bc-124">Código de cor HTML que representa a cor das linhas no gráfico.</span><span class="sxs-lookup"><span data-stu-id="d50bc-124">HTML color code representing the color of lines in the chart.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d50bc-125">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="d50bc-125">Relationships</span></span>
<span data-ttu-id="d50bc-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d50bc-126">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="d50bc-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d50bc-127">JSON representation</span></span>

<span data-ttu-id="d50bc-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d50bc-128">Here is a JSON representation of the resource.</span></span>

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
  "description": "ChartLineFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chartlineformat.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
