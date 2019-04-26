---
title: Tipo de recurso ChartGridlines
description: Representa linhas de grade principais ou secundárias em um eixo do gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 7347ac1b7ff251b12764534df217cd883ba730b3
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32569022"
---
# <a name="chartgridlines-resource-type"></a><span data-ttu-id="369e9-103">Tipo de recurso ChartGridlines</span><span class="sxs-lookup"><span data-stu-id="369e9-103">ChartGridlines resource type</span></span>

<span data-ttu-id="369e9-104">Representa linhas de grade principais ou secundárias em um eixo do gráfico.</span><span class="sxs-lookup"><span data-stu-id="369e9-104">Represents major or minor gridlines on a chart axis.</span></span>


## <a name="methods"></a><span data-ttu-id="369e9-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="369e9-105">Methods</span></span>

| <span data-ttu-id="369e9-106">Método</span><span class="sxs-lookup"><span data-stu-id="369e9-106">Method</span></span>           | <span data-ttu-id="369e9-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="369e9-107">Return Type</span></span>    |<span data-ttu-id="369e9-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="369e9-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="369e9-109">Get ChartGridlines</span><span class="sxs-lookup"><span data-stu-id="369e9-109">Get ChartGridlines</span></span>](../api/chartgridlines-get.md) | [<span data-ttu-id="369e9-110">WorkbookChartGridlines</span><span class="sxs-lookup"><span data-stu-id="369e9-110">WorkbookChartGridlines</span></span>](chartgridlines.md) |<span data-ttu-id="369e9-111">Leia as propriedades e os relacionamentos do objeto chartGridlines.</span><span class="sxs-lookup"><span data-stu-id="369e9-111">Read properties and relationships of chartGridlines object.</span></span>|
|[<span data-ttu-id="369e9-112">Update</span><span class="sxs-lookup"><span data-stu-id="369e9-112">Update</span></span>](../api/chartgridlines-update.md) | [<span data-ttu-id="369e9-113">WorkbookChartGridlines</span><span class="sxs-lookup"><span data-stu-id="369e9-113">WorkbookChartGridlines</span></span>](chartgridlines.md)    |<span data-ttu-id="369e9-114">Atualize o objeto ChartGridlines.</span><span class="sxs-lookup"><span data-stu-id="369e9-114">Update ChartGridlines object.</span></span> |

## <a name="properties"></a><span data-ttu-id="369e9-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="369e9-115">Properties</span></span>
| <span data-ttu-id="369e9-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="369e9-116">Property</span></span>     | <span data-ttu-id="369e9-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="369e9-117">Type</span></span>   |<span data-ttu-id="369e9-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="369e9-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="369e9-119">visible</span><span class="sxs-lookup"><span data-stu-id="369e9-119">visible</span></span>|<span data-ttu-id="369e9-120">booliano</span><span class="sxs-lookup"><span data-stu-id="369e9-120">boolean</span></span>|<span data-ttu-id="369e9-121">Valor booliano que determina se as linhas de grade do eixo ficam visíveis ou não.</span><span class="sxs-lookup"><span data-stu-id="369e9-121">Boolean value representing if the axis gridlines are visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="369e9-122">Relações</span><span class="sxs-lookup"><span data-stu-id="369e9-122">Relationships</span></span>
| <span data-ttu-id="369e9-123">Relação</span><span class="sxs-lookup"><span data-stu-id="369e9-123">Relationship</span></span> | <span data-ttu-id="369e9-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="369e9-124">Type</span></span>   |<span data-ttu-id="369e9-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="369e9-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="369e9-126">format</span><span class="sxs-lookup"><span data-stu-id="369e9-126">format</span></span>|[<span data-ttu-id="369e9-127">WorkbookChartGridlinesFormat</span><span class="sxs-lookup"><span data-stu-id="369e9-127">WorkbookChartGridlinesFormat</span></span>](chartgridlinesformat.md)|<span data-ttu-id="369e9-128">Representa a formatação de linhas de grade do gráfico.</span><span class="sxs-lookup"><span data-stu-id="369e9-128">Represents the formatting of chart gridlines.</span></span> <span data-ttu-id="369e9-129">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="369e9-129">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="369e9-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="369e9-130">JSON representation</span></span>

<span data-ttu-id="369e9-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="369e9-131">Here is a JSON representation of the resource.</span></span>

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
