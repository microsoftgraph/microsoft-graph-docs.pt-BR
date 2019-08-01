---
title: Tipo de recurso ChartGridlines
description: Representa linhas de grade principais ou secundárias em um eixo do gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: af1f9576c486174b6aa78dd3196c813e744a1552
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029796"
---
# <a name="chartgridlines-resource-type"></a><span data-ttu-id="53da7-103">Tipo de recurso ChartGridlines</span><span class="sxs-lookup"><span data-stu-id="53da7-103">ChartGridlines resource type</span></span>

<span data-ttu-id="53da7-104">Representa linhas de grade principais ou secundárias em um eixo do gráfico.</span><span class="sxs-lookup"><span data-stu-id="53da7-104">Represents major or minor gridlines on a chart axis.</span></span>


## <a name="methods"></a><span data-ttu-id="53da7-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="53da7-105">Methods</span></span>

| <span data-ttu-id="53da7-106">Método</span><span class="sxs-lookup"><span data-stu-id="53da7-106">Method</span></span>           | <span data-ttu-id="53da7-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="53da7-107">Return Type</span></span>    |<span data-ttu-id="53da7-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="53da7-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="53da7-109">Get ChartGridlines</span><span class="sxs-lookup"><span data-stu-id="53da7-109">Get ChartGridlines</span></span>](../api/chartgridlines-get.md) | [<span data-ttu-id="53da7-110">WorkbookChartGridlines</span><span class="sxs-lookup"><span data-stu-id="53da7-110">WorkbookChartGridlines</span></span>](chartgridlines.md) |<span data-ttu-id="53da7-111">Leia as propriedades e os relacionamentos do objeto chartGridlines.</span><span class="sxs-lookup"><span data-stu-id="53da7-111">Read properties and relationships of chartGridlines object.</span></span>|
|[<span data-ttu-id="53da7-112">Update</span><span class="sxs-lookup"><span data-stu-id="53da7-112">Update</span></span>](../api/chartgridlines-update.md) | [<span data-ttu-id="53da7-113">WorkbookChartGridlines</span><span class="sxs-lookup"><span data-stu-id="53da7-113">WorkbookChartGridlines</span></span>](chartgridlines.md)    |<span data-ttu-id="53da7-114">Atualize o objeto ChartGridlines.</span><span class="sxs-lookup"><span data-stu-id="53da7-114">Update ChartGridlines object.</span></span> |

## <a name="properties"></a><span data-ttu-id="53da7-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="53da7-115">Properties</span></span>
| <span data-ttu-id="53da7-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="53da7-116">Property</span></span>     | <span data-ttu-id="53da7-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="53da7-117">Type</span></span>   |<span data-ttu-id="53da7-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="53da7-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="53da7-119">visible</span><span class="sxs-lookup"><span data-stu-id="53da7-119">visible</span></span>|<span data-ttu-id="53da7-120">booliano</span><span class="sxs-lookup"><span data-stu-id="53da7-120">boolean</span></span>|<span data-ttu-id="53da7-121">Valor booliano que determina se as linhas de grade do eixo ficam visíveis ou não.</span><span class="sxs-lookup"><span data-stu-id="53da7-121">Boolean value representing if the axis gridlines are visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="53da7-122">Relações</span><span class="sxs-lookup"><span data-stu-id="53da7-122">Relationships</span></span>
| <span data-ttu-id="53da7-123">Relação</span><span class="sxs-lookup"><span data-stu-id="53da7-123">Relationship</span></span> | <span data-ttu-id="53da7-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="53da7-124">Type</span></span>   |<span data-ttu-id="53da7-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="53da7-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="53da7-126">formato</span><span class="sxs-lookup"><span data-stu-id="53da7-126">format</span></span>|[<span data-ttu-id="53da7-127">WorkbookChartGridlinesFormat</span><span class="sxs-lookup"><span data-stu-id="53da7-127">WorkbookChartGridlinesFormat</span></span>](chartgridlinesformat.md)|<span data-ttu-id="53da7-128">Representa a formatação de linhas de grade do gráfico.</span><span class="sxs-lookup"><span data-stu-id="53da7-128">Represents the formatting of chart gridlines.</span></span> <span data-ttu-id="53da7-129">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="53da7-129">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="53da7-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="53da7-130">JSON representation</span></span>

<span data-ttu-id="53da7-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="53da7-131">Here is a JSON representation of the resource.</span></span>

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
