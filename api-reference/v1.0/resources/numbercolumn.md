---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: NumberColumn
localization_priority: Normal
description: O recurso numberColumn em um recurso columnDefinition indica que os valores da coluna são números.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 9196e2508ed3109ee56c24ad72943ca50aed11bc
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035964"
---
# <a name="numbercolumn-resource-type"></a><span data-ttu-id="604d2-103">Tipo de recurso NumberColumn</span><span class="sxs-lookup"><span data-stu-id="604d2-103">NumberColumn resource type</span></span>

<span data-ttu-id="604d2-104">O recurso **numberColumn** em um recurso [columnDefinition](columndefinition.md) indica que os valores da coluna são números.</span><span class="sxs-lookup"><span data-stu-id="604d2-104">The **numberColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are numbers.</span></span>

## <a name="json-representation"></a><span data-ttu-id="604d2-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="604d2-105">JSON representation</span></span>

<span data-ttu-id="604d2-106">Aqui está uma representação JSON de um recurso **numberColumn**.</span><span class="sxs-lookup"><span data-stu-id="604d2-106">Here is a JSON representation of a **numberColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.numberColumn" } -->

```json
{
  "decimalPlaces": "automatic | none | one | two | three | four | five",
  "displayAs": "number | percentage",
  "maximum": 10.551,
  "minimum": 99.993
}
```

## <a name="properties"></a><span data-ttu-id="604d2-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="604d2-107">Properties</span></span>

| <span data-ttu-id="604d2-108">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="604d2-108">Property name</span></span>      | <span data-ttu-id="604d2-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="604d2-109">Type</span></span>   | <span data-ttu-id="604d2-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="604d2-110">Description</span></span>
|:-------------------|:-------|:-----------------------------------------------
| <span data-ttu-id="604d2-111">**decimalPlaces**</span><span class="sxs-lookup"><span data-stu-id="604d2-111">**decimalPlaces**</span></span>  | <span data-ttu-id="604d2-112">string</span><span class="sxs-lookup"><span data-stu-id="604d2-112">string</span></span> | <span data-ttu-id="604d2-113">Quantas casas decimais exibir.</span><span class="sxs-lookup"><span data-stu-id="604d2-113">How many decimal places to display.</span></span> <span data-ttu-id="604d2-114">Consulte abaixo para saber mais sobre os valores possíveis.</span><span class="sxs-lookup"><span data-stu-id="604d2-114">See below for information about the possible values.</span></span>
| <span data-ttu-id="604d2-115">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="604d2-115">**displayAs**</span></span>      | <span data-ttu-id="604d2-116">string</span><span class="sxs-lookup"><span data-stu-id="604d2-116">string</span></span> | <span data-ttu-id="604d2-117">Como o valor deve ser apresentado na experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="604d2-117">How the value should be presented in the UX.</span></span> <span data-ttu-id="604d2-118">Deve ser `number` ou `percentage`.</span><span class="sxs-lookup"><span data-stu-id="604d2-118">Must be one of `number` or `percentage`.</span></span> <span data-ttu-id="604d2-119">Se não for especificado, é tratado como `number`.</span><span class="sxs-lookup"><span data-stu-id="604d2-119">If unspecified, treated as `number`.</span></span>
| <span data-ttu-id="604d2-120">**maximum**</span><span class="sxs-lookup"><span data-stu-id="604d2-120">**maximum**</span></span>        | <span data-ttu-id="604d2-121">double</span><span class="sxs-lookup"><span data-stu-id="604d2-121">double</span></span> | <span data-ttu-id="604d2-122">O valor máximo permitido.</span><span class="sxs-lookup"><span data-stu-id="604d2-122">The maximum permitted value.</span></span>
| <span data-ttu-id="604d2-123">**minimum**</span><span class="sxs-lookup"><span data-stu-id="604d2-123">**minimum**</span></span>        | <span data-ttu-id="604d2-124">double</span><span class="sxs-lookup"><span data-stu-id="604d2-124">double</span></span> | <span data-ttu-id="604d2-125">O valor mínimo permitido.</span><span class="sxs-lookup"><span data-stu-id="604d2-125">The minimum permitted value.</span></span>

## <a name="decimalplaces"></a><span data-ttu-id="604d2-126">DecimalPlaces</span><span class="sxs-lookup"><span data-stu-id="604d2-126">DecimalPlaces</span></span>

| <span data-ttu-id="604d2-127">Valor</span><span class="sxs-lookup"><span data-stu-id="604d2-127">Value</span></span>          | <span data-ttu-id="604d2-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="604d2-128">Description</span></span>
|:---------------|:--------------------------------------------------------------
| <span data-ttu-id="604d2-129">**automatic**</span><span class="sxs-lookup"><span data-stu-id="604d2-129">**automatic**</span></span>  | <span data-ttu-id="604d2-130">Padrão.</span><span class="sxs-lookup"><span data-stu-id="604d2-130">Default.</span></span> <span data-ttu-id="604d2-131">Exibir casas decimais automaticamente conforme necessário.</span><span class="sxs-lookup"><span data-stu-id="604d2-131">Automatically display decimal places as needed.</span></span>
| <span data-ttu-id="604d2-132">**none**</span><span class="sxs-lookup"><span data-stu-id="604d2-132">**none**</span></span>       | <span data-ttu-id="604d2-133">Não exibir casas decimais.</span><span class="sxs-lookup"><span data-stu-id="604d2-133">Do not display any decimal places.</span></span>
| <span data-ttu-id="604d2-134">**one**</span><span class="sxs-lookup"><span data-stu-id="604d2-134">**one**</span></span>        | <span data-ttu-id="604d2-135">Exibir sempre uma casa decimal.</span><span class="sxs-lookup"><span data-stu-id="604d2-135">Always display one decimal place.</span></span>
| <span data-ttu-id="604d2-136">**two**</span><span class="sxs-lookup"><span data-stu-id="604d2-136">**two**</span></span>        | <span data-ttu-id="604d2-137">Exibir sempre duas casas decimais.</span><span class="sxs-lookup"><span data-stu-id="604d2-137">Always display two decimal places.</span></span>
| <span data-ttu-id="604d2-138">**three**</span><span class="sxs-lookup"><span data-stu-id="604d2-138">**three**</span></span>      | <span data-ttu-id="604d2-139">Exibir sempre três casas decimais.</span><span class="sxs-lookup"><span data-stu-id="604d2-139">Always display three decimal places.</span></span>
| <span data-ttu-id="604d2-140">**four**</span><span class="sxs-lookup"><span data-stu-id="604d2-140">**four**</span></span>       | <span data-ttu-id="604d2-141">Exibir sempre quatro casas decimais.</span><span class="sxs-lookup"><span data-stu-id="604d2-141">Always display four decimal places.</span></span>
| <span data-ttu-id="604d2-142">**five**</span><span class="sxs-lookup"><span data-stu-id="604d2-142">**five**</span></span>       | <span data-ttu-id="604d2-143">Exibir sempre cinco casas decimais.</span><span class="sxs-lookup"><span data-stu-id="604d2-143">Always display five decimal places.</span></span>

<span data-ttu-id="604d2-144">Observação: **decimalPlaces** e **displayAs** aplicam-se a como os números são processados, não armazenados.</span><span class="sxs-lookup"><span data-stu-id="604d2-144">Note: **decimalPlaces** and **displayAs** apply to how numbers are rendered, not stored.</span></span>
<span data-ttu-id="604d2-145">Essas propriedades podem ser atualizadas.</span><span class="sxs-lookup"><span data-stu-id="604d2-145">These properties may be updated.</span></span>

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
