---
title: tipo de recurso workbookChartLineFormat
description: Encapsula as opções de formatação dos elementos de linha.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: b40c72240771edd3517f2b29df269d83adeec8f8
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348502"
---
# <a name="workbookchartlineformat-resource-type"></a><span data-ttu-id="48b3e-103">tipo de recurso workbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="48b3e-103">workbookChartLineFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="48b3e-104">Encapsula as opções de formatação dos elementos de linha.</span><span class="sxs-lookup"><span data-stu-id="48b3e-104">Enapsulates the formatting options for line elements.</span></span>


## <a name="methods"></a><span data-ttu-id="48b3e-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="48b3e-105">Methods</span></span>

| <span data-ttu-id="48b3e-106">Método</span><span class="sxs-lookup"><span data-stu-id="48b3e-106">Method</span></span>           | <span data-ttu-id="48b3e-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="48b3e-107">Return Type</span></span>    |<span data-ttu-id="48b3e-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="48b3e-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="48b3e-109">Obter workbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="48b3e-109">Get workbookChartLineFormat</span></span>](../api/chartlineformat-get.md) | [<span data-ttu-id="48b3e-110">workbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="48b3e-110">workbookChartLineFormat</span></span>](workbookchartlineformat.md) |<span data-ttu-id="48b3e-111">Leia as propriedades e os relacionamentos do objeto chartLineFormat.</span><span class="sxs-lookup"><span data-stu-id="48b3e-111">Read properties and relationships of chartLineFormat object.</span></span>|
|[<span data-ttu-id="48b3e-112">Update</span><span class="sxs-lookup"><span data-stu-id="48b3e-112">Update</span></span>](../api/chartlineformat-update.md) | [<span data-ttu-id="48b3e-113">workbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="48b3e-113">workbookChartLineFormat</span></span>](workbookchartlineformat.md) |<span data-ttu-id="48b3e-114">Atualize o objeto ChartLineFormat.</span><span class="sxs-lookup"><span data-stu-id="48b3e-114">Update ChartLineFormat object.</span></span> |
|[<span data-ttu-id="48b3e-115">Clear</span><span class="sxs-lookup"><span data-stu-id="48b3e-115">Clear</span></span>](../api/chartlineformat-clear.md)|<span data-ttu-id="48b3e-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="48b3e-116">None</span></span>|<span data-ttu-id="48b3e-117">Limpe a formatação da linha de um elemento do gráfico.</span><span class="sxs-lookup"><span data-stu-id="48b3e-117">Clear the line format of a chart element.</span></span>|

## <a name="properties"></a><span data-ttu-id="48b3e-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="48b3e-118">Properties</span></span>
| <span data-ttu-id="48b3e-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="48b3e-119">Property</span></span>     | <span data-ttu-id="48b3e-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="48b3e-120">Type</span></span>   |<span data-ttu-id="48b3e-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="48b3e-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="48b3e-122">color</span><span class="sxs-lookup"><span data-stu-id="48b3e-122">color</span></span>|<span data-ttu-id="48b3e-123">string</span><span class="sxs-lookup"><span data-stu-id="48b3e-123">string</span></span>|<span data-ttu-id="48b3e-124">Código de cores HTML que representa a cor das linhas no gráfico.</span><span class="sxs-lookup"><span data-stu-id="48b3e-124">HTML color code representing the color of lines in the chart.</span></span>|

## <a name="relationships"></a><span data-ttu-id="48b3e-125">Relações</span><span class="sxs-lookup"><span data-stu-id="48b3e-125">Relationships</span></span>
<span data-ttu-id="48b3e-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="48b3e-126">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="48b3e-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="48b3e-127">JSON representation</span></span>

<span data-ttu-id="48b3e-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="48b3e-128">Here is a JSON representation of the resource.</span></span>

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
