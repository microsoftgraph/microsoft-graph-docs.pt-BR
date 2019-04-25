---
title: Tipo de recurso RangeBorder
description: Representa a borda de um objeto.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 9c32264311400951152f892e6f88d70645f47064
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32579484"
---
# <a name="rangeborder-resource-type"></a><span data-ttu-id="e53a8-103">Tipo de recurso RangeBorder</span><span class="sxs-lookup"><span data-stu-id="e53a8-103">RangeBorder resource type</span></span>

<span data-ttu-id="e53a8-104">Representa a borda de um objeto.</span><span class="sxs-lookup"><span data-stu-id="e53a8-104">Represents the border of an object.</span></span>


## <a name="methods"></a><span data-ttu-id="e53a8-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="e53a8-105">Methods</span></span>

| <span data-ttu-id="e53a8-106">Método</span><span class="sxs-lookup"><span data-stu-id="e53a8-106">Method</span></span>           | <span data-ttu-id="e53a8-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e53a8-107">Return Type</span></span>    |<span data-ttu-id="e53a8-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="e53a8-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e53a8-109">Get RangeBorder</span><span class="sxs-lookup"><span data-stu-id="e53a8-109">Get RangeBorder</span></span>](../api/rangeborder-get.md) | [<span data-ttu-id="e53a8-110">WorkbookRangeBorder</span><span class="sxs-lookup"><span data-stu-id="e53a8-110">WorkbookRangeBorder</span></span>](rangeborder.md) |<span data-ttu-id="e53a8-111">Leia as propriedades e relacionamentos do objeto rangeBorder.</span><span class="sxs-lookup"><span data-stu-id="e53a8-111">Read properties and relationships of rangeBorder object.</span></span>|
|[<span data-ttu-id="e53a8-112">Update</span><span class="sxs-lookup"><span data-stu-id="e53a8-112">Update</span></span>](../api/rangeborder-update.md) | [<span data-ttu-id="e53a8-113">WorkbookRangeBorder</span><span class="sxs-lookup"><span data-stu-id="e53a8-113">WorkbookRangeBorder</span></span>](rangeborder.md) |<span data-ttu-id="e53a8-114">Atualize o objeto RangeBorder.</span><span class="sxs-lookup"><span data-stu-id="e53a8-114">Update RangeBorder object.</span></span> |
|[<span data-ttu-id="e53a8-115">List</span><span class="sxs-lookup"><span data-stu-id="e53a8-115">List</span></span>](../api/rangeborder-list.md) | <span data-ttu-id="e53a8-116">Coleção [WorkbookRangeBorder](rangeborder.md)</span><span class="sxs-lookup"><span data-stu-id="e53a8-116">[WorkbookRangeBorder](rangeborder.md) collection</span></span> |<span data-ttu-id="e53a8-117">Obtenha a coleção de objetos rangeBorder.</span><span class="sxs-lookup"><span data-stu-id="e53a8-117">Get rangeBorder object collection.</span></span> |
|[<span data-ttu-id="e53a8-118">Itemat</span><span class="sxs-lookup"><span data-stu-id="e53a8-118">Itemat</span></span>](../api/rangebordercollection-itemat.md)|[<span data-ttu-id="e53a8-119">WorkbookRangeBorder</span><span class="sxs-lookup"><span data-stu-id="e53a8-119">WorkbookRangeBorder</span></span>](rangeborder.md)|<span data-ttu-id="e53a8-120">Obtém um objeto de borda usando seu índice.</span><span class="sxs-lookup"><span data-stu-id="e53a8-120">Gets a border object using its index</span></span>|

