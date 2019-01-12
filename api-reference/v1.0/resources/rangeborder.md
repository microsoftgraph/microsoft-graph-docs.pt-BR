---
title: Tipo de recurso RangeBorder
description: Representa a borda de um objeto.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 9c32264311400951152f892e6f88d70645f47064
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27947607"
---
# <a name="rangeborder-resource-type"></a><span data-ttu-id="73694-103">Tipo de recurso RangeBorder</span><span class="sxs-lookup"><span data-stu-id="73694-103">RangeBorder resource type</span></span>

<span data-ttu-id="73694-104">Representa a borda de um objeto.</span><span class="sxs-lookup"><span data-stu-id="73694-104">Represents the border of an object.</span></span>


## <a name="methods"></a><span data-ttu-id="73694-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="73694-105">Methods</span></span>

| <span data-ttu-id="73694-106">Método</span><span class="sxs-lookup"><span data-stu-id="73694-106">Method</span></span>           | <span data-ttu-id="73694-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="73694-107">Return Type</span></span>    |<span data-ttu-id="73694-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="73694-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="73694-109">Get RangeBorder</span><span class="sxs-lookup"><span data-stu-id="73694-109">Get RangeBorder</span></span>](../api/rangeborder-get.md) | [<span data-ttu-id="73694-110">WorkbookRangeBorder</span><span class="sxs-lookup"><span data-stu-id="73694-110">WorkbookRangeBorder</span></span>](rangeborder.md) |<span data-ttu-id="73694-111">Leia as propriedades e relacionamentos do objeto rangeBorder.</span><span class="sxs-lookup"><span data-stu-id="73694-111">Read properties and relationships of rangeBorder object.</span></span>|
|[<span data-ttu-id="73694-112">Update</span><span class="sxs-lookup"><span data-stu-id="73694-112">Update</span></span>](../api/rangeborder-update.md) | [<span data-ttu-id="73694-113">WorkbookRangeBorder</span><span class="sxs-lookup"><span data-stu-id="73694-113">WorkbookRangeBorder</span></span>](rangeborder.md) |<span data-ttu-id="73694-114">Atualize o objeto RangeBorder.</span><span class="sxs-lookup"><span data-stu-id="73694-114">Update RangeBorder object.</span></span> |
|[<span data-ttu-id="73694-115">List</span><span class="sxs-lookup"><span data-stu-id="73694-115">List</span></span>](../api/rangeborder-list.md) | <span data-ttu-id="73694-116">Coleção [WorkbookRangeBorder](rangeborder.md)</span><span class="sxs-lookup"><span data-stu-id="73694-116">[WorkbookRangeBorder](rangeborder.md) collection</span></span> |<span data-ttu-id="73694-117">Obtenha a coleção de objetos rangeBorder.</span><span class="sxs-lookup"><span data-stu-id="73694-117">Get rangeBorder object collection.</span></span> |
|[<span data-ttu-id="73694-118">Itemat</span><span class="sxs-lookup"><span data-stu-id="73694-118">Itemat</span></span>](../api/rangebordercollection-itemat.md)|[<span data-ttu-id="73694-119">WorkbookRangeBorder</span><span class="sxs-lookup"><span data-stu-id="73694-119">WorkbookRangeBorder</span></span>](rangeborder.md)|<span data-ttu-id="73694-120">Obtém um objeto de borda usando seu índice.</span><span class="sxs-lookup"><span data-stu-id="73694-120">Gets a border object using its index</span></span>|

