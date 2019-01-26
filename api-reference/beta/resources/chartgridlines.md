---
title: Tipo de recurso ChartGridlines
description: Representa as linhas de grade principais ou secundárias em um eixo do gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 3c57c68e7d9dfcd26741d15e302dd5dddeaae378
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572532"
---
# <a name="chartgridlines-resource-type"></a><span data-ttu-id="07840-103">Tipo de recurso ChartGridlines</span><span class="sxs-lookup"><span data-stu-id="07840-103">ChartGridlines resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="07840-104">Representa as linhas de grade principais ou secundárias em um eixo do gráfico.</span><span class="sxs-lookup"><span data-stu-id="07840-104">Represents major or minor gridlines on a chart axis.</span></span>


## <a name="methods"></a><span data-ttu-id="07840-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="07840-105">Methods</span></span>

| <span data-ttu-id="07840-106">Método</span><span class="sxs-lookup"><span data-stu-id="07840-106">Method</span></span>           | <span data-ttu-id="07840-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="07840-107">Return Type</span></span>    |<span data-ttu-id="07840-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="07840-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="07840-109">Get ChartGridlines</span><span class="sxs-lookup"><span data-stu-id="07840-109">Get ChartGridlines</span></span>](../api/chartgridlines-get.md) | [<span data-ttu-id="07840-110">WorkbookChartGridlines</span><span class="sxs-lookup"><span data-stu-id="07840-110">WorkbookChartGridlines</span></span>](chartgridlines.md) |<span data-ttu-id="07840-111">Leia as propriedades e os relacionamentos do objeto chartGridlines.</span><span class="sxs-lookup"><span data-stu-id="07840-111">Read properties and relationships of chartGridlines object.</span></span>|
|[<span data-ttu-id="07840-112">Update</span><span class="sxs-lookup"><span data-stu-id="07840-112">Update</span></span>](../api/chartgridlines-update.md) | [<span data-ttu-id="07840-113">WorkbookChartGridlines</span><span class="sxs-lookup"><span data-stu-id="07840-113">WorkbookChartGridlines</span></span>](chartgridlines.md)    |<span data-ttu-id="07840-114">Atualize o objeto ChartGridlines.</span><span class="sxs-lookup"><span data-stu-id="07840-114">Update ChartGridlines object.</span></span> |

## <a name="properties"></a><span data-ttu-id="07840-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="07840-115">Properties</span></span>
| <span data-ttu-id="07840-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="07840-116">Property</span></span>     | <span data-ttu-id="07840-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="07840-117">Type</span></span>   |<span data-ttu-id="07840-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="07840-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="07840-119">visible</span><span class="sxs-lookup"><span data-stu-id="07840-119">visible</span></span>|<span data-ttu-id="07840-120">booliano</span><span class="sxs-lookup"><span data-stu-id="07840-120">boolean</span></span>|<span data-ttu-id="07840-121">Valor booliano que determina se as linhas de grade do eixo ficam visíveis ou não.</span><span class="sxs-lookup"><span data-stu-id="07840-121">Boolean value representing if the axis gridlines are visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="07840-122">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="07840-122">Relationships</span></span>
| <span data-ttu-id="07840-123">Relação</span><span class="sxs-lookup"><span data-stu-id="07840-123">Relationship</span></span> | <span data-ttu-id="07840-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="07840-124">Type</span></span>   |<span data-ttu-id="07840-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="07840-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="07840-126">formato</span><span class="sxs-lookup"><span data-stu-id="07840-126">format</span></span>|[<span data-ttu-id="07840-127">WorkbookChartGridlinesFormat</span><span class="sxs-lookup"><span data-stu-id="07840-127">WorkbookChartGridlinesFormat</span></span>](chartgridlinesformat.md)|<span data-ttu-id="07840-p101">Representa a formatação de linhas de grade do gráfico. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="07840-p101">Represents the formatting of chart gridlines. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="07840-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="07840-130">JSON representation</span></span>

<span data-ttu-id="07840-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="07840-131">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "ChartGridlines resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chartgridlines.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
