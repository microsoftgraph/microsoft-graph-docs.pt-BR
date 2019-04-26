---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: NumberColumn
localization_priority: Normal
ms.openlocfilehash: f70a1d71729be68fc4d5dcb3de2599ff131bb8a9
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342090"
---
# <a name="numbercolumn-resource-type"></a><span data-ttu-id="59f84-102">Tipo de recurso NumberColumn</span><span class="sxs-lookup"><span data-stu-id="59f84-102">NumberColumn resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="59f84-103">O recurso **numberColumn** em um recurso [columnDefinition](columndefinition.md) indica que os valores da coluna são números.</span><span class="sxs-lookup"><span data-stu-id="59f84-103">The **numberColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are numbers.</span></span>

## <a name="json-representation"></a><span data-ttu-id="59f84-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="59f84-104">JSON representation</span></span>

<span data-ttu-id="59f84-105">Aqui está uma representação JSON de um recurso **numberColumn**.</span><span class="sxs-lookup"><span data-stu-id="59f84-105">Here is a JSON representation of a **numberColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.numberColumn" } -->

```json
{
  "decimalPlaces": "automatic | none | one | two | three | four | five",
  "displayAs": "number | percentage",
  "maximum": 10.551,
  "minimum": 99.993
}
```

## <a name="properties"></a><span data-ttu-id="59f84-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="59f84-106">Properties</span></span>

| <span data-ttu-id="59f84-107">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="59f84-107">Property name</span></span>      | <span data-ttu-id="59f84-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="59f84-108">Type</span></span>   | <span data-ttu-id="59f84-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="59f84-109">Description</span></span>
|:-------------------|:-------|:-----------------------------------------------
| <span data-ttu-id="59f84-110">**decimalPlaces**</span><span class="sxs-lookup"><span data-stu-id="59f84-110">**decimalPlaces**</span></span>  | <span data-ttu-id="59f84-111">string</span><span class="sxs-lookup"><span data-stu-id="59f84-111">string</span></span> | <span data-ttu-id="59f84-112">Quantas casas decimais exibir.</span><span class="sxs-lookup"><span data-stu-id="59f84-112">How many decimal places to display.</span></span> <span data-ttu-id="59f84-113">Consulte abaixo para saber mais sobre os valores possíveis.</span><span class="sxs-lookup"><span data-stu-id="59f84-113">See below for information about the possible values.</span></span>
| <span data-ttu-id="59f84-114">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="59f84-114">**displayAs**</span></span>      | <span data-ttu-id="59f84-115">string</span><span class="sxs-lookup"><span data-stu-id="59f84-115">string</span></span> | <span data-ttu-id="59f84-116">Como o valor deve ser apresentado na experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="59f84-116">How the value should be presented in the UX.</span></span> <span data-ttu-id="59f84-117">Deve ser `number` ou `percentage`.</span><span class="sxs-lookup"><span data-stu-id="59f84-117">Must be one of `number` or `percentage`.</span></span> <span data-ttu-id="59f84-118">Se não for especificado, é tratado como `number`.</span><span class="sxs-lookup"><span data-stu-id="59f84-118">If unspecified, treated as `number`.</span></span>
| <span data-ttu-id="59f84-119">**maximum**</span><span class="sxs-lookup"><span data-stu-id="59f84-119">**maximum**</span></span>        | <span data-ttu-id="59f84-120">double</span><span class="sxs-lookup"><span data-stu-id="59f84-120">double</span></span> | <span data-ttu-id="59f84-121">O valor máximo permitido.</span><span class="sxs-lookup"><span data-stu-id="59f84-121">The maximum permitted value.</span></span>
| <span data-ttu-id="59f84-122">**minimum**</span><span class="sxs-lookup"><span data-stu-id="59f84-122">**minimum**</span></span>        | <span data-ttu-id="59f84-123">double</span><span class="sxs-lookup"><span data-stu-id="59f84-123">double</span></span> | <span data-ttu-id="59f84-124">O valor mínimo permitido.</span><span class="sxs-lookup"><span data-stu-id="59f84-124">The minimum permitted value.</span></span>

## <a name="decimalplaces-values"></a><span data-ttu-id="59f84-125">Valores de DecimalPlaces</span><span class="sxs-lookup"><span data-stu-id="59f84-125">DecimalPlaces values</span></span>

| <span data-ttu-id="59f84-126">Valor</span><span class="sxs-lookup"><span data-stu-id="59f84-126">Value</span></span>          | <span data-ttu-id="59f84-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="59f84-127">Description</span></span>
|:---------------|:--------------------------------------------------------------
| <span data-ttu-id="59f84-128">**automatic**</span><span class="sxs-lookup"><span data-stu-id="59f84-128">**automatic**</span></span>  | <span data-ttu-id="59f84-129">Padrão.</span><span class="sxs-lookup"><span data-stu-id="59f84-129">Default.</span></span> <span data-ttu-id="59f84-130">Exibir casas decimais automaticamente conforme necessário.</span><span class="sxs-lookup"><span data-stu-id="59f84-130">Automatically display decimal places as needed.</span></span>
| <span data-ttu-id="59f84-131">**none**</span><span class="sxs-lookup"><span data-stu-id="59f84-131">**none**</span></span>       | <span data-ttu-id="59f84-132">Não exibir casas decimais.</span><span class="sxs-lookup"><span data-stu-id="59f84-132">Do not display any decimal places.</span></span>
| <span data-ttu-id="59f84-133">**one**</span><span class="sxs-lookup"><span data-stu-id="59f84-133">**one**</span></span>        | <span data-ttu-id="59f84-134">Exibir sempre uma casa decimal.</span><span class="sxs-lookup"><span data-stu-id="59f84-134">Always display one decimal place.</span></span>
| <span data-ttu-id="59f84-135">**two**</span><span class="sxs-lookup"><span data-stu-id="59f84-135">**two**</span></span>        | <span data-ttu-id="59f84-136">Exibir sempre duas casas decimais.</span><span class="sxs-lookup"><span data-stu-id="59f84-136">Always display two decimal places.</span></span>
| <span data-ttu-id="59f84-137">**three**</span><span class="sxs-lookup"><span data-stu-id="59f84-137">**three**</span></span>      | <span data-ttu-id="59f84-138">Exibir sempre três casas decimais.</span><span class="sxs-lookup"><span data-stu-id="59f84-138">Always display three decimal places.</span></span>
| <span data-ttu-id="59f84-139">**four**</span><span class="sxs-lookup"><span data-stu-id="59f84-139">**four**</span></span>       | <span data-ttu-id="59f84-140">Exibir sempre quatro casas decimais.</span><span class="sxs-lookup"><span data-stu-id="59f84-140">Always display four decimal places.</span></span>
| <span data-ttu-id="59f84-141">**five**</span><span class="sxs-lookup"><span data-stu-id="59f84-141">**five**</span></span>       | <span data-ttu-id="59f84-142">Exibir sempre cinco casas decimais.</span><span class="sxs-lookup"><span data-stu-id="59f84-142">Always display five decimal places.</span></span>

<span data-ttu-id="59f84-143">Observação: **decimalPlaces** e **displayAs** aplicam-se a como os números são processados, não armazenados.</span><span class="sxs-lookup"><span data-stu-id="59f84-143">Note: **decimalPlaces** and **displayAs** apply to how numbers are rendered, not stored.</span></span>
<span data-ttu-id="59f84-144">Essas propriedades podem ser atualizadas.</span><span class="sxs-lookup"><span data-stu-id="59f84-144">These properties may be updated.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/NumberColumn",
  "suppressions": []
}
-->
