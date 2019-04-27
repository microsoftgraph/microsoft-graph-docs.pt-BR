---
title: tipo de recurso workbookSortField
description: Representa uma condição em uma operação de classificação.
localization_priority: Normal
ms.openlocfilehash: 239c0e3b9f95108165ed32e7e22f94049e787432
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348529"
---
# <a name="workbooksortfield-resource-type"></a><span data-ttu-id="b0c2c-103">tipo de recurso workbookSortField</span><span class="sxs-lookup"><span data-stu-id="b0c2c-103">workbookSortField resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b0c2c-104">Representa uma condição em uma operação de classificação.</span><span class="sxs-lookup"><span data-stu-id="b0c2c-104">Represents a condition in a sorting operation.</span></span>

## <a name="properties"></a><span data-ttu-id="b0c2c-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b0c2c-105">Properties</span></span>
| <span data-ttu-id="b0c2c-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b0c2c-106">Property</span></span>     | <span data-ttu-id="b0c2c-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="b0c2c-107">Type</span></span>   |<span data-ttu-id="b0c2c-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="b0c2c-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b0c2c-109">ascending</span><span class="sxs-lookup"><span data-stu-id="b0c2c-109">ascending</span></span>|<span data-ttu-id="b0c2c-110">booliano</span><span class="sxs-lookup"><span data-stu-id="b0c2c-110">boolean</span></span>|<span data-ttu-id="b0c2c-111">Indica se a classificação é feita de forma crescente.</span><span class="sxs-lookup"><span data-stu-id="b0c2c-111">Represents whether the sorting is done in an ascending fashion.</span></span>|
|<span data-ttu-id="b0c2c-112">color</span><span class="sxs-lookup"><span data-stu-id="b0c2c-112">color</span></span>|<span data-ttu-id="b0c2c-113">string</span><span class="sxs-lookup"><span data-stu-id="b0c2c-113">string</span></span>|<span data-ttu-id="b0c2c-114">Representa a cor que é o destino da condição se a classificação estiver na cor da fonte ou da célula.</span><span class="sxs-lookup"><span data-stu-id="b0c2c-114">Represents the color that is the target of the condition if the sorting is on font or cell color.</span></span>|
|<span data-ttu-id="b0c2c-115">dataOption</span><span class="sxs-lookup"><span data-stu-id="b0c2c-115">dataOption</span></span>|<span data-ttu-id="b0c2c-116">string</span><span class="sxs-lookup"><span data-stu-id="b0c2c-116">string</span></span>|<span data-ttu-id="b0c2c-p101">Representa as opções de classificação adicionais para esse campo. Os valores possíveis são: `Normal` e `TextAsNumber`.</span><span class="sxs-lookup"><span data-stu-id="b0c2c-p101">Represents additional sorting options for this field. Possible values are: `Normal`, `TextAsNumber`.</span></span>|
|<span data-ttu-id="b0c2c-119">key</span><span class="sxs-lookup"><span data-stu-id="b0c2c-119">key</span></span>|<span data-ttu-id="b0c2c-120">int</span><span class="sxs-lookup"><span data-stu-id="b0c2c-120">int</span></span>|<span data-ttu-id="b0c2c-p102">Representa a coluna (ou linha, dependendo da orientação da classificação) em que a condição está. Representado como um deslocamento da primeira coluna (ou linha).</span><span class="sxs-lookup"><span data-stu-id="b0c2c-p102">Represents the column (or row, depending on the sort orientation) that the condition is on. Represented as an offset from the first column (or row).</span></span>|
|<span data-ttu-id="b0c2c-123">sortOn</span><span class="sxs-lookup"><span data-stu-id="b0c2c-123">sortOn</span></span>|<span data-ttu-id="b0c2c-124">string</span><span class="sxs-lookup"><span data-stu-id="b0c2c-124">string</span></span>|<span data-ttu-id="b0c2c-p103">Representa o tipo de classificação dessa condição. Os valores possíveis são: `Value`, `CellColor`, `FontColor` e `Icon`.</span><span class="sxs-lookup"><span data-stu-id="b0c2c-p103">Represents the type of sorting of this condition. Possible values are: `Value`, `CellColor`, `FontColor`, `Icon`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b0c2c-127">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="b0c2c-127">Relationships</span></span>
| <span data-ttu-id="b0c2c-128">Relação</span><span class="sxs-lookup"><span data-stu-id="b0c2c-128">Relationship</span></span> | <span data-ttu-id="b0c2c-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="b0c2c-129">Type</span></span>   |<span data-ttu-id="b0c2c-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="b0c2c-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b0c2c-131">ícone</span><span class="sxs-lookup"><span data-stu-id="b0c2c-131">icon</span></span>|[<span data-ttu-id="b0c2c-132">workbookIcon</span><span class="sxs-lookup"><span data-stu-id="b0c2c-132">workbookIcon</span></span>](workbookicon.md)|<span data-ttu-id="b0c2c-133">Representa o ícone que é o destino da condição se a classificação está no ícone da célula.</span><span class="sxs-lookup"><span data-stu-id="b0c2c-133">Represents the icon that is the target of the condition if the sorting is on the cell's icon.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b0c2c-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b0c2c-134">JSON representation</span></span>

<span data-ttu-id="b0c2c-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b0c2c-135">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookSortField"
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
  "suppressions": []
}
-->
