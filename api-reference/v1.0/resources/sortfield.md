---
title: Tipo de recurso SortField
description: Representa uma condição em uma operação de classificação.
localization_priority: Normal
ms.openlocfilehash: 2c1b9a272fd024455d1297c5f59ca7684283e1a1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32561296"
---
# <a name="sortfield-resource-type"></a><span data-ttu-id="eff09-103">Tipo de recurso SortField</span><span class="sxs-lookup"><span data-stu-id="eff09-103">SortField resource type</span></span>

<span data-ttu-id="eff09-104">Representa uma condição em uma operação de classificação.</span><span class="sxs-lookup"><span data-stu-id="eff09-104">Represents a condition in a sorting operation.</span></span>

## <a name="properties"></a><span data-ttu-id="eff09-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="eff09-105">Properties</span></span>
| <span data-ttu-id="eff09-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eff09-106">Property</span></span>     | <span data-ttu-id="eff09-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="eff09-107">Type</span></span>   |<span data-ttu-id="eff09-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="eff09-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eff09-109">ascending</span><span class="sxs-lookup"><span data-stu-id="eff09-109">ascending</span></span>|<span data-ttu-id="eff09-110">booliano</span><span class="sxs-lookup"><span data-stu-id="eff09-110">boolean</span></span>|<span data-ttu-id="eff09-111">Indica se a classificação é feita de forma crescente.</span><span class="sxs-lookup"><span data-stu-id="eff09-111">Represents whether the sorting is done in an ascending fashion.</span></span>|
|<span data-ttu-id="eff09-112">color</span><span class="sxs-lookup"><span data-stu-id="eff09-112">color</span></span>|<span data-ttu-id="eff09-113">string</span><span class="sxs-lookup"><span data-stu-id="eff09-113">string</span></span>|<span data-ttu-id="eff09-114">Representa a cor que é o destino da condição se a classificação estiver na cor da fonte ou da célula.</span><span class="sxs-lookup"><span data-stu-id="eff09-114">Represents the color that is the target of the condition if the sorting is on font or cell color.</span></span>|
|<span data-ttu-id="eff09-115">dataOption</span><span class="sxs-lookup"><span data-stu-id="eff09-115">dataOption</span></span>|<span data-ttu-id="eff09-116">string</span><span class="sxs-lookup"><span data-stu-id="eff09-116">string</span></span>|<span data-ttu-id="eff09-117">Representa as opções de classificação adicionais para esse campo.</span><span class="sxs-lookup"><span data-stu-id="eff09-117">Represents additional sorting options for this field.</span></span> <span data-ttu-id="eff09-118">Os valores possíveis são: `Normal`, `TextAsNumber`.</span><span class="sxs-lookup"><span data-stu-id="eff09-118">The possible values are: `Normal`, `TextAsNumber`.</span></span>|
|<span data-ttu-id="eff09-119">key</span><span class="sxs-lookup"><span data-stu-id="eff09-119">key</span></span>|<span data-ttu-id="eff09-120">int</span><span class="sxs-lookup"><span data-stu-id="eff09-120">int</span></span>|<span data-ttu-id="eff09-p102">Representa a coluna (ou linha, dependendo da orientação da classificação) em que a condição está. Representado como um deslocamento da primeira coluna (ou linha).</span><span class="sxs-lookup"><span data-stu-id="eff09-p102">Represents the column (or row, depending on the sort orientation) that the condition is on. Represented as an offset from the first column (or row).</span></span>|
|<span data-ttu-id="eff09-123">sortOn</span><span class="sxs-lookup"><span data-stu-id="eff09-123">sortOn</span></span>|<span data-ttu-id="eff09-124">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="eff09-124">string</span></span>|<span data-ttu-id="eff09-125">Representa o tipo de classificação dessa condição.</span><span class="sxs-lookup"><span data-stu-id="eff09-125">Represents the type of sorting of this condition.</span></span> <span data-ttu-id="eff09-126">Os valores possíveis são: `Value`, `CellColor`, `FontColor`, `Icon`.</span><span class="sxs-lookup"><span data-stu-id="eff09-126">The possible values are: `Value`, `CellColor`, `FontColor`, `Icon`.</span></span>|
|<span data-ttu-id="eff09-127">ícone</span><span class="sxs-lookup"><span data-stu-id="eff09-127">icon</span></span>|[<span data-ttu-id="eff09-128">WorkbookIcon</span><span class="sxs-lookup"><span data-stu-id="eff09-128">WorkbookIcon</span></span>](icon.md)|<span data-ttu-id="eff09-129">Representa o ícone que é o destino da condição se a classificação está no ícone da célula.</span><span class="sxs-lookup"><span data-stu-id="eff09-129">Represents the icon that is the target of the condition if the sorting is on the cell's icon.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="eff09-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="eff09-130">JSON representation</span></span>

<span data-ttu-id="eff09-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="eff09-131">Here is a JSON representation of the resource.</span></span>

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
