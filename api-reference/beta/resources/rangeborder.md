---
title: Tipo de recurso RangeBorder
description: Representa a borda de um objeto.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 5b3b814da53013d1daca686d549596a7ab656027
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515381"
---
# <a name="rangeborder-resource-type"></a><span data-ttu-id="2b187-103">Tipo de recurso RangeBorder</span><span class="sxs-lookup"><span data-stu-id="2b187-103">RangeBorder resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2b187-104">Representa a borda de um objeto.</span><span class="sxs-lookup"><span data-stu-id="2b187-104">Represents the border of an object.</span></span>


## <a name="methods"></a><span data-ttu-id="2b187-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="2b187-105">Methods</span></span>

| <span data-ttu-id="2b187-106">Método</span><span class="sxs-lookup"><span data-stu-id="2b187-106">Method</span></span>           | <span data-ttu-id="2b187-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="2b187-107">Return Type</span></span>    |<span data-ttu-id="2b187-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="2b187-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2b187-109">Get RangeBorder</span><span class="sxs-lookup"><span data-stu-id="2b187-109">[Get RangeBorder](../api/rangeborder-get.md)</span></span> | <span data-ttu-id="2b187-110">RangeBorder</span><span class="sxs-lookup"><span data-stu-id="2b187-110">[RangeBorder](rangeborder.md)</span></span> |<span data-ttu-id="2b187-111">Leia as propriedades e relacionamentos do objeto rangeBorder.</span><span class="sxs-lookup"><span data-stu-id="2b187-111">Read properties and relationships of rangeBorder object.</span></span>|
|[<span data-ttu-id="2b187-112">Update</span><span class="sxs-lookup"><span data-stu-id="2b187-112">Update</span></span>](../api/rangeborder-update.md) | <span data-ttu-id="2b187-113">RangeBorder</span><span class="sxs-lookup"><span data-stu-id="2b187-113">[RangeBorder](rangeborder.md)</span></span> |<span data-ttu-id="2b187-114">Atualize o objeto RangeBorder.</span><span class="sxs-lookup"><span data-stu-id="2b187-114">Update RangeBorder object.</span></span> |
|[<span data-ttu-id="2b187-115">List</span><span class="sxs-lookup"><span data-stu-id="2b187-115">List</span></span>](../api/rangeborder-list.md) | <span data-ttu-id="2b187-116">Coleção RangeBorder</span><span class="sxs-lookup"><span data-stu-id="2b187-116">[RangeBorder](rangeborder.md) collection</span></span> |<span data-ttu-id="2b187-117">Obtenha a coleção de objetos rangeBorder.</span><span class="sxs-lookup"><span data-stu-id="2b187-117">Get rangeBorder object collection.</span></span> |
|[<span data-ttu-id="2b187-118">Itemat</span><span class="sxs-lookup"><span data-stu-id="2b187-118">Itemat</span></span>](../api/rangebordercollection-itemat.md)|<span data-ttu-id="2b187-119">RangeBorder</span><span class="sxs-lookup"><span data-stu-id="2b187-119">[RangeBorder](rangeborder.md)</span></span>|<span data-ttu-id="2b187-120">Obtém um objeto de borda usando seu índice.</span><span class="sxs-lookup"><span data-stu-id="2b187-120">Gets a border object using its index</span></span>|

## <a name="properties"></a><span data-ttu-id="2b187-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2b187-121">Properties</span></span>
| <span data-ttu-id="2b187-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2b187-122">Property</span></span>     | <span data-ttu-id="2b187-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="2b187-123">Type</span></span>   |<span data-ttu-id="2b187-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="2b187-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2b187-125">color</span><span class="sxs-lookup"><span data-stu-id="2b187-125">color</span></span>|<span data-ttu-id="2b187-126">string</span><span class="sxs-lookup"><span data-stu-id="2b187-126">string</span></span>|<span data-ttu-id="2b187-127">Código de cor HTML que representa a cor #RRGGBB da linha de borda do formulário (por exemplo, "FFA500") ou uma cor HTML nomeada (por exemplo, "laranja").</span><span class="sxs-lookup"><span data-stu-id="2b187-127">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange").</span></span>|
|<span data-ttu-id="2b187-128">id</span><span class="sxs-lookup"><span data-stu-id="2b187-128">id</span></span>|<span data-ttu-id="2b187-129">string</span><span class="sxs-lookup"><span data-stu-id="2b187-129">string</span></span>|<span data-ttu-id="2b187-p101">Representa o identificador da borda. Os valores possíveis são: `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown` e `DiagonalUp`. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2b187-p101">Represents border identifier. Possible values are: `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`, `DiagonalUp`. Read-only.</span></span>|
|<span data-ttu-id="2b187-133">sideIndex</span><span class="sxs-lookup"><span data-stu-id="2b187-133">sideIndex</span></span>|<span data-ttu-id="2b187-134">string</span><span class="sxs-lookup"><span data-stu-id="2b187-134">string</span></span>|<span data-ttu-id="2b187-p102">Valor constante que indica o lado específico da borda. Os valores possíveis são: `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown` e `DiagonalUp`. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2b187-p102">Constant value that indicates the specific side of the border. Possible values are: `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`, `DiagonalUp`. Read-only.</span></span>|
|<span data-ttu-id="2b187-138">estilo</span><span class="sxs-lookup"><span data-stu-id="2b187-138">style</span></span>|<span data-ttu-id="2b187-139">string</span><span class="sxs-lookup"><span data-stu-id="2b187-139">string</span></span>|<span data-ttu-id="2b187-p103">Uma das constantes de estilo de linha especificando o estilo de linha da borda. Os valores possíveis são: `None`, `Continuous`, `Dash`, `DashDot`, `DashDotDot`, `Dot`, `Double` e `SlantDashDot`.</span><span class="sxs-lookup"><span data-stu-id="2b187-p103">One of the constants of line style specifying the line style for the border. Possible values are: `None`, `Continuous`, `Dash`, `DashDot`, `DashDotDot`, `Dot`, `Double`, `SlantDashDot`.</span></span>|
|<span data-ttu-id="2b187-142">weight</span><span class="sxs-lookup"><span data-stu-id="2b187-142">weight</span></span>|<span data-ttu-id="2b187-143">string</span><span class="sxs-lookup"><span data-stu-id="2b187-143">string</span></span>|<span data-ttu-id="2b187-p104">Especifica a espessura da borda em torno de um intervalo. Os valores possíveis são: `Hairline`, `Thin`, `Medium` e `Thick`.</span><span class="sxs-lookup"><span data-stu-id="2b187-p104">Specifies the weight of the border around a range. Possible values are: `Hairline`, `Thin`, `Medium`, `Thick`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2b187-146">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="2b187-146">Relationships</span></span>
<span data-ttu-id="2b187-147">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2b187-147">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="2b187-148">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2b187-148">JSON representation</span></span>

<span data-ttu-id="2b187-149">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2b187-149">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "RangeBorder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/rangeborder.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