## <a name="properties"></a><span data-ttu-id="73694-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="73694-121">Properties</span></span>
| <span data-ttu-id="73694-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="73694-122">Property</span></span>     | <span data-ttu-id="73694-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="73694-123">Type</span></span>   |<span data-ttu-id="73694-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="73694-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="73694-125">color</span><span class="sxs-lookup"><span data-stu-id="73694-125">color</span></span>|<span data-ttu-id="73694-126">string</span><span class="sxs-lookup"><span data-stu-id="73694-126">string</span></span>|<span data-ttu-id="73694-127">Código de cor HTML que representa a cor #RRGGBB da linha de borda do formulário (por exemplo, "FFA500") ou uma cor HTML nomeada (por exemplo, "laranja").</span><span class="sxs-lookup"><span data-stu-id="73694-127">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange").</span></span>|
|<span data-ttu-id="73694-128">id</span><span class="sxs-lookup"><span data-stu-id="73694-128">id</span></span>|<span data-ttu-id="73694-129">string</span><span class="sxs-lookup"><span data-stu-id="73694-129">string</span></span>|<span data-ttu-id="73694-130">Representa o identificador da borda.</span><span class="sxs-lookup"><span data-stu-id="73694-130">Represents border identifier.</span></span> <span data-ttu-id="73694-131">Os valores possíveis são: `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`, `DiagonalUp`.</span><span class="sxs-lookup"><span data-stu-id="73694-131">The possible values are: `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`, `DiagonalUp`.</span></span> <span data-ttu-id="73694-132">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="73694-132">Read-only.</span></span>|
|<span data-ttu-id="73694-133">sideIndex</span><span class="sxs-lookup"><span data-stu-id="73694-133">sideIndex</span></span>|<span data-ttu-id="73694-134">string</span><span class="sxs-lookup"><span data-stu-id="73694-134">string</span></span>|<span data-ttu-id="73694-135">Valor de constante que indica o lado específico da borda.</span><span class="sxs-lookup"><span data-stu-id="73694-135">Constant value that indicates the specific side of the border.</span></span> <span data-ttu-id="73694-136">Os valores possíveis são: `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`, `DiagonalUp`.</span><span class="sxs-lookup"><span data-stu-id="73694-136">The possible values are: `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`, `DiagonalUp`.</span></span> <span data-ttu-id="73694-137">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="73694-137">Read-only.</span></span>|
|<span data-ttu-id="73694-138">style</span><span class="sxs-lookup"><span data-stu-id="73694-138">style</span></span>|<span data-ttu-id="73694-139">string</span><span class="sxs-lookup"><span data-stu-id="73694-139">string</span></span>|<span data-ttu-id="73694-140">Uma das constantes de estilo de linha, especificando o estilo de linha da borda.</span><span class="sxs-lookup"><span data-stu-id="73694-140">One of the constants of line style specifying the line style for the border.</span></span> <span data-ttu-id="73694-141">Os valores possíveis são: `None`, `Continuous`, `Dash`, `DashDot`, `DashDotDot`, `Dot`, `Double`, `SlantDashDot`.</span><span class="sxs-lookup"><span data-stu-id="73694-141">The possible values are: `None`, `Continuous`, `Dash`, `DashDot`, `DashDotDot`, `Dot`, `Double`, `SlantDashDot`.</span></span>|
|<span data-ttu-id="73694-142">weight</span><span class="sxs-lookup"><span data-stu-id="73694-142">weight</span></span>|<span data-ttu-id="73694-143">string</span><span class="sxs-lookup"><span data-stu-id="73694-143">string</span></span>|<span data-ttu-id="73694-144">Especifica o peso da borda em torno de um intervalo.</span><span class="sxs-lookup"><span data-stu-id="73694-144">Specifies the weight of the border around a range.</span></span> <span data-ttu-id="73694-145">Os valores possíveis são: `Hairline`, `Thin`, `Medium`, `Thick`.</span><span class="sxs-lookup"><span data-stu-id="73694-145">The possible values are: `Hairline`, `Thin`, `Medium`, `Thick`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="73694-146">Relações</span><span class="sxs-lookup"><span data-stu-id="73694-146">Relationships</span></span>
<span data-ttu-id="73694-147">Nenhum</span><span class="sxs-lookup"><span data-stu-id="73694-147">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="73694-148">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="73694-148">JSON representation</span></span>

<span data-ttu-id="73694-149">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="73694-149">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookRangeBorder"
}-->

```json
{
  "color": "string",
  "id": "string",
  "sideIndex": "string",
  "style": "string",
  "weight": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "RangeBorder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
