---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: NumberColumn
ms.openlocfilehash: 8aa366e3c4f59fc5d22f945c863bab4f91373b67
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/28/2017
---
# <a name="numbercolumn-resource-type"></a><span data-ttu-id="3bed3-102">Tipo de recurso NumberColumn</span><span class="sxs-lookup"><span data-stu-id="3bed3-102">NumberColumn resource type</span></span>

<span data-ttu-id="3bed3-103">O recurso **numberColumn** em um recurso [columnDefinition](columnDefinition.md) indica que os valores da coluna são números.</span><span class="sxs-lookup"><span data-stu-id="3bed3-103">The **numberColumn** on a [columnDefinition](columnDefinition.md) resource indicates that the column's values are numbers.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3bed3-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3bed3-104">JSON representation</span></span>

<span data-ttu-id="3bed3-105">Aqui está uma representação JSON de um recurso **numberColumn**.</span><span class="sxs-lookup"><span data-stu-id="3bed3-105">Here is a JSON representation of a **driveItem** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.numberColumn" } -->

```json
{
  "decimalPlaces": "automatic | none | one | two | three | four | five",
  "displayAs": "number | percentage",
  "maximum": 10.551,
  "minimum": 99.993
}
```

## <a name="properties"></a><span data-ttu-id="3bed3-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3bed3-106">Properties</span></span>

| <span data-ttu-id="3bed3-107">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="3bed3-107">Property name</span></span>      | <span data-ttu-id="3bed3-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="3bed3-108">Type</span></span>   | <span data-ttu-id="3bed3-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="3bed3-109">Description</span></span>
|:-------------------|:-------|:-----------------------------------------------
| <span data-ttu-id="3bed3-110">**decimalPlaces**</span><span class="sxs-lookup"><span data-stu-id="3bed3-110">**decimalPlaces**</span></span>  | <span data-ttu-id="3bed3-111">string</span><span class="sxs-lookup"><span data-stu-id="3bed3-111">string</span></span> | <span data-ttu-id="3bed3-112">Quantas casas decimais exibir.</span><span class="sxs-lookup"><span data-stu-id="3bed3-112">How many decimal places to display.</span></span> <span data-ttu-id="3bed3-113">Consulte abaixo para saber mais sobre os valores possíveis.</span><span class="sxs-lookup"><span data-stu-id="3bed3-113">See below for information about the possible values.</span></span>
| <span data-ttu-id="3bed3-114">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="3bed3-114">**displayAs**</span></span>      | <span data-ttu-id="3bed3-115">string</span><span class="sxs-lookup"><span data-stu-id="3bed3-115">string</span></span> | <span data-ttu-id="3bed3-116">Como o valor deve ser apresentado na experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="3bed3-116">How the value should be presented in the UX.</span></span> <span data-ttu-id="3bed3-117">Deve ser `number` ou `percentage`.</span><span class="sxs-lookup"><span data-stu-id="3bed3-117">Must be one of `number` or `percentage`.</span></span> <span data-ttu-id="3bed3-118">Se não for especificado, é tratado como `number`.</span><span class="sxs-lookup"><span data-stu-id="3bed3-118">If unspecified, treated as `number`.</span></span>
| <span data-ttu-id="3bed3-119">**maximum**</span><span class="sxs-lookup"><span data-stu-id="3bed3-119">**maximum**</span></span>        | <span data-ttu-id="3bed3-120">double</span><span class="sxs-lookup"><span data-stu-id="3bed3-120">double</span></span> | <span data-ttu-id="3bed3-121">O valor máximo permitido.</span><span class="sxs-lookup"><span data-stu-id="3bed3-121">The maximum permitted value.</span></span>
| <span data-ttu-id="3bed3-122">**minimum**</span><span class="sxs-lookup"><span data-stu-id="3bed3-122">**minimum**</span></span>        | <span data-ttu-id="3bed3-123">double</span><span class="sxs-lookup"><span data-stu-id="3bed3-123">double</span></span> | <span data-ttu-id="3bed3-124">O valor mínimo permitido.</span><span class="sxs-lookup"><span data-stu-id="3bed3-124">The minimum permitted value.</span></span>

