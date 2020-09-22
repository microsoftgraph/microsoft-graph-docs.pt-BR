---
author: JeremyKelley
description: O recurso numberColumn em um recurso columnDefinition indica que os valores da coluna são números.
ms.date: 09/11/2017
title: NumberColumn
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 49c3dce15297187bcda20e20ae339dba86d154db
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47988950"
---
# <a name="numbercolumn-resource-type"></a><span data-ttu-id="63a1d-103">Tipo de recurso NumberColumn</span><span class="sxs-lookup"><span data-stu-id="63a1d-103">NumberColumn resource type</span></span>

<span data-ttu-id="63a1d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="63a1d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="63a1d-105">O recurso **numberColumn** em um recurso [columnDefinition](columndefinition.md) indica que os valores da coluna são números.</span><span class="sxs-lookup"><span data-stu-id="63a1d-105">The **numberColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are numbers.</span></span>

## <a name="json-representation"></a><span data-ttu-id="63a1d-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="63a1d-106">JSON representation</span></span>

<span data-ttu-id="63a1d-107">Aqui está uma representação JSON de um recurso **numberColumn**.</span><span class="sxs-lookup"><span data-stu-id="63a1d-107">Here is a JSON representation of a **numberColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.numberColumn" } -->

```json
{
  "decimalPlaces": "automatic | none | one | two | three | four | five",
  "displayAs": "number | percentage",
  "maximum": 10.551,
  "minimum": 99.993
}
```

## <a name="properties"></a><span data-ttu-id="63a1d-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="63a1d-108">Properties</span></span>

| <span data-ttu-id="63a1d-109">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="63a1d-109">Property name</span></span>      | <span data-ttu-id="63a1d-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="63a1d-110">Type</span></span>   | <span data-ttu-id="63a1d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="63a1d-111">Description</span></span>
|:-------------------|:-------|:-----------------------------------------------
| <span data-ttu-id="63a1d-112">**decimalPlaces**</span><span class="sxs-lookup"><span data-stu-id="63a1d-112">**decimalPlaces**</span></span>  | <span data-ttu-id="63a1d-113">string</span><span class="sxs-lookup"><span data-stu-id="63a1d-113">string</span></span> | <span data-ttu-id="63a1d-114">Quantas casas decimais exibir.</span><span class="sxs-lookup"><span data-stu-id="63a1d-114">How many decimal places to display.</span></span> <span data-ttu-id="63a1d-115">Consulte abaixo para saber mais sobre os valores possíveis.</span><span class="sxs-lookup"><span data-stu-id="63a1d-115">See below for information about the possible values.</span></span>
| <span data-ttu-id="63a1d-116">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="63a1d-116">**displayAs**</span></span>      | <span data-ttu-id="63a1d-117">string</span><span class="sxs-lookup"><span data-stu-id="63a1d-117">string</span></span> | <span data-ttu-id="63a1d-118">Como o valor deve ser apresentado na experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="63a1d-118">How the value should be presented in the UX.</span></span> <span data-ttu-id="63a1d-119">Deve ser `number` ou `percentage`.</span><span class="sxs-lookup"><span data-stu-id="63a1d-119">Must be one of `number` or `percentage`.</span></span> <span data-ttu-id="63a1d-120">Se não for especificado, é tratado como `number`.</span><span class="sxs-lookup"><span data-stu-id="63a1d-120">If unspecified, treated as `number`.</span></span>
| <span data-ttu-id="63a1d-121">**maximum**</span><span class="sxs-lookup"><span data-stu-id="63a1d-121">**maximum**</span></span>        | <span data-ttu-id="63a1d-122">double</span><span class="sxs-lookup"><span data-stu-id="63a1d-122">double</span></span> | <span data-ttu-id="63a1d-123">O valor máximo permitido.</span><span class="sxs-lookup"><span data-stu-id="63a1d-123">The maximum permitted value.</span></span>
| <span data-ttu-id="63a1d-124">**minimum**</span><span class="sxs-lookup"><span data-stu-id="63a1d-124">**minimum**</span></span>        | <span data-ttu-id="63a1d-125">double</span><span class="sxs-lookup"><span data-stu-id="63a1d-125">double</span></span> | <span data-ttu-id="63a1d-126">O valor mínimo permitido.</span><span class="sxs-lookup"><span data-stu-id="63a1d-126">The minimum permitted value.</span></span>

