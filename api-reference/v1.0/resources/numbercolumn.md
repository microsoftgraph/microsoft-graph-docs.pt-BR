---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: NumberColumn
ms.openlocfilehash: 4aaff6539fc9c7ce77029463562c0f8fca57cac6
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/21/2018
ms.locfileid: "23266503"
---
# <a name="numbercolumn-resource-type"></a><span data-ttu-id="049a4-102">Tipo de recurso NumberColumn</span><span class="sxs-lookup"><span data-stu-id="049a4-102">NumberColumn resource type</span></span>

<span data-ttu-id="049a4-103">O recurso **numberColumn** em um recurso [columnDefinition](columnDefinition.md) indica que os valores da coluna são números.</span><span class="sxs-lookup"><span data-stu-id="049a4-103">The **numberColumn** on a [columnDefinition](columnDefinition.md) resource indicates that the column's values are numbers.</span></span>

## <a name="json-representation"></a><span data-ttu-id="049a4-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="049a4-104">JSON representation</span></span>

<span data-ttu-id="049a4-105">Aqui está uma representação JSON de um recurso **numberColumn**.</span><span class="sxs-lookup"><span data-stu-id="049a4-105">Here is a JSON representation of a **numberColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.numberColumn" } -->

```json
{
  "decimalPlaces": "automatic | none | one | two | three | four | five",
  "displayAs": "number | percentage",
  "maximum": 10.551,
  "minimum": 99.993
}
```

## <a name="properties"></a><span data-ttu-id="049a4-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="049a4-106">Properties</span></span>

| <span data-ttu-id="049a4-107">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="049a4-107">Property name</span></span>      | <span data-ttu-id="049a4-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="049a4-108">Type</span></span>   | <span data-ttu-id="049a4-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="049a4-109">Description</span></span>
|:-------------------|:-------|:-----------------------------------------------
| <span data-ttu-id="049a4-110">**decimalPlaces**</span><span class="sxs-lookup"><span data-stu-id="049a4-110">**decimalPlaces**</span></span>  | <span data-ttu-id="049a4-111">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="049a4-111">string</span></span> | <span data-ttu-id="049a4-112">Quantas casas decimais exibir.</span><span class="sxs-lookup"><span data-stu-id="049a4-112">How many decimal places to display.</span></span> <span data-ttu-id="049a4-113">Consulte abaixo para saber mais sobre os valores possíveis.</span><span class="sxs-lookup"><span data-stu-id="049a4-113">See below for information about the possible values.</span></span>
| <span data-ttu-id="049a4-114">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="049a4-114">**displayAs**</span></span>      | <span data-ttu-id="049a4-115">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="049a4-115">string</span></span> | <span data-ttu-id="049a4-116">Como o valor deve ser apresentado na experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="049a4-116">How the value should be presented in the UX.</span></span> <span data-ttu-id="049a4-117">Deve ser `number` ou `percentage`.</span><span class="sxs-lookup"><span data-stu-id="049a4-117">Must be one of `number` or `percentage`.</span></span> <span data-ttu-id="049a4-118">Se não for especificado, é tratado como `number`.</span><span class="sxs-lookup"><span data-stu-id="049a4-118">If unspecified, treated as `number`.</span></span>
| <span data-ttu-id="049a4-119">**máximo**</span><span class="sxs-lookup"><span data-stu-id="049a4-119">**maximum**</span></span>        | <span data-ttu-id="049a4-120">double</span><span class="sxs-lookup"><span data-stu-id="049a4-120">double</span></span> | <span data-ttu-id="049a4-121">O valor máximo permitido.</span><span class="sxs-lookup"><span data-stu-id="049a4-121">The maximum permitted value.</span></span>
| <span data-ttu-id="049a4-122">**mínimo**</span><span class="sxs-lookup"><span data-stu-id="049a4-122">**minimum**</span></span>        | <span data-ttu-id="049a4-123">double</span><span class="sxs-lookup"><span data-stu-id="049a4-123">double</span></span> | <span data-ttu-id="049a4-124">O valor mínimo permitido.</span><span class="sxs-lookup"><span data-stu-id="049a4-124">The minimum permitted value.</span></span>

