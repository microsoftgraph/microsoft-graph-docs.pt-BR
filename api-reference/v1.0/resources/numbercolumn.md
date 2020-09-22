---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: NumberColumn
localization_priority: Normal
description: O recurso numberColumn em um recurso columnDefinition indica que os valores da coluna são números.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: f2d8955ac71a7a6e9979542f08e4d0634274b69b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48083019"
---
# <a name="numbercolumn-resource-type"></a><span data-ttu-id="19cc5-103">Tipo de recurso NumberColumn</span><span class="sxs-lookup"><span data-stu-id="19cc5-103">NumberColumn resource type</span></span>

<span data-ttu-id="19cc5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="19cc5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="19cc5-105">O recurso **numberColumn** em um recurso [columnDefinition](columndefinition.md) indica que os valores da coluna são números.</span><span class="sxs-lookup"><span data-stu-id="19cc5-105">The **numberColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are numbers.</span></span>

## <a name="json-representation"></a><span data-ttu-id="19cc5-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="19cc5-106">JSON representation</span></span>

<span data-ttu-id="19cc5-107">Aqui está uma representação JSON de um recurso **numberColumn**.</span><span class="sxs-lookup"><span data-stu-id="19cc5-107">Here is a JSON representation of a **numberColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.numberColumn" } -->

```json
{
  "decimalPlaces": "automatic | none | one | two | three | four | five",
  "displayAs": "number | percentage",
  "maximum": 10.551,
  "minimum": 99.993
}
```

## <a name="properties"></a><span data-ttu-id="19cc5-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="19cc5-108">Properties</span></span>

| <span data-ttu-id="19cc5-109">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="19cc5-109">Property name</span></span>      | <span data-ttu-id="19cc5-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="19cc5-110">Type</span></span>   | <span data-ttu-id="19cc5-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="19cc5-111">Description</span></span>
|:-------------------|:-------|:-----------------------------------------------
| <span data-ttu-id="19cc5-112">**decimalPlaces**</span><span class="sxs-lookup"><span data-stu-id="19cc5-112">**decimalPlaces**</span></span>  | <span data-ttu-id="19cc5-113">string</span><span class="sxs-lookup"><span data-stu-id="19cc5-113">string</span></span> | <span data-ttu-id="19cc5-114">Quantas casas decimais exibir.</span><span class="sxs-lookup"><span data-stu-id="19cc5-114">How many decimal places to display.</span></span> <span data-ttu-id="19cc5-115">Consulte abaixo para saber mais sobre os valores possíveis.</span><span class="sxs-lookup"><span data-stu-id="19cc5-115">See below for information about the possible values.</span></span>
| <span data-ttu-id="19cc5-116">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="19cc5-116">**displayAs**</span></span>      | <span data-ttu-id="19cc5-117">string</span><span class="sxs-lookup"><span data-stu-id="19cc5-117">string</span></span> | <span data-ttu-id="19cc5-118">Como o valor deve ser apresentado na experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="19cc5-118">How the value should be presented in the UX.</span></span> <span data-ttu-id="19cc5-119">Deve ser `number` ou `percentage`.</span><span class="sxs-lookup"><span data-stu-id="19cc5-119">Must be one of `number` or `percentage`.</span></span> <span data-ttu-id="19cc5-120">Se não for especificado, é tratado como `number`.</span><span class="sxs-lookup"><span data-stu-id="19cc5-120">If unspecified, treated as `number`.</span></span>
| <span data-ttu-id="19cc5-121">**maximum**</span><span class="sxs-lookup"><span data-stu-id="19cc5-121">**maximum**</span></span>        | <span data-ttu-id="19cc5-122">double</span><span class="sxs-lookup"><span data-stu-id="19cc5-122">double</span></span> | <span data-ttu-id="19cc5-123">O valor máximo permitido.</span><span class="sxs-lookup"><span data-stu-id="19cc5-123">The maximum permitted value.</span></span>
| <span data-ttu-id="19cc5-124">**minimum**</span><span class="sxs-lookup"><span data-stu-id="19cc5-124">**minimum**</span></span>        | <span data-ttu-id="19cc5-125">double</span><span class="sxs-lookup"><span data-stu-id="19cc5-125">double</span></span> | <span data-ttu-id="19cc5-126">O valor mínimo permitido.</span><span class="sxs-lookup"><span data-stu-id="19cc5-126">The minimum permitted value.</span></span>

