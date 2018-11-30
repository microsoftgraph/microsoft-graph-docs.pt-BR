---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: NumberColumn
ms.openlocfilehash: 27d17d3e9b9d3d1debcd20f2beb916222801ebe9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27040763"
---
# <a name="numbercolumn-resource-type"></a><span data-ttu-id="38e4b-102">Tipo de recurso NumberColumn</span><span class="sxs-lookup"><span data-stu-id="38e4b-102">NumberColumn resource type</span></span>

> <span data-ttu-id="38e4b-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="38e4b-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="38e4b-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="38e4b-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="38e4b-105">O recurso **numberColumn** em um recurso [columnDefinition](columndefinition.md) indica que os valores da coluna são números.</span><span class="sxs-lookup"><span data-stu-id="38e4b-105">The **numberColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are numbers.</span></span>

## <a name="json-representation"></a><span data-ttu-id="38e4b-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="38e4b-106">JSON representation</span></span>

<span data-ttu-id="38e4b-107">Aqui está uma representação JSON de um recurso **numberColumn**.</span><span class="sxs-lookup"><span data-stu-id="38e4b-107">Here is a JSON representation of a **numberColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.numberColumn" } -->

```json
{
  "decimalPlaces": "automatic | none | one | two | three | four | five",
  "displayAs": "number | percentage",
  "maximum": 10.551,
  "minimum": 99.993
}
```

## <a name="properties"></a><span data-ttu-id="38e4b-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="38e4b-108">Properties</span></span>

| <span data-ttu-id="38e4b-109">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="38e4b-109">Property name</span></span>      | <span data-ttu-id="38e4b-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="38e4b-110">Type</span></span>   | <span data-ttu-id="38e4b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="38e4b-111">Description</span></span>
|:-------------------|:-------|:-----------------------------------------------
| <span data-ttu-id="38e4b-112">**decimalPlaces**</span><span class="sxs-lookup"><span data-stu-id="38e4b-112">**decimalPlaces**</span></span>  | <span data-ttu-id="38e4b-113">string</span><span class="sxs-lookup"><span data-stu-id="38e4b-113">string</span></span> | <span data-ttu-id="38e4b-114">Quantas casas decimais exibir.</span><span class="sxs-lookup"><span data-stu-id="38e4b-114">How many decimal places to display.</span></span> <span data-ttu-id="38e4b-115">Consulte abaixo para saber mais sobre os valores possíveis.</span><span class="sxs-lookup"><span data-stu-id="38e4b-115">See below for information about the possible values.</span></span>
| <span data-ttu-id="38e4b-116">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="38e4b-116">**displayAs**</span></span>      | <span data-ttu-id="38e4b-117">string</span><span class="sxs-lookup"><span data-stu-id="38e4b-117">string</span></span> | <span data-ttu-id="38e4b-118">Como o valor deve ser apresentado na experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="38e4b-118">How the value should be presented in the UX.</span></span> <span data-ttu-id="38e4b-119">Deve ser `number` ou `percentage`.</span><span class="sxs-lookup"><span data-stu-id="38e4b-119">Must be one of `number` or `percentage`.</span></span> <span data-ttu-id="38e4b-120">Se não for especificado, é tratado como `number`.</span><span class="sxs-lookup"><span data-stu-id="38e4b-120">If unspecified, treated as `number`.</span></span>
| <span data-ttu-id="38e4b-121">**maximum**</span><span class="sxs-lookup"><span data-stu-id="38e4b-121">**maximum**</span></span>        | <span data-ttu-id="38e4b-122">double</span><span class="sxs-lookup"><span data-stu-id="38e4b-122">double</span></span> | <span data-ttu-id="38e4b-123">O valor máximo permitido.</span><span class="sxs-lookup"><span data-stu-id="38e4b-123">The maximum permitted value.</span></span>
| <span data-ttu-id="38e4b-124">**minimum**</span><span class="sxs-lookup"><span data-stu-id="38e4b-124">**minimum**</span></span>        | <span data-ttu-id="38e4b-125">double</span><span class="sxs-lookup"><span data-stu-id="38e4b-125">double</span></span> | <span data-ttu-id="38e4b-126">O valor mínimo permitido.</span><span class="sxs-lookup"><span data-stu-id="38e4b-126">The minimum permitted value.</span></span>

