---
title: Tipo de recurso RangeBorder
description: Representa a borda de um objeto.
ms.openlocfilehash: ace494607d7e5803bf0ab0be5d5b3c86be875dcb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27040693"
---
# <a name="rangeborder-resource-type"></a><span data-ttu-id="cb2af-103">Tipo de recurso RangeBorder</span><span class="sxs-lookup"><span data-stu-id="cb2af-103">RangeBorder resource type</span></span>

> <span data-ttu-id="cb2af-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="cb2af-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cb2af-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="cb2af-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cb2af-106">Representa a borda de um objeto.</span><span class="sxs-lookup"><span data-stu-id="cb2af-106">Represents the border of an object.</span></span>


## <a name="methods"></a><span data-ttu-id="cb2af-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="cb2af-107">Methods</span></span>

| <span data-ttu-id="cb2af-108">Método</span><span class="sxs-lookup"><span data-stu-id="cb2af-108">Method</span></span>           | <span data-ttu-id="cb2af-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="cb2af-109">Return Type</span></span>    |<span data-ttu-id="cb2af-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="cb2af-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="cb2af-111">Get RangeBorder</span><span class="sxs-lookup"><span data-stu-id="cb2af-111">Get RangeBorder</span></span>](../api/rangeborder-get.md) | [<span data-ttu-id="cb2af-112">RangeBorder</span><span class="sxs-lookup"><span data-stu-id="cb2af-112">RangeBorder</span></span>](rangeborder.md) |<span data-ttu-id="cb2af-113">Leia as propriedades e relacionamentos do objeto rangeBorder.</span><span class="sxs-lookup"><span data-stu-id="cb2af-113">Read properties and relationships of rangeBorder object.</span></span>|
|[<span data-ttu-id="cb2af-114">Update</span><span class="sxs-lookup"><span data-stu-id="cb2af-114">Update</span></span>](../api/rangeborder-update.md) | [<span data-ttu-id="cb2af-115">RangeBorder</span><span class="sxs-lookup"><span data-stu-id="cb2af-115">RangeBorder</span></span>](rangeborder.md) |<span data-ttu-id="cb2af-116">Atualize o objeto RangeBorder.</span><span class="sxs-lookup"><span data-stu-id="cb2af-116">Update RangeBorder object.</span></span> |
|[<span data-ttu-id="cb2af-117">List</span><span class="sxs-lookup"><span data-stu-id="cb2af-117">List</span></span>](../api/rangeborder-list.md) | <span data-ttu-id="cb2af-118">Coleção [RangeBorder](rangeborder.md)</span><span class="sxs-lookup"><span data-stu-id="cb2af-118">[RangeBorder](rangeborder.md) collection</span></span> |<span data-ttu-id="cb2af-119">Obtenha a coleção de objetos rangeBorder.</span><span class="sxs-lookup"><span data-stu-id="cb2af-119">Get rangeBorder object collection.</span></span> |
|[<span data-ttu-id="cb2af-120">Itemat</span><span class="sxs-lookup"><span data-stu-id="cb2af-120">Itemat</span></span>](../api/rangebordercollection-itemat.md)|[<span data-ttu-id="cb2af-121">RangeBorder</span><span class="sxs-lookup"><span data-stu-id="cb2af-121">RangeBorder</span></span>](rangeborder.md)|<span data-ttu-id="cb2af-122">Obtém um objeto de borda usando seu índice.</span><span class="sxs-lookup"><span data-stu-id="cb2af-122">Gets a border object using its index</span></span>|

## <a name="properties"></a><span data-ttu-id="cb2af-123">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cb2af-123">Properties</span></span>
| <span data-ttu-id="cb2af-124">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cb2af-124">Property</span></span>     | <span data-ttu-id="cb2af-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="cb2af-125">Type</span></span>   |<span data-ttu-id="cb2af-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="cb2af-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cb2af-127">color</span><span class="sxs-lookup"><span data-stu-id="cb2af-127">color</span></span>|<span data-ttu-id="cb2af-128">string</span><span class="sxs-lookup"><span data-stu-id="cb2af-128">string</span></span>|<span data-ttu-id="cb2af-129">Código de cor HTML que representa a cor #RRGGBB da linha de borda do formulário (por exemplo, "FFA500") ou uma cor HTML nomeada (por exemplo, "laranja").</span><span class="sxs-lookup"><span data-stu-id="cb2af-129">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange").</span></span>|
|<span data-ttu-id="cb2af-130">id</span><span class="sxs-lookup"><span data-stu-id="cb2af-130">id</span></span>|<span data-ttu-id="cb2af-131">string</span><span class="sxs-lookup"><span data-stu-id="cb2af-131">string</span></span>|<span data-ttu-id="cb2af-p102">Representa o identificador da borda. Os valores possíveis são: `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown` e `DiagonalUp`. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cb2af-p102">Represents border identifier. Possible values are: `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`, `DiagonalUp`. Read-only.</span></span>|
|<span data-ttu-id="cb2af-135">sideIndex</span><span class="sxs-lookup"><span data-stu-id="cb2af-135">sideIndex</span></span>|<span data-ttu-id="cb2af-136">string</span><span class="sxs-lookup"><span data-stu-id="cb2af-136">string</span></span>|<span data-ttu-id="cb2af-p103">Valor constante que indica o lado específico da borda. Os valores possíveis são: `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown` e `DiagonalUp`. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cb2af-p103">Constant value that indicates the specific side of the border. Possible values are: `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`, `DiagonalUp`. Read-only.</span></span>|
|<span data-ttu-id="cb2af-140">estilo</span><span class="sxs-lookup"><span data-stu-id="cb2af-140">style</span></span>|<span data-ttu-id="cb2af-141">string</span><span class="sxs-lookup"><span data-stu-id="cb2af-141">string</span></span>|<span data-ttu-id="cb2af-p104">Uma das constantes de estilo de linha especificando o estilo de linha da borda. Os valores possíveis são: `None`, `Continuous`, `Dash`, `DashDot`, `DashDotDot`, `Dot`, `Double` e `SlantDashDot`.</span><span class="sxs-lookup"><span data-stu-id="cb2af-p104">One of the constants of line style specifying the line style for the border. Possible values are: `None`, `Continuous`, `Dash`, `DashDot`, `DashDotDot`, `Dot`, `Double`, `SlantDashDot`.</span></span>|
|<span data-ttu-id="cb2af-144">weight</span><span class="sxs-lookup"><span data-stu-id="cb2af-144">weight</span></span>|<span data-ttu-id="cb2af-145">string</span><span class="sxs-lookup"><span data-stu-id="cb2af-145">string</span></span>|<span data-ttu-id="cb2af-p105">Especifica a espessura da borda em torno de um intervalo. Os valores possíveis são: `Hairline`, `Thin`, `Medium` e `Thick`.</span><span class="sxs-lookup"><span data-stu-id="cb2af-p105">Specifies the weight of the border around a range. Possible values are: `Hairline`, `Thin`, `Medium`, `Thick`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cb2af-148">Relações</span><span class="sxs-lookup"><span data-stu-id="cb2af-148">Relationships</span></span>
<span data-ttu-id="cb2af-149">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cb2af-149">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="cb2af-150">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cb2af-150">JSON representation</span></span>

<span data-ttu-id="cb2af-151">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cb2af-151">Here is a JSON representation of the resource.</span></span>

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