---
title: Tipo de recurso ChartGridlines
description: Representa as linhas de grade principais ou secundárias em um eixo do gráfico.
author: lumine2008
ms.openlocfilehash: 2aaf044b09d061af4853e76e0f2ba118bd1b2321
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27353029"
---
# <a name="chartgridlines-resource-type"></a><span data-ttu-id="31848-103">Tipo de recurso ChartGridlines</span><span class="sxs-lookup"><span data-stu-id="31848-103">ChartGridlines resource type</span></span>

<span data-ttu-id="31848-104">Representa as linhas de grade principais ou secundárias em um eixo do gráfico.</span><span class="sxs-lookup"><span data-stu-id="31848-104">Represents major or minor gridlines on a chart axis.</span></span>


## <a name="methods"></a><span data-ttu-id="31848-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="31848-105">Methods</span></span>

| <span data-ttu-id="31848-106">Método</span><span class="sxs-lookup"><span data-stu-id="31848-106">Method</span></span>           | <span data-ttu-id="31848-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="31848-107">Return Type</span></span>    |<span data-ttu-id="31848-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="31848-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="31848-109">Get ChartGridlines</span><span class="sxs-lookup"><span data-stu-id="31848-109">Get ChartGridlines</span></span>](../api/chartgridlines-get.md) | [<span data-ttu-id="31848-110">WorkbookChartGridlines</span><span class="sxs-lookup"><span data-stu-id="31848-110">WorkbookChartGridlines</span></span>](chartgridlines.md) |<span data-ttu-id="31848-111">Leia as propriedades e os relacionamentos do objeto chartGridlines.</span><span class="sxs-lookup"><span data-stu-id="31848-111">Read properties and relationships of chartGridlines object.</span></span>|
|[<span data-ttu-id="31848-112">Update</span><span class="sxs-lookup"><span data-stu-id="31848-112">Update</span></span>](../api/chartgridlines-update.md) | [<span data-ttu-id="31848-113">WorkbookChartGridlines</span><span class="sxs-lookup"><span data-stu-id="31848-113">WorkbookChartGridlines</span></span>](chartgridlines.md)    |<span data-ttu-id="31848-114">Atualize o objeto ChartGridlines.</span><span class="sxs-lookup"><span data-stu-id="31848-114">Update ChartGridlines object.</span></span> |

## <a name="properties"></a><span data-ttu-id="31848-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="31848-115">Properties</span></span>
| <span data-ttu-id="31848-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="31848-116">Property</span></span>     | <span data-ttu-id="31848-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="31848-117">Type</span></span>   |<span data-ttu-id="31848-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="31848-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="31848-119">visible</span><span class="sxs-lookup"><span data-stu-id="31848-119">visible</span></span>|<span data-ttu-id="31848-120">booliano</span><span class="sxs-lookup"><span data-stu-id="31848-120">boolean</span></span>|<span data-ttu-id="31848-121">Valor booliano que determina se as linhas de grade do eixo ficam visíveis ou não.</span><span class="sxs-lookup"><span data-stu-id="31848-121">Boolean value representing if the axis gridlines are visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="31848-122">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="31848-122">Relationships</span></span>
| <span data-ttu-id="31848-123">Relação</span><span class="sxs-lookup"><span data-stu-id="31848-123">Relationship</span></span> | <span data-ttu-id="31848-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="31848-124">Type</span></span>   |<span data-ttu-id="31848-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="31848-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="31848-126">formato</span><span class="sxs-lookup"><span data-stu-id="31848-126">format</span></span>|[<span data-ttu-id="31848-127">WorkbookChartGridlinesFormat</span><span class="sxs-lookup"><span data-stu-id="31848-127">WorkbookChartGridlinesFormat</span></span>](chartgridlinesformat.md)|<span data-ttu-id="31848-p101">Representa a formatação de linhas de grade do gráfico. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="31848-p101">Represents the formatting of chart gridlines. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="31848-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="31848-130">JSON representation</span></span>

<span data-ttu-id="31848-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="31848-131">Here is a JSON representation of the resource.</span></span>

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