---
author: JeremyKelley
ms.date: 09/11/2017
title: NumberColumn
localization_priority: Normal
description: O recurso numberColumn em um recurso columnDefinition indica que os valores da coluna são números.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 89b5c81f94895e248dfd4c5f75983bacf352f9e8
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/14/2021
ms.locfileid: "50238628"
---
# <a name="numbercolumn-resource-type"></a><span data-ttu-id="8d93a-103">Tipo de recurso NumberColumn</span><span class="sxs-lookup"><span data-stu-id="8d93a-103">NumberColumn resource type</span></span>

<span data-ttu-id="8d93a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8d93a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8d93a-105">O recurso **numberColumn** em um recurso [columnDefinition](columndefinition.md) indica que os valores da coluna são números.</span><span class="sxs-lookup"><span data-stu-id="8d93a-105">The **numberColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are numbers.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8d93a-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8d93a-106">JSON representation</span></span>

<span data-ttu-id="8d93a-107">Aqui está uma representação JSON de um recurso **numberColumn**.</span><span class="sxs-lookup"><span data-stu-id="8d93a-107">Here is a JSON representation of a **numberColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.numberColumn" } -->

```json
{
  "decimalPlaces": "automatic | none | one | two | three | four | five",
  "displayAs": "number | percentage",
  "maximum": 10.551,
  "minimum": 99.993
}
```

## <a name="properties"></a><span data-ttu-id="8d93a-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8d93a-108">Properties</span></span>

| <span data-ttu-id="8d93a-109">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="8d93a-109">Property name</span></span>      | <span data-ttu-id="8d93a-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="8d93a-110">Type</span></span>   | <span data-ttu-id="8d93a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="8d93a-111">Description</span></span>
|:-------------------|:-------|:-----------------------------------------------
| <span data-ttu-id="8d93a-112">**decimalPlaces**</span><span class="sxs-lookup"><span data-stu-id="8d93a-112">**decimalPlaces**</span></span>  | <span data-ttu-id="8d93a-113">string</span><span class="sxs-lookup"><span data-stu-id="8d93a-113">string</span></span> | <span data-ttu-id="8d93a-114">Quantas casas decimais exibir.</span><span class="sxs-lookup"><span data-stu-id="8d93a-114">How many decimal places to display.</span></span> <span data-ttu-id="8d93a-115">Consulte abaixo para saber mais sobre os valores possíveis.</span><span class="sxs-lookup"><span data-stu-id="8d93a-115">See below for information about the possible values.</span></span>
| <span data-ttu-id="8d93a-116">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="8d93a-116">**displayAs**</span></span>      | <span data-ttu-id="8d93a-117">string</span><span class="sxs-lookup"><span data-stu-id="8d93a-117">string</span></span> | <span data-ttu-id="8d93a-118">Como o valor deve ser apresentado na experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="8d93a-118">How the value should be presented in the UX.</span></span> <span data-ttu-id="8d93a-119">Deve ser `number` ou `percentage`.</span><span class="sxs-lookup"><span data-stu-id="8d93a-119">Must be one of `number` or `percentage`.</span></span> <span data-ttu-id="8d93a-120">Se não for especificado, é tratado como `number`.</span><span class="sxs-lookup"><span data-stu-id="8d93a-120">If unspecified, treated as `number`.</span></span>
| <span data-ttu-id="8d93a-121">**maximum**</span><span class="sxs-lookup"><span data-stu-id="8d93a-121">**maximum**</span></span>        | <span data-ttu-id="8d93a-122">double</span><span class="sxs-lookup"><span data-stu-id="8d93a-122">double</span></span> | <span data-ttu-id="8d93a-123">O valor máximo permitido.</span><span class="sxs-lookup"><span data-stu-id="8d93a-123">The maximum permitted value.</span></span>
| <span data-ttu-id="8d93a-124">**minimum**</span><span class="sxs-lookup"><span data-stu-id="8d93a-124">**minimum**</span></span>        | <span data-ttu-id="8d93a-125">double</span><span class="sxs-lookup"><span data-stu-id="8d93a-125">double</span></span> | <span data-ttu-id="8d93a-126">O valor mínimo permitido.</span><span class="sxs-lookup"><span data-stu-id="8d93a-126">The minimum permitted value.</span></span>