## <a name="decimalplaces-values"></a><span data-ttu-id="3bed3-125">Valores de DecimalPlaces</span><span class="sxs-lookup"><span data-stu-id="3bed3-125">DecimalPlaces values</span></span>

| <span data-ttu-id="3bed3-126">Valor</span><span class="sxs-lookup"><span data-stu-id="3bed3-126">Value</span></span>          | <span data-ttu-id="3bed3-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="3bed3-127">Description</span></span>
|:---------------|:--------------------------------------------------------------
| <span data-ttu-id="3bed3-128">**automatic**</span><span class="sxs-lookup"><span data-stu-id="3bed3-128">**Automatic**</span></span>  | <span data-ttu-id="3bed3-129">Padrão.</span><span class="sxs-lookup"><span data-stu-id="3bed3-129">Default.</span></span> <span data-ttu-id="3bed3-130">Exibir casas decimais automaticamente conforme necessário.</span><span class="sxs-lookup"><span data-stu-id="3bed3-130">Automatically display decimal places as needed.</span></span>
| <span data-ttu-id="3bed3-131">**none**</span><span class="sxs-lookup"><span data-stu-id="3bed3-131">**None**</span></span>       | <span data-ttu-id="3bed3-132">Não exibir casas decimais.</span><span class="sxs-lookup"><span data-stu-id="3bed3-132">Do not display any decimal places.</span></span>
| <span data-ttu-id="3bed3-133">**one**</span><span class="sxs-lookup"><span data-stu-id="3bed3-133">**One**</span></span>        | <span data-ttu-id="3bed3-134">Exibir sempre uma casa decimal.</span><span class="sxs-lookup"><span data-stu-id="3bed3-134">Always display one decimal place.</span></span>
| <span data-ttu-id="3bed3-135">**two**</span><span class="sxs-lookup"><span data-stu-id="3bed3-135">**Two**</span></span>        | <span data-ttu-id="3bed3-136">Exibir sempre duas casas decimais.</span><span class="sxs-lookup"><span data-stu-id="3bed3-136">Always display two decimal places.</span></span>
| <span data-ttu-id="3bed3-137">**three**</span><span class="sxs-lookup"><span data-stu-id="3bed3-137">**Three**</span></span>      | <span data-ttu-id="3bed3-138">Exibir sempre três casas decimais.</span><span class="sxs-lookup"><span data-stu-id="3bed3-138">Always display three decimal places.</span></span>
| <span data-ttu-id="3bed3-139">**four**</span><span class="sxs-lookup"><span data-stu-id="3bed3-139">**Four**</span></span>       | <span data-ttu-id="3bed3-140">Exibir sempre quatro casas decimais.</span><span class="sxs-lookup"><span data-stu-id="3bed3-140">Always display four decimal places.</span></span>
| <span data-ttu-id="3bed3-141">**five**</span><span class="sxs-lookup"><span data-stu-id="3bed3-141">**five**</span></span>       | <span data-ttu-id="3bed3-142">Exibir sempre cinco casas decimais.</span><span class="sxs-lookup"><span data-stu-id="3bed3-142">Always display five decimal places.</span></span>

<span data-ttu-id="3bed3-143">Observação: **decimalPlaces** e **displayAs** aplicam-se a como os números são processados, não armazenados.</span><span class="sxs-lookup"><span data-stu-id="3bed3-143">Note: **decimalPlaces** and **displayAs** apply to how numbers are rendered, not stored.</span></span>
<span data-ttu-id="3bed3-144">Essas propriedades podem ser atualizadas.</span><span class="sxs-lookup"><span data-stu-id="3bed3-144">These properties may be updated.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/NumberColumn"
} -->
