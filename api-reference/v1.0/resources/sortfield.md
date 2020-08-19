---
title: Tipo de recurso SortField
description: Representa uma condição em uma operação de classificação.
localization_priority: Normal
author: ruoyingl
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: debc1f860e2e24306d6261444a29e126037aa3ae
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46806741"
---
# <a name="sortfield-resource-type"></a><span data-ttu-id="d82f4-103">Tipo de recurso SortField</span><span class="sxs-lookup"><span data-stu-id="d82f4-103">SortField resource type</span></span>

<span data-ttu-id="d82f4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d82f4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d82f4-105">Representa uma condição em uma operação de classificação.</span><span class="sxs-lookup"><span data-stu-id="d82f4-105">Represents a condition in a sorting operation.</span></span>

## <a name="properties"></a><span data-ttu-id="d82f4-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d82f4-106">Properties</span></span>
| <span data-ttu-id="d82f4-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d82f4-107">Property</span></span>     | <span data-ttu-id="d82f4-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="d82f4-108">Type</span></span>   |<span data-ttu-id="d82f4-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="d82f4-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d82f4-110">ascending</span><span class="sxs-lookup"><span data-stu-id="d82f4-110">ascending</span></span>|<span data-ttu-id="d82f4-111">booliano</span><span class="sxs-lookup"><span data-stu-id="d82f4-111">boolean</span></span>|<span data-ttu-id="d82f4-112">Indica se a classificação é feita de forma crescente.</span><span class="sxs-lookup"><span data-stu-id="d82f4-112">Represents whether the sorting is done in an ascending fashion.</span></span>|
|<span data-ttu-id="d82f4-113">color</span><span class="sxs-lookup"><span data-stu-id="d82f4-113">color</span></span>|<span data-ttu-id="d82f4-114">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d82f4-114">string</span></span>|<span data-ttu-id="d82f4-115">Representa a cor que é o destino da condição se a classificação estiver na cor da fonte ou da célula.</span><span class="sxs-lookup"><span data-stu-id="d82f4-115">Represents the color that is the target of the condition if the sorting is on font or cell color.</span></span>|
|<span data-ttu-id="d82f4-116">dataOption</span><span class="sxs-lookup"><span data-stu-id="d82f4-116">dataOption</span></span>|<span data-ttu-id="d82f4-117">string</span><span class="sxs-lookup"><span data-stu-id="d82f4-117">string</span></span>|<span data-ttu-id="d82f4-118">Representa as opções de classificação adicionais para esse campo.</span><span class="sxs-lookup"><span data-stu-id="d82f4-118">Represents additional sorting options for this field.</span></span> <span data-ttu-id="d82f4-119">Os valores possíveis são: `Normal` , `TextAsNumber` .</span><span class="sxs-lookup"><span data-stu-id="d82f4-119">The possible values are: `Normal`, `TextAsNumber`.</span></span>|
|<span data-ttu-id="d82f4-120">key</span><span class="sxs-lookup"><span data-stu-id="d82f4-120">key</span></span>|<span data-ttu-id="d82f4-121">int</span><span class="sxs-lookup"><span data-stu-id="d82f4-121">int</span></span>|<span data-ttu-id="d82f4-p102">Representa a coluna (ou linha, dependendo da orientação da classificação) em que a condição está. Representado como um deslocamento da primeira coluna (ou linha).</span><span class="sxs-lookup"><span data-stu-id="d82f4-p102">Represents the column (or row, depending on the sort orientation) that the condition is on. Represented as an offset from the first column (or row).</span></span>|
|<span data-ttu-id="d82f4-124">sortOn</span><span class="sxs-lookup"><span data-stu-id="d82f4-124">sortOn</span></span>|<span data-ttu-id="d82f4-125">string</span><span class="sxs-lookup"><span data-stu-id="d82f4-125">string</span></span>|<span data-ttu-id="d82f4-126">Representa o tipo de classificação dessa condição.</span><span class="sxs-lookup"><span data-stu-id="d82f4-126">Represents the type of sorting of this condition.</span></span> <span data-ttu-id="d82f4-127">Os valores possíveis são: `Value`, `CellColor`, `FontColor`, `Icon`.</span><span class="sxs-lookup"><span data-stu-id="d82f4-127">The possible values are: `Value`, `CellColor`, `FontColor`, `Icon`.</span></span>|
|<span data-ttu-id="d82f4-128">ícone</span><span class="sxs-lookup"><span data-stu-id="d82f4-128">icon</span></span>|[<span data-ttu-id="d82f4-129">WorkbookIcon</span><span class="sxs-lookup"><span data-stu-id="d82f4-129">WorkbookIcon</span></span>](icon.md)|<span data-ttu-id="d82f4-130">Representa o ícone que é o destino da condição se a classificação está no ícone da célula.</span><span class="sxs-lookup"><span data-stu-id="d82f4-130">Represents the icon that is the target of the condition if the sorting is on the cell's icon.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d82f4-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d82f4-131">JSON representation</span></span>

<span data-ttu-id="d82f4-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d82f4-132">Here is a JSON representation of the resource.</span></span>

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
