---
title: Tipo de recurso SortField
description: Representa uma condição em uma operação de classificação.
localization_priority: Normal
ms.openlocfilehash: 2c1b9a272fd024455d1297c5f59ca7684283e1a1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27825967"
---
# <a name="sortfield-resource-type"></a><span data-ttu-id="0d6ca-103">Tipo de recurso SortField</span><span class="sxs-lookup"><span data-stu-id="0d6ca-103">SortField resource type</span></span>

<span data-ttu-id="0d6ca-104">Representa uma condição em uma operação de classificação.</span><span class="sxs-lookup"><span data-stu-id="0d6ca-104">Represents a condition in a sorting operation.</span></span>

## <a name="properties"></a><span data-ttu-id="0d6ca-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0d6ca-105">Properties</span></span>
| <span data-ttu-id="0d6ca-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0d6ca-106">Property</span></span>     | <span data-ttu-id="0d6ca-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="0d6ca-107">Type</span></span>   |<span data-ttu-id="0d6ca-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="0d6ca-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0d6ca-109">ascending</span><span class="sxs-lookup"><span data-stu-id="0d6ca-109">ascending</span></span>|<span data-ttu-id="0d6ca-110">booliano</span><span class="sxs-lookup"><span data-stu-id="0d6ca-110">boolean</span></span>|<span data-ttu-id="0d6ca-111">Indica se a classificação é feita de forma crescente.</span><span class="sxs-lookup"><span data-stu-id="0d6ca-111">Represents whether the sorting is done in an ascending fashion.</span></span>|
|<span data-ttu-id="0d6ca-112">color</span><span class="sxs-lookup"><span data-stu-id="0d6ca-112">color</span></span>|<span data-ttu-id="0d6ca-113">string</span><span class="sxs-lookup"><span data-stu-id="0d6ca-113">string</span></span>|<span data-ttu-id="0d6ca-114">Representa a cor que é o destino da condição se a classificação estiver na cor da fonte ou da célula.</span><span class="sxs-lookup"><span data-stu-id="0d6ca-114">Represents the color that is the target of the condition if the sorting is on font or cell color.</span></span>|
|<span data-ttu-id="0d6ca-115">dataOption</span><span class="sxs-lookup"><span data-stu-id="0d6ca-115">dataOption</span></span>|<span data-ttu-id="0d6ca-116">string</span><span class="sxs-lookup"><span data-stu-id="0d6ca-116">string</span></span>|<span data-ttu-id="0d6ca-117">Representa as opções de classificação adicionais para esse campo.</span><span class="sxs-lookup"><span data-stu-id="0d6ca-117">Represents additional sorting options for this field.</span></span> <span data-ttu-id="0d6ca-118">Os valores possíveis são: `Normal`, `TextAsNumber`.</span><span class="sxs-lookup"><span data-stu-id="0d6ca-118">The possible values are: `Normal`, `TextAsNumber`.</span></span>|
|<span data-ttu-id="0d6ca-119">key</span><span class="sxs-lookup"><span data-stu-id="0d6ca-119">key</span></span>|<span data-ttu-id="0d6ca-120">int</span><span class="sxs-lookup"><span data-stu-id="0d6ca-120">int</span></span>|<span data-ttu-id="0d6ca-p102">Representa a coluna (ou linha, dependendo da orientação da classificação) em que a condição está. Representado como um deslocamento da primeira coluna (ou linha).</span><span class="sxs-lookup"><span data-stu-id="0d6ca-p102">Represents the column (or row, depending on the sort orientation) that the condition is on. Represented as an offset from the first column (or row).</span></span>|
|<span data-ttu-id="0d6ca-123">sortOn</span><span class="sxs-lookup"><span data-stu-id="0d6ca-123">sortOn</span></span>|<span data-ttu-id="0d6ca-124">string</span><span class="sxs-lookup"><span data-stu-id="0d6ca-124">string</span></span>|<span data-ttu-id="0d6ca-125">Representa o tipo de classificação dessa condição.</span><span class="sxs-lookup"><span data-stu-id="0d6ca-125">Represents the type of sorting of this condition.</span></span> <span data-ttu-id="0d6ca-126">Os valores possíveis são: `Value`, `CellColor`, `FontColor`, `Icon`.</span><span class="sxs-lookup"><span data-stu-id="0d6ca-126">The possible values are: `Value`, `CellColor`, `FontColor`, `Icon`.</span></span>|
|<span data-ttu-id="0d6ca-127">ícone</span><span class="sxs-lookup"><span data-stu-id="0d6ca-127">icon</span></span>|[<span data-ttu-id="0d6ca-128">WorkbookIcon</span><span class="sxs-lookup"><span data-stu-id="0d6ca-128">WorkbookIcon</span></span>](icon.md)|<span data-ttu-id="0d6ca-129">Representa o ícone que é o destino da condição se a classificação está no ícone da célula.</span><span class="sxs-lookup"><span data-stu-id="0d6ca-129">Represents the icon that is the target of the condition if the sorting is on the cell's icon.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0d6ca-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0d6ca-130">JSON representation</span></span>

<span data-ttu-id="0d6ca-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0d6ca-131">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.workbookSortField"
}-->

```json
{
  "ascending": true,
  "color": "string",
  "dataOption": "string",
  "key": 1024,
  "sortOn": "string",
  "icon": { "@odata.type": "microsoft.graph.workbookIcon" }
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "SortField resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
