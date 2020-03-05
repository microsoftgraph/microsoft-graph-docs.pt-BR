---
title: tipo de recurso workbookSortField
description: Representa uma condição em uma operação de classificação.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: excel
author: ''
ms.openlocfilehash: adcebc20b39d40ef283d25cfd2a8c247160580eb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519138"
---
# <a name="workbooksortfield-resource-type"></a><span data-ttu-id="77753-103">tipo de recurso workbookSortField</span><span class="sxs-lookup"><span data-stu-id="77753-103">workbookSortField resource type</span></span>

<span data-ttu-id="77753-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="77753-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="77753-105">Representa uma condição em uma operação de classificação.</span><span class="sxs-lookup"><span data-stu-id="77753-105">Represents a condition in a sorting operation.</span></span>

## <a name="properties"></a><span data-ttu-id="77753-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="77753-106">Properties</span></span>
| <span data-ttu-id="77753-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="77753-107">Property</span></span>     | <span data-ttu-id="77753-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="77753-108">Type</span></span>   |<span data-ttu-id="77753-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="77753-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="77753-110">ascending</span><span class="sxs-lookup"><span data-stu-id="77753-110">ascending</span></span>|<span data-ttu-id="77753-111">booliano</span><span class="sxs-lookup"><span data-stu-id="77753-111">boolean</span></span>|<span data-ttu-id="77753-112">Indica se a classificação é feita de forma crescente.</span><span class="sxs-lookup"><span data-stu-id="77753-112">Represents whether the sorting is done in an ascending fashion.</span></span>|
|<span data-ttu-id="77753-113">color</span><span class="sxs-lookup"><span data-stu-id="77753-113">color</span></span>|<span data-ttu-id="77753-114">string</span><span class="sxs-lookup"><span data-stu-id="77753-114">string</span></span>|<span data-ttu-id="77753-115">Representa a cor que é o destino da condição se a classificação estiver na cor da fonte ou da célula.</span><span class="sxs-lookup"><span data-stu-id="77753-115">Represents the color that is the target of the condition if the sorting is on font or cell color.</span></span>|
|<span data-ttu-id="77753-116">dataOption</span><span class="sxs-lookup"><span data-stu-id="77753-116">dataOption</span></span>|<span data-ttu-id="77753-117">string</span><span class="sxs-lookup"><span data-stu-id="77753-117">string</span></span>|<span data-ttu-id="77753-p101">Representa as opções de classificação adicionais para esse campo. Os valores possíveis são: `Normal` e `TextAsNumber`.</span><span class="sxs-lookup"><span data-stu-id="77753-p101">Represents additional sorting options for this field. Possible values are: `Normal`, `TextAsNumber`.</span></span>|
|<span data-ttu-id="77753-120">key</span><span class="sxs-lookup"><span data-stu-id="77753-120">key</span></span>|<span data-ttu-id="77753-121">int</span><span class="sxs-lookup"><span data-stu-id="77753-121">int</span></span>|<span data-ttu-id="77753-p102">Representa a coluna (ou linha, dependendo da orientação da classificação) em que a condição está. Representado como um deslocamento da primeira coluna (ou linha).</span><span class="sxs-lookup"><span data-stu-id="77753-p102">Represents the column (or row, depending on the sort orientation) that the condition is on. Represented as an offset from the first column (or row).</span></span>|
|<span data-ttu-id="77753-124">sortOn</span><span class="sxs-lookup"><span data-stu-id="77753-124">sortOn</span></span>|<span data-ttu-id="77753-125">string</span><span class="sxs-lookup"><span data-stu-id="77753-125">string</span></span>|<span data-ttu-id="77753-p103">Representa o tipo de classificação dessa condição. Os valores possíveis são: `Value`, `CellColor`, `FontColor` e `Icon`.</span><span class="sxs-lookup"><span data-stu-id="77753-p103">Represents the type of sorting of this condition. Possible values are: `Value`, `CellColor`, `FontColor`, `Icon`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="77753-128">Relações</span><span class="sxs-lookup"><span data-stu-id="77753-128">Relationships</span></span>
| <span data-ttu-id="77753-129">Relação</span><span class="sxs-lookup"><span data-stu-id="77753-129">Relationship</span></span> | <span data-ttu-id="77753-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="77753-130">Type</span></span>   |<span data-ttu-id="77753-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="77753-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="77753-132">ícone</span><span class="sxs-lookup"><span data-stu-id="77753-132">icon</span></span>|[<span data-ttu-id="77753-133">workbookIcon</span><span class="sxs-lookup"><span data-stu-id="77753-133">workbookIcon</span></span>](workbookicon.md)|<span data-ttu-id="77753-134">Representa o ícone que é o destino da condição se a classificação está no ícone da célula.</span><span class="sxs-lookup"><span data-stu-id="77753-134">Represents the icon that is the target of the condition if the sorting is on the cell's icon.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="77753-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="77753-135">JSON representation</span></span>

<span data-ttu-id="77753-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="77753-136">Here is a JSON representation of the resource.</span></span>

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
