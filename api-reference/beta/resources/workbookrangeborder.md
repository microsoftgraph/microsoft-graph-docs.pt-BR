---
title: tipo de recurso workbookRangeBorder
description: Representa a borda de um objeto.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 6b7bf53e74679a591c113f89c8744ff9c20a1211
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348498"
---
# <a name="workbookrangeborder-resource-type"></a><span data-ttu-id="acdaa-103">tipo de recurso workbookRangeBorder</span><span class="sxs-lookup"><span data-stu-id="acdaa-103">workbookRangeBorder resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="acdaa-104">Representa a borda de um objeto.</span><span class="sxs-lookup"><span data-stu-id="acdaa-104">Represents the border of an object.</span></span>


## <a name="methods"></a><span data-ttu-id="acdaa-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="acdaa-105">Methods</span></span>

| <span data-ttu-id="acdaa-106">Método</span><span class="sxs-lookup"><span data-stu-id="acdaa-106">Method</span></span>           | <span data-ttu-id="acdaa-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="acdaa-107">Return Type</span></span>    |<span data-ttu-id="acdaa-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="acdaa-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="acdaa-109">Obter workbookRangeBorder</span><span class="sxs-lookup"><span data-stu-id="acdaa-109">Get workbookRangeBorder</span></span>](../api/rangeborder-get.md) | [<span data-ttu-id="acdaa-110">workbookRangeBorder</span><span class="sxs-lookup"><span data-stu-id="acdaa-110">workbookRangeBorder</span></span>](workbookrangeborder.md) |<span data-ttu-id="acdaa-111">Leia as propriedades e relacionamentos do objeto rangeBorder.</span><span class="sxs-lookup"><span data-stu-id="acdaa-111">Read properties and relationships of rangeBorder object.</span></span>|
|[<span data-ttu-id="acdaa-112">Update</span><span class="sxs-lookup"><span data-stu-id="acdaa-112">Update</span></span>](../api/rangeborder-update.md) | [<span data-ttu-id="acdaa-113">workbookRangeBorder</span><span class="sxs-lookup"><span data-stu-id="acdaa-113">workbookRangeBorder</span></span>](workbookrangeborder.md) |<span data-ttu-id="acdaa-114">Atualize o objeto RangeBorder.</span><span class="sxs-lookup"><span data-stu-id="acdaa-114">Update RangeBorder object.</span></span> |
|[<span data-ttu-id="acdaa-115">List</span><span class="sxs-lookup"><span data-stu-id="acdaa-115">List</span></span>](../api/rangeborder-list.md) | <span data-ttu-id="acdaa-116">coleção [workbookRangeBorder](workbookrangeborder.md)</span><span class="sxs-lookup"><span data-stu-id="acdaa-116">[workbookRangeBorder](workbookrangeborder.md) collection</span></span> |<span data-ttu-id="acdaa-117">Obtenha a coleção de objetos rangeBorder.</span><span class="sxs-lookup"><span data-stu-id="acdaa-117">Get rangeBorder object collection.</span></span> |
|[<span data-ttu-id="acdaa-118">Itemat</span><span class="sxs-lookup"><span data-stu-id="acdaa-118">Itemat</span></span>](../api/rangebordercollection-itemat.md)|[<span data-ttu-id="acdaa-119">workbookRangeBorder</span><span class="sxs-lookup"><span data-stu-id="acdaa-119">workbookRangeBorder</span></span>](workbookrangeborder.md)|<span data-ttu-id="acdaa-120">Obtém um objeto de borda usando seu índice.</span><span class="sxs-lookup"><span data-stu-id="acdaa-120">Gets a border object using its index</span></span>|

## <a name="properties"></a><span data-ttu-id="acdaa-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="acdaa-121">Properties</span></span>
| <span data-ttu-id="acdaa-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="acdaa-122">Property</span></span>     | <span data-ttu-id="acdaa-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="acdaa-123">Type</span></span>   |<span data-ttu-id="acdaa-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="acdaa-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="acdaa-125">color</span><span class="sxs-lookup"><span data-stu-id="acdaa-125">color</span></span>|<span data-ttu-id="acdaa-126">string</span><span class="sxs-lookup"><span data-stu-id="acdaa-126">string</span></span>|<span data-ttu-id="acdaa-127">Código de cor HTML que representa a cor #RRGGBB da linha de borda do formulário (por exemplo, "FFA500") ou uma cor HTML nomeada (por exemplo, "laranja").</span><span class="sxs-lookup"><span data-stu-id="acdaa-127">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange").</span></span>|
|<span data-ttu-id="acdaa-128">id</span><span class="sxs-lookup"><span data-stu-id="acdaa-128">id</span></span>|<span data-ttu-id="acdaa-129">string</span><span class="sxs-lookup"><span data-stu-id="acdaa-129">string</span></span>|<span data-ttu-id="acdaa-p101">Representa o identificador da borda. Os valores possíveis são: `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown` e `DiagonalUp`. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="acdaa-p101">Represents border identifier. Possible values are: `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`, `DiagonalUp`. Read-only.</span></span>|
|<span data-ttu-id="acdaa-133">sideIndex</span><span class="sxs-lookup"><span data-stu-id="acdaa-133">sideIndex</span></span>|<span data-ttu-id="acdaa-134">string</span><span class="sxs-lookup"><span data-stu-id="acdaa-134">string</span></span>|<span data-ttu-id="acdaa-p102">Valor constante que indica o lado específico da borda. Os valores possíveis são: `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown` e `DiagonalUp`. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="acdaa-p102">Constant value that indicates the specific side of the border. Possible values are: `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`, `DiagonalUp`. Read-only.</span></span>|
|<span data-ttu-id="acdaa-138">style</span><span class="sxs-lookup"><span data-stu-id="acdaa-138">style</span></span>|<span data-ttu-id="acdaa-139">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="acdaa-139">string</span></span>|<span data-ttu-id="acdaa-p103">Uma das constantes de estilo de linha especificando o estilo de linha da borda. Os valores possíveis são: `None`, `Continuous`, `Dash`, `DashDot`, `DashDotDot`, `Dot`, `Double` e `SlantDashDot`.</span><span class="sxs-lookup"><span data-stu-id="acdaa-p103">One of the constants of line style specifying the line style for the border. Possible values are: `None`, `Continuous`, `Dash`, `DashDot`, `DashDotDot`, `Dot`, `Double`, `SlantDashDot`.</span></span>|
|<span data-ttu-id="acdaa-142">weight</span><span class="sxs-lookup"><span data-stu-id="acdaa-142">weight</span></span>|<span data-ttu-id="acdaa-143">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="acdaa-143">string</span></span>|<span data-ttu-id="acdaa-p104">Especifica a espessura da borda em torno de um intervalo. Os valores possíveis são: `Hairline`, `Thin`, `Medium` e `Thick`.</span><span class="sxs-lookup"><span data-stu-id="acdaa-p104">Specifies the weight of the border around a range. Possible values are: `Hairline`, `Thin`, `Medium`, `Thick`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="acdaa-146">Relações</span><span class="sxs-lookup"><span data-stu-id="acdaa-146">Relationships</span></span>
<span data-ttu-id="acdaa-147">Nenhum</span><span class="sxs-lookup"><span data-stu-id="acdaa-147">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="acdaa-148">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="acdaa-148">JSON representation</span></span>

<span data-ttu-id="acdaa-149">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="acdaa-149">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
<!--
{
  "type": "#page.annotation",
  "description": "RangeBorder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
