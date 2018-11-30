---
title: Tipo de recurso SortField
description: Representa uma condição em uma operação de classificação.
ms.openlocfilehash: b6fc87e03b63a3e1cc34beef61a7538a913a118a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006261"
---
# <a name="sortfield-resource-type"></a><span data-ttu-id="2ae1a-103">Tipo de recurso SortField</span><span class="sxs-lookup"><span data-stu-id="2ae1a-103">SortField resource type</span></span>

<span data-ttu-id="2ae1a-104">Representa uma condição em uma operação de classificação.</span><span class="sxs-lookup"><span data-stu-id="2ae1a-104">Represents a condition in a sorting operation.</span></span>

## <a name="properties"></a><span data-ttu-id="2ae1a-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2ae1a-105">Properties</span></span>
| <span data-ttu-id="2ae1a-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2ae1a-106">Property</span></span>     | <span data-ttu-id="2ae1a-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="2ae1a-107">Type</span></span>   |<span data-ttu-id="2ae1a-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="2ae1a-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2ae1a-109">ascending</span><span class="sxs-lookup"><span data-stu-id="2ae1a-109">ascending</span></span>|<span data-ttu-id="2ae1a-110">booliano</span><span class="sxs-lookup"><span data-stu-id="2ae1a-110">boolean</span></span>|<span data-ttu-id="2ae1a-111">Indica se a classificação é feita de forma crescente.</span><span class="sxs-lookup"><span data-stu-id="2ae1a-111">Represents whether the sorting is done in an ascending fashion.</span></span>|
|<span data-ttu-id="2ae1a-112">color</span><span class="sxs-lookup"><span data-stu-id="2ae1a-112">color</span></span>|<span data-ttu-id="2ae1a-113">string</span><span class="sxs-lookup"><span data-stu-id="2ae1a-113">string</span></span>|<span data-ttu-id="2ae1a-114">Representa a cor que é o destino da condição se a classificação estiver na cor da fonte ou da célula.</span><span class="sxs-lookup"><span data-stu-id="2ae1a-114">Represents the color that is the target of the condition if the sorting is on font or cell color.</span></span>|
|<span data-ttu-id="2ae1a-115">dataOption</span><span class="sxs-lookup"><span data-stu-id="2ae1a-115">dataOption</span></span>|<span data-ttu-id="2ae1a-116">string</span><span class="sxs-lookup"><span data-stu-id="2ae1a-116">string</span></span>|<span data-ttu-id="2ae1a-117">Representa as opções de classificação adicionais para esse campo.</span><span class="sxs-lookup"><span data-stu-id="2ae1a-117">Represents additional sorting options for this field.</span></span> <span data-ttu-id="2ae1a-118">Os valores possíveis são: `Normal`, `TextAsNumber`.</span><span class="sxs-lookup"><span data-stu-id="2ae1a-118">The possible values are: `Normal`, `TextAsNumber`.</span></span>|
|<span data-ttu-id="2ae1a-119">key</span><span class="sxs-lookup"><span data-stu-id="2ae1a-119">key</span></span>|<span data-ttu-id="2ae1a-120">inteiro</span><span class="sxs-lookup"><span data-stu-id="2ae1a-120">int</span></span>|<span data-ttu-id="2ae1a-p102">Representa a coluna (ou linha, dependendo da orientação da classificação) em que a condição está. Representado como um deslocamento da primeira coluna (ou linha).</span><span class="sxs-lookup"><span data-stu-id="2ae1a-p102">Represents the column (or row, depending on the sort orientation) that the condition is on. Represented as an offset from the first column (or row).</span></span>|
|<span data-ttu-id="2ae1a-123">sortOn</span><span class="sxs-lookup"><span data-stu-id="2ae1a-123">sortOn</span></span>|<span data-ttu-id="2ae1a-124">string</span><span class="sxs-lookup"><span data-stu-id="2ae1a-124">string</span></span>|<span data-ttu-id="2ae1a-125">Representa o tipo de classificação dessa condição.</span><span class="sxs-lookup"><span data-stu-id="2ae1a-125">Represents the type of sorting of this condition.</span></span> <span data-ttu-id="2ae1a-126">Os valores possíveis são: `Value`, `CellColor`, `FontColor`, `Icon`.</span><span class="sxs-lookup"><span data-stu-id="2ae1a-126">The possible values are: `Value`, `CellColor`, `FontColor`, `Icon`.</span></span>|
|<span data-ttu-id="2ae1a-127">ícone</span><span class="sxs-lookup"><span data-stu-id="2ae1a-127">icon</span></span>|[<span data-ttu-id="2ae1a-128">WorkbookIcon</span><span class="sxs-lookup"><span data-stu-id="2ae1a-128">WorkbookIcon</span></span>](icon.md)|<span data-ttu-id="2ae1a-129">Representa o ícone que é o destino da condição se a classificação está no ícone da célula.</span><span class="sxs-lookup"><span data-stu-id="2ae1a-129">Represents the icon that is the target of the condition if the sorting is on the cell's icon.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2ae1a-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2ae1a-130">JSON representation</span></span>

<span data-ttu-id="2ae1a-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2ae1a-131">Here is a JSON representation of the resource.</span></span>

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