---
title: Tipo de recurso RangeBorder
description: Representa a borda de um objeto.
author: lumine2008
ms.openlocfilehash: c6166e1cfebc0759ad25fda5c0e8ec471af07b11
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27359147"
---
# <a name="rangeborder-resource-type"></a><span data-ttu-id="f7769-103">Tipo de recurso RangeBorder</span><span class="sxs-lookup"><span data-stu-id="f7769-103">RangeBorder resource type</span></span>

<span data-ttu-id="f7769-104">Representa a borda de um objeto.</span><span class="sxs-lookup"><span data-stu-id="f7769-104">Represents the border of an object.</span></span>


## <a name="methods"></a><span data-ttu-id="f7769-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="f7769-105">Methods</span></span>

| <span data-ttu-id="f7769-106">Método</span><span class="sxs-lookup"><span data-stu-id="f7769-106">Method</span></span>           | <span data-ttu-id="f7769-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f7769-107">Return Type</span></span>    |<span data-ttu-id="f7769-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="f7769-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f7769-109">Get RangeBorder</span><span class="sxs-lookup"><span data-stu-id="f7769-109">Get RangeBorder</span></span>](../api/rangeborder-get.md) | [<span data-ttu-id="f7769-110">WorkbookRangeBorder</span><span class="sxs-lookup"><span data-stu-id="f7769-110">WorkbookRangeBorder</span></span>](rangeborder.md) |<span data-ttu-id="f7769-111">Leia as propriedades e relacionamentos do objeto rangeBorder.</span><span class="sxs-lookup"><span data-stu-id="f7769-111">Read properties and relationships of rangeBorder object.</span></span>|
|[<span data-ttu-id="f7769-112">Update</span><span class="sxs-lookup"><span data-stu-id="f7769-112">Update</span></span>](../api/rangeborder-update.md) | [<span data-ttu-id="f7769-113">WorkbookRangeBorder</span><span class="sxs-lookup"><span data-stu-id="f7769-113">WorkbookRangeBorder</span></span>](rangeborder.md) |<span data-ttu-id="f7769-114">Atualize o objeto RangeBorder.</span><span class="sxs-lookup"><span data-stu-id="f7769-114">Update RangeBorder object.</span></span> |
|[<span data-ttu-id="f7769-115">List</span><span class="sxs-lookup"><span data-stu-id="f7769-115">List</span></span>](../api/rangeborder-list.md) | <span data-ttu-id="f7769-116">Coleção [WorkbookRangeBorder](rangeborder.md)</span><span class="sxs-lookup"><span data-stu-id="f7769-116">[WorkbookRangeBorder](rangeborder.md) collection</span></span> |<span data-ttu-id="f7769-117">Obtenha a coleção de objetos rangeBorder.</span><span class="sxs-lookup"><span data-stu-id="f7769-117">Get rangeBorder object collection.</span></span> |
|[<span data-ttu-id="f7769-118">Itemat</span><span class="sxs-lookup"><span data-stu-id="f7769-118">Itemat</span></span>](../api/rangebordercollection-itemat.md)|[<span data-ttu-id="f7769-119">WorkbookRangeBorder</span><span class="sxs-lookup"><span data-stu-id="f7769-119">WorkbookRangeBorder</span></span>](rangeborder.md)|<span data-ttu-id="f7769-120">Obtém um objeto de borda usando seu índice.</span><span class="sxs-lookup"><span data-stu-id="f7769-120">Gets a border object using its index</span></span>|