## <a name="decimalplaces"></a><span data-ttu-id="19cc5-127">DecimalPlaces</span><span class="sxs-lookup"><span data-stu-id="19cc5-127">DecimalPlaces</span></span>

| <span data-ttu-id="19cc5-128">Valor</span><span class="sxs-lookup"><span data-stu-id="19cc5-128">Value</span></span>          | <span data-ttu-id="19cc5-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="19cc5-129">Description</span></span>
|:---------------|:--------------------------------------------------------------
| <span data-ttu-id="19cc5-130">**automatic**</span><span class="sxs-lookup"><span data-stu-id="19cc5-130">**automatic**</span></span>  | <span data-ttu-id="19cc5-131">Padrão.</span><span class="sxs-lookup"><span data-stu-id="19cc5-131">Default.</span></span> <span data-ttu-id="19cc5-132">Exibir casas decimais automaticamente conforme necessário.</span><span class="sxs-lookup"><span data-stu-id="19cc5-132">Automatically display decimal places as needed.</span></span>
| <span data-ttu-id="19cc5-133">**none**</span><span class="sxs-lookup"><span data-stu-id="19cc5-133">**none**</span></span>       | <span data-ttu-id="19cc5-134">Não exibir casas decimais.</span><span class="sxs-lookup"><span data-stu-id="19cc5-134">Do not display any decimal places.</span></span>
| <span data-ttu-id="19cc5-135">**one**</span><span class="sxs-lookup"><span data-stu-id="19cc5-135">**one**</span></span>        | <span data-ttu-id="19cc5-136">Exibir sempre uma casa decimal.</span><span class="sxs-lookup"><span data-stu-id="19cc5-136">Always display one decimal place.</span></span>
| <span data-ttu-id="19cc5-137">**two**</span><span class="sxs-lookup"><span data-stu-id="19cc5-137">**two**</span></span>        | <span data-ttu-id="19cc5-138">Exibir sempre duas casas decimais.</span><span class="sxs-lookup"><span data-stu-id="19cc5-138">Always display two decimal places.</span></span>
| <span data-ttu-id="19cc5-139">**three**</span><span class="sxs-lookup"><span data-stu-id="19cc5-139">**three**</span></span>      | <span data-ttu-id="19cc5-140">Exibir sempre três casas decimais.</span><span class="sxs-lookup"><span data-stu-id="19cc5-140">Always display three decimal places.</span></span>
| <span data-ttu-id="19cc5-141">**four**</span><span class="sxs-lookup"><span data-stu-id="19cc5-141">**four**</span></span>       | <span data-ttu-id="19cc5-142">Exibir sempre quatro casas decimais.</span><span class="sxs-lookup"><span data-stu-id="19cc5-142">Always display four decimal places.</span></span>
| <span data-ttu-id="19cc5-143">**five**</span><span class="sxs-lookup"><span data-stu-id="19cc5-143">**five**</span></span>       | <span data-ttu-id="19cc5-144">Exibir sempre cinco casas decimais.</span><span class="sxs-lookup"><span data-stu-id="19cc5-144">Always display five decimal places.</span></span>

<span data-ttu-id="19cc5-145">Observação: **decimalPlaces** e **displayAs** aplicam-se a como os números são processados, não armazenados.</span><span class="sxs-lookup"><span data-stu-id="19cc5-145">Note: **decimalPlaces** and **displayAs** apply to how numbers are rendered, not stored.</span></span>
<span data-ttu-id="19cc5-146">Essas propriedades podem ser atualizadas.</span><span class="sxs-lookup"><span data-stu-id="19cc5-146">These properties may be updated.</span></span>

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

