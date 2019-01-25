---
title: Tipo de recurso SortField
description: Representa uma condição em uma operação de classificação.
localization_priority: Normal
ms.openlocfilehash: 52817df89ed130b6984ae3a76da775e0e000dee5
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521632"
---
# <a name="sortfield-resource-type"></a><span data-ttu-id="7f0dc-103">Tipo de recurso SortField</span><span class="sxs-lookup"><span data-stu-id="7f0dc-103">SortField resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7f0dc-104">Representa uma condição em uma operação de classificação.</span><span class="sxs-lookup"><span data-stu-id="7f0dc-104">Represents a condition in a sorting operation.</span></span>

## <a name="properties"></a><span data-ttu-id="7f0dc-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7f0dc-105">Properties</span></span>
| <span data-ttu-id="7f0dc-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7f0dc-106">Property</span></span>     | <span data-ttu-id="7f0dc-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="7f0dc-107">Type</span></span>   |<span data-ttu-id="7f0dc-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="7f0dc-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7f0dc-109">ascending</span><span class="sxs-lookup"><span data-stu-id="7f0dc-109">ascending</span></span>|<span data-ttu-id="7f0dc-110">booliano</span><span class="sxs-lookup"><span data-stu-id="7f0dc-110">boolean</span></span>|<span data-ttu-id="7f0dc-111">Indica se a classificação é feita de forma crescente.</span><span class="sxs-lookup"><span data-stu-id="7f0dc-111">Represents whether the sorting is done in an ascending fashion.</span></span>|
|<span data-ttu-id="7f0dc-112">color</span><span class="sxs-lookup"><span data-stu-id="7f0dc-112">color</span></span>|<span data-ttu-id="7f0dc-113">string</span><span class="sxs-lookup"><span data-stu-id="7f0dc-113">string</span></span>|<span data-ttu-id="7f0dc-114">Representa a cor que é o destino da condição se a classificação estiver na cor da fonte ou da célula.</span><span class="sxs-lookup"><span data-stu-id="7f0dc-114">Represents the color that is the target of the condition if the sorting is on font or cell color.</span></span>|
|<span data-ttu-id="7f0dc-115">dataOption</span><span class="sxs-lookup"><span data-stu-id="7f0dc-115">dataOption</span></span>|<span data-ttu-id="7f0dc-116">string</span><span class="sxs-lookup"><span data-stu-id="7f0dc-116">string</span></span>|<span data-ttu-id="7f0dc-p101">Representa as opções de classificação adicionais para esse campo. Os valores possíveis são: `Normal` e `TextAsNumber`.</span><span class="sxs-lookup"><span data-stu-id="7f0dc-p101">Represents additional sorting options for this field. Possible values are: `Normal`, `TextAsNumber`.</span></span>|
|<span data-ttu-id="7f0dc-119">key</span><span class="sxs-lookup"><span data-stu-id="7f0dc-119">key</span></span>|<span data-ttu-id="7f0dc-120">int</span><span class="sxs-lookup"><span data-stu-id="7f0dc-120">int</span></span>|<span data-ttu-id="7f0dc-p102">Representa a coluna (ou linha, dependendo da orientação da classificação) em que a condição está. Representado como um deslocamento da primeira coluna (ou linha).</span><span class="sxs-lookup"><span data-stu-id="7f0dc-p102">Represents the column (or row, depending on the sort orientation) that the condition is on. Represented as an offset from the first column (or row).</span></span>|
|<span data-ttu-id="7f0dc-123">sortOn</span><span class="sxs-lookup"><span data-stu-id="7f0dc-123">sortOn</span></span>|<span data-ttu-id="7f0dc-124">string</span><span class="sxs-lookup"><span data-stu-id="7f0dc-124">string</span></span>|<span data-ttu-id="7f0dc-p103">Representa o tipo de classificação dessa condição. Os valores possíveis são: `Value`, `CellColor`, `FontColor` e `Icon`.</span><span class="sxs-lookup"><span data-stu-id="7f0dc-p103">Represents the type of sorting of this condition. Possible values are: `Value`, `CellColor`, `FontColor`, `Icon`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7f0dc-127">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="7f0dc-127">Relationships</span></span>
| <span data-ttu-id="7f0dc-128">Relação</span><span class="sxs-lookup"><span data-stu-id="7f0dc-128">Relationship</span></span> | <span data-ttu-id="7f0dc-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="7f0dc-129">Type</span></span>   |<span data-ttu-id="7f0dc-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="7f0dc-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7f0dc-131">ícone</span><span class="sxs-lookup"><span data-stu-id="7f0dc-131">icon</span></span>|[<span data-ttu-id="7f0dc-132">Icon</span><span class="sxs-lookup"><span data-stu-id="7f0dc-132">Icon</span></span>](icon.md)|<span data-ttu-id="7f0dc-133">Representa o ícone que é o destino da condição se a classificação está no ícone da célula.</span><span class="sxs-lookup"><span data-stu-id="7f0dc-133">Represents the icon that is the target of the condition if the sorting is on the cell's icon.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7f0dc-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7f0dc-134">JSON representation</span></span>

<span data-ttu-id="7f0dc-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7f0dc-135">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.sortField"
}-->

```json
{
  "ascending": true,
  "color": "string",
  "dataOption": "string",
  "key": 1024,
  "sortOn": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "SortField resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/sortfield.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