## <a name="decimalplaces-values"></a><span data-ttu-id="63a1d-127">Valores de DecimalPlaces</span><span class="sxs-lookup"><span data-stu-id="63a1d-127">DecimalPlaces values</span></span>

| <span data-ttu-id="63a1d-128">Valor</span><span class="sxs-lookup"><span data-stu-id="63a1d-128">Value</span></span>          | <span data-ttu-id="63a1d-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="63a1d-129">Description</span></span>
|:---------------|:--------------------------------------------------------------
| <span data-ttu-id="63a1d-130">**automatic**</span><span class="sxs-lookup"><span data-stu-id="63a1d-130">**automatic**</span></span>  | <span data-ttu-id="63a1d-131">Padrão.</span><span class="sxs-lookup"><span data-stu-id="63a1d-131">Default.</span></span> <span data-ttu-id="63a1d-132">Exibir casas decimais automaticamente conforme necessário.</span><span class="sxs-lookup"><span data-stu-id="63a1d-132">Automatically display decimal places as needed.</span></span>
| <span data-ttu-id="63a1d-133">**none**</span><span class="sxs-lookup"><span data-stu-id="63a1d-133">**none**</span></span>       | <span data-ttu-id="63a1d-134">Não exibir casas decimais.</span><span class="sxs-lookup"><span data-stu-id="63a1d-134">Do not display any decimal places.</span></span>
| <span data-ttu-id="63a1d-135">**one**</span><span class="sxs-lookup"><span data-stu-id="63a1d-135">**one**</span></span>        | <span data-ttu-id="63a1d-136">Exibir sempre uma casa decimal.</span><span class="sxs-lookup"><span data-stu-id="63a1d-136">Always display one decimal place.</span></span>
| <span data-ttu-id="63a1d-137">**two**</span><span class="sxs-lookup"><span data-stu-id="63a1d-137">**two**</span></span>        | <span data-ttu-id="63a1d-138">Exibir sempre duas casas decimais.</span><span class="sxs-lookup"><span data-stu-id="63a1d-138">Always display two decimal places.</span></span>
| <span data-ttu-id="63a1d-139">**three**</span><span class="sxs-lookup"><span data-stu-id="63a1d-139">**three**</span></span>      | <span data-ttu-id="63a1d-140">Exibir sempre três casas decimais.</span><span class="sxs-lookup"><span data-stu-id="63a1d-140">Always display three decimal places.</span></span>
| <span data-ttu-id="63a1d-141">**four**</span><span class="sxs-lookup"><span data-stu-id="63a1d-141">**four**</span></span>       | <span data-ttu-id="63a1d-142">Exibir sempre quatro casas decimais.</span><span class="sxs-lookup"><span data-stu-id="63a1d-142">Always display four decimal places.</span></span>
| <span data-ttu-id="63a1d-143">**five**</span><span class="sxs-lookup"><span data-stu-id="63a1d-143">**five**</span></span>       | <span data-ttu-id="63a1d-144">Exibir sempre cinco casas decimais.</span><span class="sxs-lookup"><span data-stu-id="63a1d-144">Always display five decimal places.</span></span>

<span data-ttu-id="63a1d-145">Observação: **decimalPlaces** e **displayAs** aplicam-se a como os números são processados, não armazenados.</span><span class="sxs-lookup"><span data-stu-id="63a1d-145">Note: **decimalPlaces** and **displayAs** apply to how numbers are rendered, not stored.</span></span>
<span data-ttu-id="63a1d-146">Essas propriedades podem ser atualizadas.</span><span class="sxs-lookup"><span data-stu-id="63a1d-146">These properties may be updated.</span></span>

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


