---
title: Tipo de recurso RangeBorder
description: Representa a borda de um objeto.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 8b5a12c05bed39363d8a8a01eef749f2e88b929e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034927"
---
# <a name="rangeborder-resource-type"></a><span data-ttu-id="b646f-103">Tipo de recurso RangeBorder</span><span class="sxs-lookup"><span data-stu-id="b646f-103">RangeBorder resource type</span></span>

<span data-ttu-id="b646f-104">Representa a borda de um objeto.</span><span class="sxs-lookup"><span data-stu-id="b646f-104">Represents the border of an object.</span></span>


## <a name="methods"></a><span data-ttu-id="b646f-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="b646f-105">Methods</span></span>

| <span data-ttu-id="b646f-106">Método</span><span class="sxs-lookup"><span data-stu-id="b646f-106">Method</span></span>           | <span data-ttu-id="b646f-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b646f-107">Return Type</span></span>    |<span data-ttu-id="b646f-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="b646f-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b646f-109">Get RangeBorder</span><span class="sxs-lookup"><span data-stu-id="b646f-109">Get RangeBorder</span></span>](../api/rangeborder-get.md) | [<span data-ttu-id="b646f-110">WorkbookRangeBorder</span><span class="sxs-lookup"><span data-stu-id="b646f-110">WorkbookRangeBorder</span></span>](rangeborder.md) |<span data-ttu-id="b646f-111">Leia as propriedades e relacionamentos do objeto rangeBorder.</span><span class="sxs-lookup"><span data-stu-id="b646f-111">Read properties and relationships of rangeBorder object.</span></span>|
|[<span data-ttu-id="b646f-112">Update</span><span class="sxs-lookup"><span data-stu-id="b646f-112">Update</span></span>](../api/rangeborder-update.md) | [<span data-ttu-id="b646f-113">WorkbookRangeBorder</span><span class="sxs-lookup"><span data-stu-id="b646f-113">WorkbookRangeBorder</span></span>](rangeborder.md) |<span data-ttu-id="b646f-114">Atualize o objeto RangeBorder.</span><span class="sxs-lookup"><span data-stu-id="b646f-114">Update RangeBorder object.</span></span> |
|[<span data-ttu-id="b646f-115">List</span><span class="sxs-lookup"><span data-stu-id="b646f-115">List</span></span>](../api/rangeborder-list.md) | <span data-ttu-id="b646f-116">Coleção [WorkbookRangeBorder](rangeborder.md)</span><span class="sxs-lookup"><span data-stu-id="b646f-116">[WorkbookRangeBorder](rangeborder.md) collection</span></span> |<span data-ttu-id="b646f-117">Obtenha a coleção de objetos rangeBorder.</span><span class="sxs-lookup"><span data-stu-id="b646f-117">Get rangeBorder object collection.</span></span> |
|[<span data-ttu-id="b646f-118">Itemat</span><span class="sxs-lookup"><span data-stu-id="b646f-118">Itemat</span></span>](../api/rangebordercollection-itemat.md)|[<span data-ttu-id="b646f-119">WorkbookRangeBorder</span><span class="sxs-lookup"><span data-stu-id="b646f-119">WorkbookRangeBorder</span></span>](rangeborder.md)|<span data-ttu-id="b646f-120">Obtém um objeto de borda usando seu índice.</span><span class="sxs-lookup"><span data-stu-id="b646f-120">Gets a border object using its index</span></span>|

