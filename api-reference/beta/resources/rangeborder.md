---
title: Tipo de recurso RangeBorder
description: Representa a borda de um objeto.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 8404a45ea7c56bbbb318994daa55229706d700a2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27960235"
---
# <a name="rangeborder-resource-type"></a><span data-ttu-id="0c5b8-103">Tipo de recurso RangeBorder</span><span class="sxs-lookup"><span data-stu-id="0c5b8-103">RangeBorder resource type</span></span>

> <span data-ttu-id="0c5b8-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="0c5b8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0c5b8-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="0c5b8-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0c5b8-106">Representa a borda de um objeto.</span><span class="sxs-lookup"><span data-stu-id="0c5b8-106">Represents the border of an object.</span></span>


## <a name="methods"></a><span data-ttu-id="0c5b8-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="0c5b8-107">Methods</span></span>

| <span data-ttu-id="0c5b8-108">Método</span><span class="sxs-lookup"><span data-stu-id="0c5b8-108">Method</span></span>           | <span data-ttu-id="0c5b8-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="0c5b8-109">Return Type</span></span>    |<span data-ttu-id="0c5b8-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="0c5b8-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0c5b8-111">Get RangeBorder</span><span class="sxs-lookup"><span data-stu-id="0c5b8-111">Get RangeBorder</span></span>](../api/rangeborder-get.md) | [<span data-ttu-id="0c5b8-112">RangeBorder</span><span class="sxs-lookup"><span data-stu-id="0c5b8-112">RangeBorder</span></span>](rangeborder.md) |<span data-ttu-id="0c5b8-113">Leia as propriedades e relacionamentos do objeto rangeBorder.</span><span class="sxs-lookup"><span data-stu-id="0c5b8-113">Read properties and relationships of rangeBorder object.</span></span>|
|[<span data-ttu-id="0c5b8-114">Update</span><span class="sxs-lookup"><span data-stu-id="0c5b8-114">Update</span></span>](../api/rangeborder-update.md) | [<span data-ttu-id="0c5b8-115">RangeBorder</span><span class="sxs-lookup"><span data-stu-id="0c5b8-115">RangeBorder</span></span>](rangeborder.md) |<span data-ttu-id="0c5b8-116">Atualize o objeto RangeBorder.</span><span class="sxs-lookup"><span data-stu-id="0c5b8-116">Update RangeBorder object.</span></span> |
|[<span data-ttu-id="0c5b8-117">List</span><span class="sxs-lookup"><span data-stu-id="0c5b8-117">List</span></span>](../api/rangeborder-list.md) | <span data-ttu-id="0c5b8-118">Coleção [RangeBorder](rangeborder.md)</span><span class="sxs-lookup"><span data-stu-id="0c5b8-118">[RangeBorder](rangeborder.md) collection</span></span> |<span data-ttu-id="0c5b8-119">Obtenha a coleção de objetos rangeBorder.</span><span class="sxs-lookup"><span data-stu-id="0c5b8-119">Get rangeBorder object collection.</span></span> |
|[<span data-ttu-id="0c5b8-120">Itemat</span><span class="sxs-lookup"><span data-stu-id="0c5b8-120">Itemat</span></span>](../api/rangebordercollection-itemat.md)|[<span data-ttu-id="0c5b8-121">RangeBorder</span><span class="sxs-lookup"><span data-stu-id="0c5b8-121">RangeBorder</span></span>](rangeborder.md)|<span data-ttu-id="0c5b8-122">Obtém um objeto de borda usando seu índice.</span><span class="sxs-lookup"><span data-stu-id="0c5b8-122">Gets a border object using its index</span></span>|

## <a name="properties"></a><span data-ttu-id="0c5b8-123">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0c5b8-123">Properties</span></span>
| <span data-ttu-id="0c5b8-124">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0c5b8-124">Property</span></span>     | <span data-ttu-id="0c5b8-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="0c5b8-125">Type</span></span>   |<span data-ttu-id="0c5b8-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="0c5b8-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0c5b8-127">color</span><span class="sxs-lookup"><span data-stu-id="0c5b8-127">color</span></span>|<span data-ttu-id="0c5b8-128">string</span><span class="sxs-lookup"><span data-stu-id="0c5b8-128">string</span></span>|<span data-ttu-id="0c5b8-129">Código de cor HTML que representa a cor #RRGGBB da linha de borda do formulário (por exemplo, "FFA500") ou uma cor HTML nomeada (por exemplo, "laranja").</span><span class="sxs-lookup"><span data-stu-id="0c5b8-129">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange").</span></span>|
|<span data-ttu-id="0c5b8-130">id</span><span class="sxs-lookup"><span data-stu-id="0c5b8-130">id</span></span>|<span data-ttu-id="0c5b8-131">string</span><span class="sxs-lookup"><span data-stu-id="0c5b8-131">string</span></span>|<span data-ttu-id="0c5b8-p102">Representa o identificador da borda. Os valores possíveis são: `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown` e `DiagonalUp`. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0c5b8-p102">Represents border identifier. Possible values are: `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`, `DiagonalUp`. Read-only.</span></span>|
|<span data-ttu-id="0c5b8-135">sideIndex</span><span class="sxs-lookup"><span data-stu-id="0c5b8-135">sideIndex</span></span>|<span data-ttu-id="0c5b8-136">string</span><span class="sxs-lookup"><span data-stu-id="0c5b8-136">string</span></span>|<span data-ttu-id="0c5b8-p103">Valor constante que indica o lado específico da borda. Os valores possíveis são: `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown` e `DiagonalUp`. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0c5b8-p103">Constant value that indicates the specific side of the border. Possible values are: `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`, `DiagonalUp`. Read-only.</span></span>|
|<span data-ttu-id="0c5b8-140">style</span><span class="sxs-lookup"><span data-stu-id="0c5b8-140">style</span></span>|<span data-ttu-id="0c5b8-141">string</span><span class="sxs-lookup"><span data-stu-id="0c5b8-141">string</span></span>|<span data-ttu-id="0c5b8-p104">Uma das constantes de estilo de linha especificando o estilo de linha da borda. Os valores possíveis são: `None`, `Continuous`, `Dash`, `DashDot`, `DashDotDot`, `Dot`, `Double` e `SlantDashDot`.</span><span class="sxs-lookup"><span data-stu-id="0c5b8-p104">One of the constants of line style specifying the line style for the border. Possible values are: `None`, `Continuous`, `Dash`, `DashDot`, `DashDotDot`, `Dot`, `Double`, `SlantDashDot`.</span></span>|
|<span data-ttu-id="0c5b8-144">weight</span><span class="sxs-lookup"><span data-stu-id="0c5b8-144">weight</span></span>|<span data-ttu-id="0c5b8-145">string</span><span class="sxs-lookup"><span data-stu-id="0c5b8-145">string</span></span>|<span data-ttu-id="0c5b8-p105">Especifica a espessura da borda em torno de um intervalo. Os valores possíveis são: `Hairline`, `Thin`, `Medium` e `Thick`.</span><span class="sxs-lookup"><span data-stu-id="0c5b8-p105">Specifies the weight of the border around a range. Possible values are: `Hairline`, `Thin`, `Medium`, `Thick`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0c5b8-148">Relações</span><span class="sxs-lookup"><span data-stu-id="0c5b8-148">Relationships</span></span>
<span data-ttu-id="0c5b8-149">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0c5b8-149">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="0c5b8-150">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0c5b8-150">JSON representation</span></span>

<span data-ttu-id="0c5b8-151">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0c5b8-151">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.rangeBorder"
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