## <a name="decimalplaces"></a><span data-ttu-id="049a4-125">DecimalPlaces</span><span class="sxs-lookup"><span data-stu-id="049a4-125">DecimalPlaces</span></span>

| <span data-ttu-id="049a4-126">Valor</span><span class="sxs-lookup"><span data-stu-id="049a4-126">Value</span></span>          | <span data-ttu-id="049a4-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="049a4-127">Description</span></span>
|:---------------|:--------------------------------------------------------------
| <span data-ttu-id="049a4-128">**automático**</span><span class="sxs-lookup"><span data-stu-id="049a4-128">**automatic**</span></span>  | <span data-ttu-id="049a4-129">Padrão.</span><span class="sxs-lookup"><span data-stu-id="049a4-129">Default.</span></span> <span data-ttu-id="049a4-130">Exibir casas decimais automaticamente conforme necessário.</span><span class="sxs-lookup"><span data-stu-id="049a4-130">Automatically display decimal places as needed.</span></span>
| <span data-ttu-id="049a4-131">**nenhum**</span><span class="sxs-lookup"><span data-stu-id="049a4-131">**none**</span></span>       | <span data-ttu-id="049a4-132">Não exibir casas decimais.</span><span class="sxs-lookup"><span data-stu-id="049a4-132">Do not display any decimal places.</span></span>
| <span data-ttu-id="049a4-133">**um**</span><span class="sxs-lookup"><span data-stu-id="049a4-133">**one**</span></span>        | <span data-ttu-id="049a4-134">Exibir sempre uma casa decimal.</span><span class="sxs-lookup"><span data-stu-id="049a4-134">Always display one decimal place.</span></span>
| <span data-ttu-id="049a4-135">**dois**</span><span class="sxs-lookup"><span data-stu-id="049a4-135">**two**</span></span>        | <span data-ttu-id="049a4-136">Exibir sempre duas casas decimais.</span><span class="sxs-lookup"><span data-stu-id="049a4-136">Always display two decimal places.</span></span>
| <span data-ttu-id="049a4-137">**três**</span><span class="sxs-lookup"><span data-stu-id="049a4-137">**three**</span></span>      | <span data-ttu-id="049a4-138">Exibir sempre três casas decimais.</span><span class="sxs-lookup"><span data-stu-id="049a4-138">Always display three decimal places.</span></span>
| <span data-ttu-id="049a4-139">**quatro**</span><span class="sxs-lookup"><span data-stu-id="049a4-139">**four**</span></span>       | <span data-ttu-id="049a4-140">Exibir sempre quatro casas decimais.</span><span class="sxs-lookup"><span data-stu-id="049a4-140">Always display four decimal places.</span></span>
| <span data-ttu-id="049a4-141">**cinco**</span><span class="sxs-lookup"><span data-stu-id="049a4-141">**five**</span></span>       | <span data-ttu-id="049a4-142">Exibir sempre cinco casas decimais.</span><span class="sxs-lookup"><span data-stu-id="049a4-142">Always display five decimal places.</span></span>

<span data-ttu-id="049a4-143">Observação: **decimalPlaces** e **displayAs** aplicam-se a como os números são processados, não armazenados.</span><span class="sxs-lookup"><span data-stu-id="049a4-143">Note: **decimalPlaces** and **displayAs** apply to how numbers are rendered, not stored.</span></span>
<span data-ttu-id="049a4-144">Essas propriedades podem ser atualizadas.</span><span class="sxs-lookup"><span data-stu-id="049a4-144">These properties may be updated.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/numbercolumn.md:
      Found potential enums in resource example that weren't defined in a table:(automatic,none,one,two,three,four,five) are in resource, but () are in table",
    "Warning: /api-reference/v1.0/resources/numbercolumn.md:
      Found potential enums in resource example that weren't defined in a table:(number,percentage) are in resource, but () are in table"
  ],
  "tocPath": "Resources/NumberColumn"
} -->