## <a name="properties"></a><span data-ttu-id="e53a8-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e53a8-121">Properties</span></span>
| <span data-ttu-id="e53a8-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e53a8-122">Property</span></span>     | <span data-ttu-id="e53a8-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="e53a8-123">Type</span></span>   |<span data-ttu-id="e53a8-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="e53a8-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e53a8-125">color</span><span class="sxs-lookup"><span data-stu-id="e53a8-125">color</span></span>|<span data-ttu-id="e53a8-126">string</span><span class="sxs-lookup"><span data-stu-id="e53a8-126">string</span></span>|<span data-ttu-id="e53a8-127">Código de cor HTML que representa a cor #RRGGBB da linha de borda do formulário (por exemplo, "FFA500") ou uma cor HTML nomeada (por exemplo, "laranja").</span><span class="sxs-lookup"><span data-stu-id="e53a8-127">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange").</span></span>|
|<span data-ttu-id="e53a8-128">id</span><span class="sxs-lookup"><span data-stu-id="e53a8-128">id</span></span>|<span data-ttu-id="e53a8-129">string</span><span class="sxs-lookup"><span data-stu-id="e53a8-129">string</span></span>|<span data-ttu-id="e53a8-130">Representa o identificador da borda.</span><span class="sxs-lookup"><span data-stu-id="e53a8-130">Represents border identifier.</span></span> <span data-ttu-id="e53a8-131">Os valores possíveis são: `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`, `DiagonalUp`.</span><span class="sxs-lookup"><span data-stu-id="e53a8-131">The possible values are: `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`, `DiagonalUp`.</span></span> <span data-ttu-id="e53a8-132">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e53a8-132">Read-only.</span></span>|
|<span data-ttu-id="e53a8-133">sideIndex</span><span class="sxs-lookup"><span data-stu-id="e53a8-133">sideIndex</span></span>|<span data-ttu-id="e53a8-134">string</span><span class="sxs-lookup"><span data-stu-id="e53a8-134">string</span></span>|<span data-ttu-id="e53a8-135">Valor constante que indica o lado específico da borda.</span><span class="sxs-lookup"><span data-stu-id="e53a8-135">Constant value that indicates the specific side of the border.</span></span> <span data-ttu-id="e53a8-136">Os valores possíveis são: `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`, `DiagonalUp`.</span><span class="sxs-lookup"><span data-stu-id="e53a8-136">The possible values are: `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`, `DiagonalUp`.</span></span> <span data-ttu-id="e53a8-137">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e53a8-137">Read-only.</span></span>|
|<span data-ttu-id="e53a8-138">estilo</span><span class="sxs-lookup"><span data-stu-id="e53a8-138">style</span></span>|<span data-ttu-id="e53a8-139">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e53a8-139">string</span></span>|<span data-ttu-id="e53a8-140">Uma das constantes de estilo de linha especificando o estilo de linha da borda.</span><span class="sxs-lookup"><span data-stu-id="e53a8-140">One of the constants of line style specifying the line style for the border.</span></span> <span data-ttu-id="e53a8-141">Os valores possíveis são: `None`, `Continuous`, `Dash`, `DashDot`, `DashDotDot`, `Dot`, `Double`, `SlantDashDot`.</span><span class="sxs-lookup"><span data-stu-id="e53a8-141">The possible values are: `None`, `Continuous`, `Dash`, `DashDot`, `DashDotDot`, `Dot`, `Double`, `SlantDashDot`.</span></span>|
|<span data-ttu-id="e53a8-142">weight</span><span class="sxs-lookup"><span data-stu-id="e53a8-142">weight</span></span>|<span data-ttu-id="e53a8-143">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e53a8-143">string</span></span>|<span data-ttu-id="e53a8-144">Especifica a espessura da borda em torno de um intervalo.</span><span class="sxs-lookup"><span data-stu-id="e53a8-144">Specifies the weight of the border around a range.</span></span> <span data-ttu-id="e53a8-145">Os valores possíveis são: `Hairline`, `Thin`, `Medium`, `Thick`.</span><span class="sxs-lookup"><span data-stu-id="e53a8-145">The possible values are: `Hairline`, `Thin`, `Medium`, `Thick`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e53a8-146">Relações</span><span class="sxs-lookup"><span data-stu-id="e53a8-146">Relationships</span></span>
<span data-ttu-id="e53a8-147">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e53a8-147">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="e53a8-148">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e53a8-148">JSON representation</span></span>

<span data-ttu-id="e53a8-149">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e53a8-149">Here is a JSON representation of the resource.</span></span>

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
