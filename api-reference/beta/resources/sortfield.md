---
title: Tipo de recurso SortField
description: Representa uma condição em uma operação de classificação.
localization_priority: Normal
ms.openlocfilehash: fc93f33f7e1c6f366986cd5d1ca82ea186ad44b9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894275"
---
# <a name="sortfield-resource-type"></a><span data-ttu-id="0b69a-103">Tipo de recurso SortField</span><span class="sxs-lookup"><span data-stu-id="0b69a-103">SortField resource type</span></span>

> <span data-ttu-id="0b69a-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="0b69a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0b69a-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="0b69a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0b69a-106">Representa uma condição em uma operação de classificação.</span><span class="sxs-lookup"><span data-stu-id="0b69a-106">Represents a condition in a sorting operation.</span></span>

## <a name="properties"></a><span data-ttu-id="0b69a-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0b69a-107">Properties</span></span>
| <span data-ttu-id="0b69a-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0b69a-108">Property</span></span>     | <span data-ttu-id="0b69a-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="0b69a-109">Type</span></span>   |<span data-ttu-id="0b69a-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="0b69a-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0b69a-111">ascending</span><span class="sxs-lookup"><span data-stu-id="0b69a-111">ascending</span></span>|<span data-ttu-id="0b69a-112">booliano</span><span class="sxs-lookup"><span data-stu-id="0b69a-112">boolean</span></span>|<span data-ttu-id="0b69a-113">Indica se a classificação é feita de forma crescente.</span><span class="sxs-lookup"><span data-stu-id="0b69a-113">Represents whether the sorting is done in an ascending fashion.</span></span>|
|<span data-ttu-id="0b69a-114">color</span><span class="sxs-lookup"><span data-stu-id="0b69a-114">color</span></span>|<span data-ttu-id="0b69a-115">string</span><span class="sxs-lookup"><span data-stu-id="0b69a-115">string</span></span>|<span data-ttu-id="0b69a-116">Representa a cor que é o destino da condição se a classificação estiver na cor da fonte ou da célula.</span><span class="sxs-lookup"><span data-stu-id="0b69a-116">Represents the color that is the target of the condition if the sorting is on font or cell color.</span></span>|
|<span data-ttu-id="0b69a-117">dataOption</span><span class="sxs-lookup"><span data-stu-id="0b69a-117">dataOption</span></span>|<span data-ttu-id="0b69a-118">string</span><span class="sxs-lookup"><span data-stu-id="0b69a-118">string</span></span>|<span data-ttu-id="0b69a-p102">Representa as opções de classificação adicionais para esse campo. Os valores possíveis são: `Normal` e `TextAsNumber`.</span><span class="sxs-lookup"><span data-stu-id="0b69a-p102">Represents additional sorting options for this field. Possible values are: `Normal`, `TextAsNumber`.</span></span>|
|<span data-ttu-id="0b69a-121">key</span><span class="sxs-lookup"><span data-stu-id="0b69a-121">key</span></span>|<span data-ttu-id="0b69a-122">int</span><span class="sxs-lookup"><span data-stu-id="0b69a-122">int</span></span>|<span data-ttu-id="0b69a-p103">Representa a coluna (ou linha, dependendo da orientação da classificação) em que a condição está. Representado como um deslocamento da primeira coluna (ou linha).</span><span class="sxs-lookup"><span data-stu-id="0b69a-p103">Represents the column (or row, depending on the sort orientation) that the condition is on. Represented as an offset from the first column (or row).</span></span>|
|<span data-ttu-id="0b69a-125">sortOn</span><span class="sxs-lookup"><span data-stu-id="0b69a-125">sortOn</span></span>|<span data-ttu-id="0b69a-126">string</span><span class="sxs-lookup"><span data-stu-id="0b69a-126">string</span></span>|<span data-ttu-id="0b69a-p104">Representa o tipo de classificação dessa condição. Os valores possíveis são: `Value`, `CellColor`, `FontColor` e `Icon`.</span><span class="sxs-lookup"><span data-stu-id="0b69a-p104">Represents the type of sorting of this condition. Possible values are: `Value`, `CellColor`, `FontColor`, `Icon`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0b69a-129">Relações</span><span class="sxs-lookup"><span data-stu-id="0b69a-129">Relationships</span></span>
| <span data-ttu-id="0b69a-130">Relação</span><span class="sxs-lookup"><span data-stu-id="0b69a-130">Relationship</span></span> | <span data-ttu-id="0b69a-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="0b69a-131">Type</span></span>   |<span data-ttu-id="0b69a-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="0b69a-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0b69a-133">ícone</span><span class="sxs-lookup"><span data-stu-id="0b69a-133">icon</span></span>|[<span data-ttu-id="0b69a-134">Icon</span><span class="sxs-lookup"><span data-stu-id="0b69a-134">Icon</span></span>](icon.md)|<span data-ttu-id="0b69a-135">Representa o ícone que é o destino da condição se a classificação está no ícone da célula.</span><span class="sxs-lookup"><span data-stu-id="0b69a-135">Represents the icon that is the target of the condition if the sorting is on the cell's icon.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0b69a-136">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0b69a-136">JSON representation</span></span>

<span data-ttu-id="0b69a-137">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0b69a-137">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "SortField resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