## <a name="properties"></a><span data-ttu-id="b646f-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b646f-121">Properties</span></span>
| <span data-ttu-id="b646f-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b646f-122">Property</span></span>     | <span data-ttu-id="b646f-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="b646f-123">Type</span></span>   |<span data-ttu-id="b646f-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="b646f-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b646f-125">color</span><span class="sxs-lookup"><span data-stu-id="b646f-125">color</span></span>|<span data-ttu-id="b646f-126">string</span><span class="sxs-lookup"><span data-stu-id="b646f-126">string</span></span>|<span data-ttu-id="b646f-127">Código de cor HTML que representa a cor #RRGGBB da linha de borda do formulário (por exemplo, "FFA500") ou uma cor HTML nomeada (por exemplo, "laranja").</span><span class="sxs-lookup"><span data-stu-id="b646f-127">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange").</span></span>|
|<span data-ttu-id="b646f-128">id</span><span class="sxs-lookup"><span data-stu-id="b646f-128">id</span></span>|<span data-ttu-id="b646f-129">string</span><span class="sxs-lookup"><span data-stu-id="b646f-129">string</span></span>|<span data-ttu-id="b646f-130">Representa o identificador da borda.</span><span class="sxs-lookup"><span data-stu-id="b646f-130">Represents border identifier.</span></span> <span data-ttu-id="b646f-131">Os valores possíveis são: `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`, `DiagonalUp`.</span><span class="sxs-lookup"><span data-stu-id="b646f-131">The possible values are: `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`, `DiagonalUp`.</span></span> <span data-ttu-id="b646f-132">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b646f-132">Read-only.</span></span>|
|<span data-ttu-id="b646f-133">sideIndex</span><span class="sxs-lookup"><span data-stu-id="b646f-133">sideIndex</span></span>|<span data-ttu-id="b646f-134">string</span><span class="sxs-lookup"><span data-stu-id="b646f-134">string</span></span>|<span data-ttu-id="b646f-135">Valor constante que indica o lado específico da borda.</span><span class="sxs-lookup"><span data-stu-id="b646f-135">Constant value that indicates the specific side of the border.</span></span> <span data-ttu-id="b646f-136">Os valores possíveis são: `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`, `DiagonalUp`.</span><span class="sxs-lookup"><span data-stu-id="b646f-136">The possible values are: `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`, `DiagonalUp`.</span></span> <span data-ttu-id="b646f-137">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b646f-137">Read-only.</span></span>|
|<span data-ttu-id="b646f-138">style</span><span class="sxs-lookup"><span data-stu-id="b646f-138">style</span></span>|<span data-ttu-id="b646f-139">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b646f-139">string</span></span>|<span data-ttu-id="b646f-140">Uma das constantes de estilo de linha especificando o estilo de linha da borda.</span><span class="sxs-lookup"><span data-stu-id="b646f-140">One of the constants of line style specifying the line style for the border.</span></span> <span data-ttu-id="b646f-141">Os valores possíveis são: `None`, `Continuous`, `Dash`, `DashDot`, `DashDotDot`, `Dot`, `Double`, `SlantDashDot`.</span><span class="sxs-lookup"><span data-stu-id="b646f-141">The possible values are: `None`, `Continuous`, `Dash`, `DashDot`, `DashDotDot`, `Dot`, `Double`, `SlantDashDot`.</span></span>|
|<span data-ttu-id="b646f-142">weight</span><span class="sxs-lookup"><span data-stu-id="b646f-142">weight</span></span>|<span data-ttu-id="b646f-143">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b646f-143">string</span></span>|<span data-ttu-id="b646f-144">Especifica a espessura da borda em torno de um intervalo.</span><span class="sxs-lookup"><span data-stu-id="b646f-144">Specifies the weight of the border around a range.</span></span> <span data-ttu-id="b646f-145">Os valores possíveis são: `Hairline`, `Thin`, `Medium`, `Thick`.</span><span class="sxs-lookup"><span data-stu-id="b646f-145">The possible values are: `Hairline`, `Thin`, `Medium`, `Thick`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b646f-146">Relações</span><span class="sxs-lookup"><span data-stu-id="b646f-146">Relationships</span></span>
<span data-ttu-id="b646f-147">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b646f-147">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="b646f-148">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b646f-148">JSON representation</span></span>

<span data-ttu-id="b646f-149">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b646f-149">Here is a JSON representation of the resource.</span></span>

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