## <a name="decimalplaces"></a><span data-ttu-id="8d93a-127">DecimalPlaces</span><span class="sxs-lookup"><span data-stu-id="8d93a-127">DecimalPlaces</span></span>

| <span data-ttu-id="8d93a-128">Valor</span><span class="sxs-lookup"><span data-stu-id="8d93a-128">Value</span></span>          | <span data-ttu-id="8d93a-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="8d93a-129">Description</span></span>
|:---------------|:--------------------------------------------------------------
| <span data-ttu-id="8d93a-130">**automatic**</span><span class="sxs-lookup"><span data-stu-id="8d93a-130">**automatic**</span></span>  | <span data-ttu-id="8d93a-131">Padrão.</span><span class="sxs-lookup"><span data-stu-id="8d93a-131">Default.</span></span> <span data-ttu-id="8d93a-132">Exibir casas decimais automaticamente conforme necessário.</span><span class="sxs-lookup"><span data-stu-id="8d93a-132">Automatically display decimal places as needed.</span></span>
| <span data-ttu-id="8d93a-133">**none**</span><span class="sxs-lookup"><span data-stu-id="8d93a-133">**none**</span></span>       | <span data-ttu-id="8d93a-134">Não exibir casas decimais.</span><span class="sxs-lookup"><span data-stu-id="8d93a-134">Do not display any decimal places.</span></span>
| <span data-ttu-id="8d93a-135">**one**</span><span class="sxs-lookup"><span data-stu-id="8d93a-135">**one**</span></span>        | <span data-ttu-id="8d93a-136">Exibir sempre uma casa decimal.</span><span class="sxs-lookup"><span data-stu-id="8d93a-136">Always display one decimal place.</span></span>
| <span data-ttu-id="8d93a-137">**two**</span><span class="sxs-lookup"><span data-stu-id="8d93a-137">**two**</span></span>        | <span data-ttu-id="8d93a-138">Exibir sempre duas casas decimais.</span><span class="sxs-lookup"><span data-stu-id="8d93a-138">Always display two decimal places.</span></span>
| <span data-ttu-id="8d93a-139">**three**</span><span class="sxs-lookup"><span data-stu-id="8d93a-139">**three**</span></span>      | <span data-ttu-id="8d93a-140">Exibir sempre três casas decimais.</span><span class="sxs-lookup"><span data-stu-id="8d93a-140">Always display three decimal places.</span></span>
| <span data-ttu-id="8d93a-141">**four**</span><span class="sxs-lookup"><span data-stu-id="8d93a-141">**four**</span></span>       | <span data-ttu-id="8d93a-142">Exibir sempre quatro casas decimais.</span><span class="sxs-lookup"><span data-stu-id="8d93a-142">Always display four decimal places.</span></span>
| <span data-ttu-id="8d93a-143">**five**</span><span class="sxs-lookup"><span data-stu-id="8d93a-143">**five**</span></span>       | <span data-ttu-id="8d93a-144">Exibir sempre cinco casas decimais.</span><span class="sxs-lookup"><span data-stu-id="8d93a-144">Always display five decimal places.</span></span>

<span data-ttu-id="8d93a-145">Observação: **decimalPlaces** e **displayAs** aplicam-se a como os números são processados, não armazenados.</span><span class="sxs-lookup"><span data-stu-id="8d93a-145">Note: **decimalPlaces** and **displayAs** apply to how numbers are rendered, not stored.</span></span>
<span data-ttu-id="8d93a-146">Essas propriedades podem ser atualizadas.</span><span class="sxs-lookup"><span data-stu-id="8d93a-146">These properties may be updated.</span></span>

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

