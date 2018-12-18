---
title: Tipo de recurso RangeBorder
description: Representa a borda de um objeto.
author: lumine2008
ms.openlocfilehash: 2aa8807949724766930c5938d1ee6e06db98212a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27301215"
---
# <a name="rangeborder-resource-type"></a><span data-ttu-id="061a3-103">Tipo de recurso RangeBorder</span><span class="sxs-lookup"><span data-stu-id="061a3-103">RangeBorder resource type</span></span>

> <span data-ttu-id="061a3-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="061a3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="061a3-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="061a3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="061a3-106">Representa a borda de um objeto.</span><span class="sxs-lookup"><span data-stu-id="061a3-106">Represents the border of an object.</span></span>


## <a name="methods"></a><span data-ttu-id="061a3-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="061a3-107">Methods</span></span>

| <span data-ttu-id="061a3-108">Método</span><span class="sxs-lookup"><span data-stu-id="061a3-108">Method</span></span>           | <span data-ttu-id="061a3-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="061a3-109">Return Type</span></span>    |<span data-ttu-id="061a3-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="061a3-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="061a3-111">Get RangeBorder</span><span class="sxs-lookup"><span data-stu-id="061a3-111">Get RangeBorder</span></span>](../api/rangeborder-get.md) | [<span data-ttu-id="061a3-112">RangeBorder</span><span class="sxs-lookup"><span data-stu-id="061a3-112">RangeBorder</span></span>](rangeborder.md) |<span data-ttu-id="061a3-113">Leia as propriedades e relacionamentos do objeto rangeBorder.</span><span class="sxs-lookup"><span data-stu-id="061a3-113">Read properties and relationships of rangeBorder object.</span></span>|
|[<span data-ttu-id="061a3-114">Update</span><span class="sxs-lookup"><span data-stu-id="061a3-114">Update</span></span>](../api/rangeborder-update.md) | [<span data-ttu-id="061a3-115">RangeBorder</span><span class="sxs-lookup"><span data-stu-id="061a3-115">RangeBorder</span></span>](rangeborder.md) |<span data-ttu-id="061a3-116">Atualize o objeto RangeBorder.</span><span class="sxs-lookup"><span data-stu-id="061a3-116">Update RangeBorder object.</span></span> |
|[<span data-ttu-id="061a3-117">List</span><span class="sxs-lookup"><span data-stu-id="061a3-117">List</span></span>](../api/rangeborder-list.md) | <span data-ttu-id="061a3-118">Coleção [RangeBorder](rangeborder.md)</span><span class="sxs-lookup"><span data-stu-id="061a3-118">[RangeBorder](rangeborder.md) collection</span></span> |<span data-ttu-id="061a3-119">Obtenha a coleção de objetos rangeBorder.</span><span class="sxs-lookup"><span data-stu-id="061a3-119">Get rangeBorder object collection.</span></span> |
|[<span data-ttu-id="061a3-120">Itemat</span><span class="sxs-lookup"><span data-stu-id="061a3-120">Itemat</span></span>](../api/rangebordercollection-itemat.md)|[<span data-ttu-id="061a3-121">RangeBorder</span><span class="sxs-lookup"><span data-stu-id="061a3-121">RangeBorder</span></span>](rangeborder.md)|<span data-ttu-id="061a3-122">Obtém um objeto de borda usando seu índice.</span><span class="sxs-lookup"><span data-stu-id="061a3-122">Gets a border object using its index</span></span>|

## <a name="properties"></a><span data-ttu-id="061a3-123">Propriedades</span><span class="sxs-lookup"><span data-stu-id="061a3-123">Properties</span></span>
| <span data-ttu-id="061a3-124">Propriedade</span><span class="sxs-lookup"><span data-stu-id="061a3-124">Property</span></span>     | <span data-ttu-id="061a3-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="061a3-125">Type</span></span>   |<span data-ttu-id="061a3-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="061a3-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="061a3-127">color</span><span class="sxs-lookup"><span data-stu-id="061a3-127">color</span></span>|<span data-ttu-id="061a3-128">string</span><span class="sxs-lookup"><span data-stu-id="061a3-128">string</span></span>|<span data-ttu-id="061a3-129">Código de cor HTML que representa a cor #RRGGBB da linha de borda do formulário (por exemplo, "FFA500") ou uma cor HTML nomeada (por exemplo, "laranja").</span><span class="sxs-lookup"><span data-stu-id="061a3-129">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange").</span></span>|
|<span data-ttu-id="061a3-130">id</span><span class="sxs-lookup"><span data-stu-id="061a3-130">id</span></span>|<span data-ttu-id="061a3-131">string</span><span class="sxs-lookup"><span data-stu-id="061a3-131">string</span></span>|<span data-ttu-id="061a3-p102">Representa o identificador da borda. Os valores possíveis são: `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown` e `DiagonalUp`. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="061a3-p102">Represents border identifier. Possible values are: `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`, `DiagonalUp`. Read-only.</span></span>|
|<span data-ttu-id="061a3-135">sideIndex</span><span class="sxs-lookup"><span data-stu-id="061a3-135">sideIndex</span></span>|<span data-ttu-id="061a3-136">string</span><span class="sxs-lookup"><span data-stu-id="061a3-136">string</span></span>|<span data-ttu-id="061a3-p103">Valor constante que indica o lado específico da borda. Os valores possíveis são: `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown` e `DiagonalUp`. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="061a3-p103">Constant value that indicates the specific side of the border. Possible values are: `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`, `DiagonalUp`. Read-only.</span></span>|
|<span data-ttu-id="061a3-140">style</span><span class="sxs-lookup"><span data-stu-id="061a3-140">style</span></span>|<span data-ttu-id="061a3-141">string</span><span class="sxs-lookup"><span data-stu-id="061a3-141">string</span></span>|<span data-ttu-id="061a3-p104">Uma das constantes de estilo de linha especificando o estilo de linha da borda. Os valores possíveis são: `None`, `Continuous`, `Dash`, `DashDot`, `DashDotDot`, `Dot`, `Double` e `SlantDashDot`.</span><span class="sxs-lookup"><span data-stu-id="061a3-p104">One of the constants of line style specifying the line style for the border. Possible values are: `None`, `Continuous`, `Dash`, `DashDot`, `DashDotDot`, `Dot`, `Double`, `SlantDashDot`.</span></span>|
|<span data-ttu-id="061a3-144">weight</span><span class="sxs-lookup"><span data-stu-id="061a3-144">weight</span></span>|<span data-ttu-id="061a3-145">string</span><span class="sxs-lookup"><span data-stu-id="061a3-145">string</span></span>|<span data-ttu-id="061a3-p105">Especifica a espessura da borda em torno de um intervalo. Os valores possíveis são: `Hairline`, `Thin`, `Medium` e `Thick`.</span><span class="sxs-lookup"><span data-stu-id="061a3-p105">Specifies the weight of the border around a range. Possible values are: `Hairline`, `Thin`, `Medium`, `Thick`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="061a3-148">Relações</span><span class="sxs-lookup"><span data-stu-id="061a3-148">Relationships</span></span>
<span data-ttu-id="061a3-149">Nenhum</span><span class="sxs-lookup"><span data-stu-id="061a3-149">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="061a3-150">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="061a3-150">JSON representation</span></span>

<span data-ttu-id="061a3-151">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="061a3-151">Here is a JSON representation of the resource.</span></span>

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