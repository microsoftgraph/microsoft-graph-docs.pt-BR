---
title: Tipo de recurso Icon
description: Representa um ícone de célula.
localization_priority: Normal
ms.openlocfilehash: c15ee02d1c6830cbb5246826665d0353b7e999b9
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516298"
---
# <a name="icon-resource-type"></a><span data-ttu-id="950ec-103">Tipo de recurso Icon</span><span class="sxs-lookup"><span data-stu-id="950ec-103">Icon resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="950ec-104">Representa um ícone de célula.</span><span class="sxs-lookup"><span data-stu-id="950ec-104">Represents a cell icon.</span></span>


## <a name="methods"></a><span data-ttu-id="950ec-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="950ec-105">Methods</span></span>

| <span data-ttu-id="950ec-106">Método</span><span class="sxs-lookup"><span data-stu-id="950ec-106">Method</span></span>           | <span data-ttu-id="950ec-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="950ec-107">Return Type</span></span>    |<span data-ttu-id="950ec-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="950ec-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="950ec-109">Get Icon</span><span class="sxs-lookup"><span data-stu-id="950ec-109">[Get Icon](../api/icon-get.md)</span></span> | [<span data-ttu-id="950ec-110">Icon</span><span class="sxs-lookup"><span data-stu-id="950ec-110">Icon</span></span>](icon.md) |<span data-ttu-id="950ec-111">Leia as propriedades e os relacionamentos do objeto de ícone.</span><span class="sxs-lookup"><span data-stu-id="950ec-111">Read properties and relationships of icon object.</span></span>|
|[<span data-ttu-id="950ec-112">Update</span><span class="sxs-lookup"><span data-stu-id="950ec-112">Update</span></span>](../api/icon-update.md) | [<span data-ttu-id="950ec-113">Icon</span><span class="sxs-lookup"><span data-stu-id="950ec-113">Icon</span></span>](icon.md)  |<span data-ttu-id="950ec-114">Atualize o objeto Icon.</span><span class="sxs-lookup"><span data-stu-id="950ec-114">Update Icon object.</span></span> |

## <a name="properties"></a><span data-ttu-id="950ec-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="950ec-115">Properties</span></span>
| <span data-ttu-id="950ec-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="950ec-116">Property</span></span>     | <span data-ttu-id="950ec-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="950ec-117">Type</span></span>   |<span data-ttu-id="950ec-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="950ec-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="950ec-119">índice</span><span class="sxs-lookup"><span data-stu-id="950ec-119">index</span></span>|<span data-ttu-id="950ec-120">int</span><span class="sxs-lookup"><span data-stu-id="950ec-120">int</span></span>|<span data-ttu-id="950ec-121">Representa o índice do ícone em determinado conjunto.</span><span class="sxs-lookup"><span data-stu-id="950ec-121">Represents the index of the icon in the given set.</span></span>|
|<span data-ttu-id="950ec-122">set</span><span class="sxs-lookup"><span data-stu-id="950ec-122">set</span></span>|<span data-ttu-id="950ec-123">string</span><span class="sxs-lookup"><span data-stu-id="950ec-123">string</span></span>|<span data-ttu-id="950ec-p101">Representa o conjunto do qual o ícone faz parte. Os valores possíveis são: `Invalid`, `ThreeArrows`, `ThreeArrowsGray`, `ThreeFlags`, `ThreeTrafficLights1`, `ThreeTrafficLights2`, `ThreeSigns`, `ThreeSymbols`, `ThreeSymbols2`, `FourArrows`, `FourArrowsGray`, `FourRedToBlack`, `FourRating`, `FourTrafficLights`, `FiveArrows`, `FiveArrowsGray`, `FiveRating`, `FiveQuarters`, `ThreeStars`, `ThreeTriangles` e `FiveBoxes`.</span><span class="sxs-lookup"><span data-stu-id="950ec-p101">Represents the set that the icon is part of. Possible values are: `Invalid`, `ThreeArrows`, `ThreeArrowsGray`, `ThreeFlags`, `ThreeTrafficLights1`, `ThreeTrafficLights2`, `ThreeSigns`, `ThreeSymbols`, `ThreeSymbols2`, `FourArrows`, `FourArrowsGray`, `FourRedToBlack`, `FourRating`, `FourTrafficLights`, `FiveArrows`, `FiveArrowsGray`, `FiveRating`, `FiveQuarters`, `ThreeStars`, `ThreeTriangles`, `FiveBoxes`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="950ec-126">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="950ec-126">Relationships</span></span>
<span data-ttu-id="950ec-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="950ec-127">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="950ec-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="950ec-128">JSON representation</span></span>

<span data-ttu-id="950ec-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="950ec-129">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.icon"
}-->

```json
{
  "index": 1024,
  "set": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Icon resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/icon.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
