---
title: tipo de recurso workbookSortField
description: Representa uma condição em uma operação de classificação.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: excel
author: ''
ms.openlocfilehash: 55a1f822e080f786b588837dd6d9120cea546d4b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35963903"
---
# <a name="workbooksortfield-resource-type"></a><span data-ttu-id="9697f-103">tipo de recurso workbookSortField</span><span class="sxs-lookup"><span data-stu-id="9697f-103">workbookSortField resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9697f-104">Representa uma condição em uma operação de classificação.</span><span class="sxs-lookup"><span data-stu-id="9697f-104">Represents a condition in a sorting operation.</span></span>

## <a name="properties"></a><span data-ttu-id="9697f-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9697f-105">Properties</span></span>
| <span data-ttu-id="9697f-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9697f-106">Property</span></span>     | <span data-ttu-id="9697f-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="9697f-107">Type</span></span>   |<span data-ttu-id="9697f-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="9697f-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9697f-109">ascending</span><span class="sxs-lookup"><span data-stu-id="9697f-109">ascending</span></span>|<span data-ttu-id="9697f-110">booliano</span><span class="sxs-lookup"><span data-stu-id="9697f-110">boolean</span></span>|<span data-ttu-id="9697f-111">Indica se a classificação é feita de forma crescente.</span><span class="sxs-lookup"><span data-stu-id="9697f-111">Represents whether the sorting is done in an ascending fashion.</span></span>|
|<span data-ttu-id="9697f-112">color</span><span class="sxs-lookup"><span data-stu-id="9697f-112">color</span></span>|<span data-ttu-id="9697f-113">string</span><span class="sxs-lookup"><span data-stu-id="9697f-113">string</span></span>|<span data-ttu-id="9697f-114">Representa a cor que é o destino da condição se a classificação estiver na cor da fonte ou da célula.</span><span class="sxs-lookup"><span data-stu-id="9697f-114">Represents the color that is the target of the condition if the sorting is on font or cell color.</span></span>|
|<span data-ttu-id="9697f-115">dataOption</span><span class="sxs-lookup"><span data-stu-id="9697f-115">dataOption</span></span>|<span data-ttu-id="9697f-116">string</span><span class="sxs-lookup"><span data-stu-id="9697f-116">string</span></span>|<span data-ttu-id="9697f-p101">Representa as opções de classificação adicionais para esse campo. Os valores possíveis são: `Normal` e `TextAsNumber`.</span><span class="sxs-lookup"><span data-stu-id="9697f-p101">Represents additional sorting options for this field. Possible values are: `Normal`, `TextAsNumber`.</span></span>|
|<span data-ttu-id="9697f-119">key</span><span class="sxs-lookup"><span data-stu-id="9697f-119">key</span></span>|<span data-ttu-id="9697f-120">int</span><span class="sxs-lookup"><span data-stu-id="9697f-120">int</span></span>|<span data-ttu-id="9697f-p102">Representa a coluna (ou linha, dependendo da orientação da classificação) em que a condição está. Representado como um deslocamento da primeira coluna (ou linha).</span><span class="sxs-lookup"><span data-stu-id="9697f-p102">Represents the column (or row, depending on the sort orientation) that the condition is on. Represented as an offset from the first column (or row).</span></span>|
|<span data-ttu-id="9697f-123">sortOn</span><span class="sxs-lookup"><span data-stu-id="9697f-123">sortOn</span></span>|<span data-ttu-id="9697f-124">string</span><span class="sxs-lookup"><span data-stu-id="9697f-124">string</span></span>|<span data-ttu-id="9697f-p103">Representa o tipo de classificação dessa condição. Os valores possíveis são: `Value`, `CellColor`, `FontColor` e `Icon`.</span><span class="sxs-lookup"><span data-stu-id="9697f-p103">Represents the type of sorting of this condition. Possible values are: `Value`, `CellColor`, `FontColor`, `Icon`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9697f-127">Relações</span><span class="sxs-lookup"><span data-stu-id="9697f-127">Relationships</span></span>
| <span data-ttu-id="9697f-128">Relação</span><span class="sxs-lookup"><span data-stu-id="9697f-128">Relationship</span></span> | <span data-ttu-id="9697f-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="9697f-129">Type</span></span>   |<span data-ttu-id="9697f-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="9697f-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9697f-131">ícone</span><span class="sxs-lookup"><span data-stu-id="9697f-131">icon</span></span>|[<span data-ttu-id="9697f-132">workbookIcon</span><span class="sxs-lookup"><span data-stu-id="9697f-132">workbookIcon</span></span>](workbookicon.md)|<span data-ttu-id="9697f-133">Representa o ícone que é o destino da condição se a classificação está no ícone da célula.</span><span class="sxs-lookup"><span data-stu-id="9697f-133">Represents the icon that is the target of the condition if the sorting is on the cell's icon.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9697f-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9697f-134">JSON representation</span></span>

<span data-ttu-id="9697f-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9697f-135">Here is a JSON representation of the resource.</span></span>

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
