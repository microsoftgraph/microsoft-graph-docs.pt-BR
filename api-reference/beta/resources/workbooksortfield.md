---
title: Tipo de recurso workbookSortField
description: Representa uma condição em uma operação de classificação.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: excel
author: ruoyingl
ms.openlocfilehash: a245591755542a0a9bcfefb3f220511bd1521118
ms.sourcegitcommit: de175a11806f9e9ba3c916384e897aee1cc7f75c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/09/2021
ms.locfileid: "49790668"
---
# <a name="workbooksortfield-resource-type"></a><span data-ttu-id="b244f-103">Tipo de recurso workbookSortField</span><span class="sxs-lookup"><span data-stu-id="b244f-103">workbookSortField resource type</span></span>

<span data-ttu-id="b244f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b244f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b244f-105">Representa uma condição em uma operação de classificação.</span><span class="sxs-lookup"><span data-stu-id="b244f-105">Represents a condition in a sorting operation.</span></span>

## <a name="properties"></a><span data-ttu-id="b244f-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b244f-106">Properties</span></span>
| <span data-ttu-id="b244f-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b244f-107">Property</span></span>     | <span data-ttu-id="b244f-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="b244f-108">Type</span></span>   |<span data-ttu-id="b244f-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="b244f-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b244f-110">ascending</span><span class="sxs-lookup"><span data-stu-id="b244f-110">ascending</span></span>|<span data-ttu-id="b244f-111">booliano</span><span class="sxs-lookup"><span data-stu-id="b244f-111">boolean</span></span>|<span data-ttu-id="b244f-112">Indica se a classificação é feita de forma crescente.</span><span class="sxs-lookup"><span data-stu-id="b244f-112">Represents whether the sorting is done in an ascending fashion.</span></span>|
|<span data-ttu-id="b244f-113">color</span><span class="sxs-lookup"><span data-stu-id="b244f-113">color</span></span>|<span data-ttu-id="b244f-114">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b244f-114">string</span></span>|<span data-ttu-id="b244f-115">Representa a cor que é o destino da condição se a classificação estiver na cor da fonte ou da célula.</span><span class="sxs-lookup"><span data-stu-id="b244f-115">Represents the color that is the target of the condition if the sorting is on font or cell color.</span></span>|
|<span data-ttu-id="b244f-116">dataOption</span><span class="sxs-lookup"><span data-stu-id="b244f-116">dataOption</span></span>|<span data-ttu-id="b244f-117">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b244f-117">string</span></span>|<span data-ttu-id="b244f-p101">Representa as opções de classificação adicionais para esse campo. Os valores possíveis são: `Normal` e `TextAsNumber`.</span><span class="sxs-lookup"><span data-stu-id="b244f-p101">Represents additional sorting options for this field. Possible values are: `Normal`, `TextAsNumber`.</span></span>|
|<span data-ttu-id="b244f-120">ícone</span><span class="sxs-lookup"><span data-stu-id="b244f-120">icon</span></span>|[<span data-ttu-id="b244f-121">workbookIcon</span><span class="sxs-lookup"><span data-stu-id="b244f-121">workbookIcon</span></span>](workbookicon.md)|<span data-ttu-id="b244f-122">Representa o ícone que é o destino da condição se a classificação está no ícone da célula.</span><span class="sxs-lookup"><span data-stu-id="b244f-122">Represents the icon that is the target of the condition if the sorting is on the cell's icon.</span></span>|
|<span data-ttu-id="b244f-123">key</span><span class="sxs-lookup"><span data-stu-id="b244f-123">key</span></span>|<span data-ttu-id="b244f-124">int</span><span class="sxs-lookup"><span data-stu-id="b244f-124">int</span></span>|<span data-ttu-id="b244f-p102">Representa a coluna (ou linha, dependendo da orientação da classificação) em que a condição está. Representado como um deslocamento da primeira coluna (ou linha).</span><span class="sxs-lookup"><span data-stu-id="b244f-p102">Represents the column (or row, depending on the sort orientation) that the condition is on. Represented as an offset from the first column (or row).</span></span>|
|<span data-ttu-id="b244f-127">sortOn</span><span class="sxs-lookup"><span data-stu-id="b244f-127">sortOn</span></span>|<span data-ttu-id="b244f-128">string</span><span class="sxs-lookup"><span data-stu-id="b244f-128">string</span></span>|<span data-ttu-id="b244f-p103">Representa o tipo de classificação dessa condição. Os valores possíveis são: `Value`, `CellColor`, `FontColor` e `Icon`.</span><span class="sxs-lookup"><span data-stu-id="b244f-p103">Represents the type of sorting of this condition. Possible values are: `Value`, `CellColor`, `FontColor`, `Icon`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b244f-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b244f-131">JSON representation</span></span>

<span data-ttu-id="b244f-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b244f-132">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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


