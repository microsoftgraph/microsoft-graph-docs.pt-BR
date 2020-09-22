---
title: Tipo de recurso SortField
description: Representa uma condição em uma operação de classificação.
localization_priority: Normal
author: ruoyingl
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 6bc2a983fe5b27759a0944975876c2c0a0b1ca41
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48086403"
---
# <a name="sortfield-resource-type"></a><span data-ttu-id="78699-103">Tipo de recurso SortField</span><span class="sxs-lookup"><span data-stu-id="78699-103">SortField resource type</span></span>

<span data-ttu-id="78699-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="78699-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="78699-105">Representa uma condição em uma operação de classificação.</span><span class="sxs-lookup"><span data-stu-id="78699-105">Represents a condition in a sorting operation.</span></span>

## <a name="properties"></a><span data-ttu-id="78699-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="78699-106">Properties</span></span>
| <span data-ttu-id="78699-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="78699-107">Property</span></span>     | <span data-ttu-id="78699-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="78699-108">Type</span></span>   |<span data-ttu-id="78699-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="78699-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="78699-110">ascending</span><span class="sxs-lookup"><span data-stu-id="78699-110">ascending</span></span>|<span data-ttu-id="78699-111">booliano</span><span class="sxs-lookup"><span data-stu-id="78699-111">boolean</span></span>|<span data-ttu-id="78699-112">Indica se a classificação é feita de forma crescente.</span><span class="sxs-lookup"><span data-stu-id="78699-112">Represents whether the sorting is done in an ascending fashion.</span></span>|
|<span data-ttu-id="78699-113">color</span><span class="sxs-lookup"><span data-stu-id="78699-113">color</span></span>|<span data-ttu-id="78699-114">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="78699-114">string</span></span>|<span data-ttu-id="78699-115">Representa a cor que é o destino da condição se a classificação estiver na cor da fonte ou da célula.</span><span class="sxs-lookup"><span data-stu-id="78699-115">Represents the color that is the target of the condition if the sorting is on font or cell color.</span></span>|
|<span data-ttu-id="78699-116">dataOption</span><span class="sxs-lookup"><span data-stu-id="78699-116">dataOption</span></span>|<span data-ttu-id="78699-117">string</span><span class="sxs-lookup"><span data-stu-id="78699-117">string</span></span>|<span data-ttu-id="78699-118">Representa as opções de classificação adicionais para esse campo.</span><span class="sxs-lookup"><span data-stu-id="78699-118">Represents additional sorting options for this field.</span></span> <span data-ttu-id="78699-119">Os valores possíveis são: `Normal` , `TextAsNumber` .</span><span class="sxs-lookup"><span data-stu-id="78699-119">The possible values are: `Normal`, `TextAsNumber`.</span></span>|
|<span data-ttu-id="78699-120">key</span><span class="sxs-lookup"><span data-stu-id="78699-120">key</span></span>|<span data-ttu-id="78699-121">int</span><span class="sxs-lookup"><span data-stu-id="78699-121">int</span></span>|<span data-ttu-id="78699-p102">Representa a coluna (ou linha, dependendo da orientação da classificação) em que a condição está. Representado como um deslocamento da primeira coluna (ou linha).</span><span class="sxs-lookup"><span data-stu-id="78699-p102">Represents the column (or row, depending on the sort orientation) that the condition is on. Represented as an offset from the first column (or row).</span></span>|
|<span data-ttu-id="78699-124">sortOn</span><span class="sxs-lookup"><span data-stu-id="78699-124">sortOn</span></span>|<span data-ttu-id="78699-125">string</span><span class="sxs-lookup"><span data-stu-id="78699-125">string</span></span>|<span data-ttu-id="78699-126">Representa o tipo de classificação dessa condição.</span><span class="sxs-lookup"><span data-stu-id="78699-126">Represents the type of sorting of this condition.</span></span> <span data-ttu-id="78699-127">Os valores possíveis são: `Value`, `CellColor`, `FontColor`, `Icon`.</span><span class="sxs-lookup"><span data-stu-id="78699-127">The possible values are: `Value`, `CellColor`, `FontColor`, `Icon`.</span></span>|
|<span data-ttu-id="78699-128">ícone</span><span class="sxs-lookup"><span data-stu-id="78699-128">icon</span></span>|[<span data-ttu-id="78699-129">WorkbookIcon</span><span class="sxs-lookup"><span data-stu-id="78699-129">WorkbookIcon</span></span>](icon.md)|<span data-ttu-id="78699-130">Representa o ícone que é o destino da condição se a classificação está no ícone da célula.</span><span class="sxs-lookup"><span data-stu-id="78699-130">Represents the icon that is the target of the condition if the sorting is on the cell's icon.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="78699-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="78699-131">JSON representation</span></span>

<span data-ttu-id="78699-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="78699-132">Here is a JSON representation of the resource.</span></span>

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