## <a name="decimalplaces-values"></a><span data-ttu-id="38e4b-127">Valores de DecimalPlaces</span><span class="sxs-lookup"><span data-stu-id="38e4b-127">DecimalPlaces values</span></span>

| <span data-ttu-id="38e4b-128">Valor</span><span class="sxs-lookup"><span data-stu-id="38e4b-128">Value</span></span>          | <span data-ttu-id="38e4b-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="38e4b-129">Description</span></span>
|:---------------|:--------------------------------------------------------------
| <span data-ttu-id="38e4b-130">**automatic**</span><span class="sxs-lookup"><span data-stu-id="38e4b-130">**automatic**</span></span>  | <span data-ttu-id="38e4b-131">Padrão.</span><span class="sxs-lookup"><span data-stu-id="38e4b-131">Default.</span></span> <span data-ttu-id="38e4b-132">Exibir casas decimais automaticamente conforme necessário.</span><span class="sxs-lookup"><span data-stu-id="38e4b-132">Automatically display decimal places as needed.</span></span>
| <span data-ttu-id="38e4b-133">**none**</span><span class="sxs-lookup"><span data-stu-id="38e4b-133">**none**</span></span>       | <span data-ttu-id="38e4b-134">Não exibir casas decimais.</span><span class="sxs-lookup"><span data-stu-id="38e4b-134">Do not display any decimal places.</span></span>
| <span data-ttu-id="38e4b-135">**one**</span><span class="sxs-lookup"><span data-stu-id="38e4b-135">**one**</span></span>        | <span data-ttu-id="38e4b-136">Exibir sempre uma casa decimal.</span><span class="sxs-lookup"><span data-stu-id="38e4b-136">Always display one decimal place.</span></span>
| <span data-ttu-id="38e4b-137">**two**</span><span class="sxs-lookup"><span data-stu-id="38e4b-137">**two**</span></span>        | <span data-ttu-id="38e4b-138">Exibir sempre duas casas decimais.</span><span class="sxs-lookup"><span data-stu-id="38e4b-138">Always display two decimal places.</span></span>
| <span data-ttu-id="38e4b-139">**three**</span><span class="sxs-lookup"><span data-stu-id="38e4b-139">**three**</span></span>      | <span data-ttu-id="38e4b-140">Exibir sempre três casas decimais.</span><span class="sxs-lookup"><span data-stu-id="38e4b-140">Always display three decimal places.</span></span>
| <span data-ttu-id="38e4b-141">**four**</span><span class="sxs-lookup"><span data-stu-id="38e4b-141">**four**</span></span>       | <span data-ttu-id="38e4b-142">Exibir sempre quatro casas decimais.</span><span class="sxs-lookup"><span data-stu-id="38e4b-142">Always display four decimal places.</span></span>
| <span data-ttu-id="38e4b-143">**five**</span><span class="sxs-lookup"><span data-stu-id="38e4b-143">**five**</span></span>       | <span data-ttu-id="38e4b-144">Exibir sempre cinco casas decimais.</span><span class="sxs-lookup"><span data-stu-id="38e4b-144">Always display five decimal places.</span></span>

<span data-ttu-id="38e4b-145">Observação: **decimalPlaces** e **displayAs** aplicam-se a como os números são processados, não armazenados.</span><span class="sxs-lookup"><span data-stu-id="38e4b-145">Note: **decimalPlaces** and **displayAs** apply to how numbers are rendered, not stored.</span></span>
<span data-ttu-id="38e4b-146">Essas propriedades podem ser atualizadas.</span><span class="sxs-lookup"><span data-stu-id="38e4b-146">These properties may be updated.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/NumberColumn"
} -->