## <a name="properties"></a><span data-ttu-id="f7769-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f7769-121">Properties</span></span>
| <span data-ttu-id="f7769-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f7769-122">Property</span></span>     | <span data-ttu-id="f7769-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="f7769-123">Type</span></span>   |<span data-ttu-id="f7769-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="f7769-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f7769-125">color</span><span class="sxs-lookup"><span data-stu-id="f7769-125">color</span></span>|<span data-ttu-id="f7769-126">string</span><span class="sxs-lookup"><span data-stu-id="f7769-126">string</span></span>|<span data-ttu-id="f7769-127">Código de cor HTML que representa a cor #RRGGBB da linha de borda do formulário (por exemplo, "FFA500") ou uma cor HTML nomeada (por exemplo, "laranja").</span><span class="sxs-lookup"><span data-stu-id="f7769-127">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange").</span></span>|
|<span data-ttu-id="f7769-128">id</span><span class="sxs-lookup"><span data-stu-id="f7769-128">id</span></span>|<span data-ttu-id="f7769-129">string</span><span class="sxs-lookup"><span data-stu-id="f7769-129">string</span></span>|<span data-ttu-id="f7769-130">Representa o identificador da borda.</span><span class="sxs-lookup"><span data-stu-id="f7769-130">Represents border identifier.</span></span> <span data-ttu-id="f7769-131">Os valores possíveis são: `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`, `DiagonalUp`.</span><span class="sxs-lookup"><span data-stu-id="f7769-131">The possible values are: `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`, `DiagonalUp`.</span></span> <span data-ttu-id="f7769-132">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f7769-132">Read-only.</span></span>|
|<span data-ttu-id="f7769-133">sideIndex</span><span class="sxs-lookup"><span data-stu-id="f7769-133">sideIndex</span></span>|<span data-ttu-id="f7769-134">string</span><span class="sxs-lookup"><span data-stu-id="f7769-134">string</span></span>|<span data-ttu-id="f7769-135">Valor de constante que indica o lado específico da borda.</span><span class="sxs-lookup"><span data-stu-id="f7769-135">Constant value that indicates the specific side of the border.</span></span> <span data-ttu-id="f7769-136">Os valores possíveis são: `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`, `DiagonalUp`.</span><span class="sxs-lookup"><span data-stu-id="f7769-136">The possible values are: `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`, `DiagonalUp`.</span></span> <span data-ttu-id="f7769-137">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f7769-137">Read-only.</span></span>|
|<span data-ttu-id="f7769-138">style</span><span class="sxs-lookup"><span data-stu-id="f7769-138">style</span></span>|<span data-ttu-id="f7769-139">string</span><span class="sxs-lookup"><span data-stu-id="f7769-139">string</span></span>|<span data-ttu-id="f7769-140">Uma das constantes de estilo de linha, especificando o estilo de linha da borda.</span><span class="sxs-lookup"><span data-stu-id="f7769-140">One of the constants of line style specifying the line style for the border.</span></span> <span data-ttu-id="f7769-141">Os valores possíveis são: `None`, `Continuous`, `Dash`, `DashDot`, `DashDotDot`, `Dot`, `Double`, `SlantDashDot`.</span><span class="sxs-lookup"><span data-stu-id="f7769-141">The possible values are: `None`, `Continuous`, `Dash`, `DashDot`, `DashDotDot`, `Dot`, `Double`, `SlantDashDot`.</span></span>|
|<span data-ttu-id="f7769-142">weight</span><span class="sxs-lookup"><span data-stu-id="f7769-142">weight</span></span>|<span data-ttu-id="f7769-143">string</span><span class="sxs-lookup"><span data-stu-id="f7769-143">string</span></span>|<span data-ttu-id="f7769-144">Especifica o peso da borda em torno de um intervalo.</span><span class="sxs-lookup"><span data-stu-id="f7769-144">Specifies the weight of the border around a range.</span></span> <span data-ttu-id="f7769-145">Os valores possíveis são: `Hairline`, `Thin`, `Medium`, `Thick`.</span><span class="sxs-lookup"><span data-stu-id="f7769-145">The possible values are: `Hairline`, `Thin`, `Medium`, `Thick`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f7769-146">Relações</span><span class="sxs-lookup"><span data-stu-id="f7769-146">Relationships</span></span>
<span data-ttu-id="f7769-147">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f7769-147">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="f7769-148">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f7769-148">JSON representation</span></span>

<span data-ttu-id="f7769-149">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f7769-149">Here is a JSON representation of the resource.</span></span>

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