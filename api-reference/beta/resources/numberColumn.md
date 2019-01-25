---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: NumberColumn
localization_priority: Normal
ms.openlocfilehash: cf1f6c6cafd23a5503d645d13e597a8941019fee
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512875"
---
# <a name="numbercolumn-resource-type"></a><span data-ttu-id="3b58d-102">Tipo de recurso NumberColumn</span><span class="sxs-lookup"><span data-stu-id="3b58d-102">NumberColumn resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3b58d-103">O recurso **numberColumn** em um recurso [columnDefinition](columndefinition.md) indica que os valores da coluna são números.</span><span class="sxs-lookup"><span data-stu-id="3b58d-103">The **numberColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are numbers.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3b58d-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3b58d-104">JSON representation</span></span>

<span data-ttu-id="3b58d-105">Aqui está uma representação JSON de um recurso **numberColumn**.</span><span class="sxs-lookup"><span data-stu-id="3b58d-105">Here is a JSON representation of a **numberColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.numberColumn" } -->

```json
{
  "decimalPlaces": "automatic | none | one | two | three | four | five",
  "displayAs": "number | percentage",
  "maximum": 10.551,
  "minimum": 99.993
}
```

## <a name="properties"></a><span data-ttu-id="3b58d-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3b58d-106">Properties</span></span>

| <span data-ttu-id="3b58d-107">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="3b58d-107">Property name</span></span>      | <span data-ttu-id="3b58d-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="3b58d-108">Type</span></span>   | <span data-ttu-id="3b58d-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="3b58d-109">Description</span></span>
|:-------------------|:-------|:-----------------------------------------------
| <span data-ttu-id="3b58d-110">**decimalPlaces**</span><span class="sxs-lookup"><span data-stu-id="3b58d-110">**decimalPlaces**</span></span>  | <span data-ttu-id="3b58d-111">string</span><span class="sxs-lookup"><span data-stu-id="3b58d-111">string</span></span> | <span data-ttu-id="3b58d-112">Quantas casas decimais exibir.</span><span class="sxs-lookup"><span data-stu-id="3b58d-112">How many decimal places to display.</span></span> <span data-ttu-id="3b58d-113">Consulte abaixo para saber mais sobre os valores possíveis.</span><span class="sxs-lookup"><span data-stu-id="3b58d-113">See below for information about the possible values.</span></span>
| <span data-ttu-id="3b58d-114">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="3b58d-114">**displayAs**</span></span>      | <span data-ttu-id="3b58d-115">string</span><span class="sxs-lookup"><span data-stu-id="3b58d-115">string</span></span> | <span data-ttu-id="3b58d-116">Como o valor deve ser apresentado na experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="3b58d-116">How the value should be presented in the UX.</span></span> <span data-ttu-id="3b58d-117">Deve ser `number` ou `percentage`.</span><span class="sxs-lookup"><span data-stu-id="3b58d-117">Must be one of `number` or `percentage`.</span></span> <span data-ttu-id="3b58d-118">Se não for especificado, é tratado como `number`.</span><span class="sxs-lookup"><span data-stu-id="3b58d-118">If unspecified, treated as `number`.</span></span>
| <span data-ttu-id="3b58d-119">**maximum**</span><span class="sxs-lookup"><span data-stu-id="3b58d-119">**maximum**</span></span>        | <span data-ttu-id="3b58d-120">double</span><span class="sxs-lookup"><span data-stu-id="3b58d-120">double</span></span> | <span data-ttu-id="3b58d-121">O valor máximo permitido.</span><span class="sxs-lookup"><span data-stu-id="3b58d-121">The maximum permitted value.</span></span>
| <span data-ttu-id="3b58d-122">**minimum**</span><span class="sxs-lookup"><span data-stu-id="3b58d-122">**minimum**</span></span>        | <span data-ttu-id="3b58d-123">double</span><span class="sxs-lookup"><span data-stu-id="3b58d-123">double</span></span> | <span data-ttu-id="3b58d-124">O valor mínimo permitido.</span><span class="sxs-lookup"><span data-stu-id="3b58d-124">The minimum permitted value.</span></span>

## <a name="decimalplaces-values"></a><span data-ttu-id="3b58d-125">Valores de DecimalPlaces</span><span class="sxs-lookup"><span data-stu-id="3b58d-125">DecimalPlaces values</span></span>

| <span data-ttu-id="3b58d-126">Valor</span><span class="sxs-lookup"><span data-stu-id="3b58d-126">Value</span></span>          | <span data-ttu-id="3b58d-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="3b58d-127">Description</span></span>
|:---------------|:--------------------------------------------------------------
| <span data-ttu-id="3b58d-128">**automatic**</span><span class="sxs-lookup"><span data-stu-id="3b58d-128">**automatic**</span></span>  | <span data-ttu-id="3b58d-129">Padrão.</span><span class="sxs-lookup"><span data-stu-id="3b58d-129">Default.</span></span> <span data-ttu-id="3b58d-130">Exibir casas decimais automaticamente conforme necessário.</span><span class="sxs-lookup"><span data-stu-id="3b58d-130">Automatically display decimal places as needed.</span></span>
| <span data-ttu-id="3b58d-131">**none**</span><span class="sxs-lookup"><span data-stu-id="3b58d-131">**none**</span></span>       | <span data-ttu-id="3b58d-132">Não exibir casas decimais.</span><span class="sxs-lookup"><span data-stu-id="3b58d-132">Do not display any decimal places.</span></span>
| <span data-ttu-id="3b58d-133">**one**</span><span class="sxs-lookup"><span data-stu-id="3b58d-133">**one**</span></span>        | <span data-ttu-id="3b58d-134">Exibir sempre uma casa decimal.</span><span class="sxs-lookup"><span data-stu-id="3b58d-134">Always display one decimal place.</span></span>
| <span data-ttu-id="3b58d-135">**two**</span><span class="sxs-lookup"><span data-stu-id="3b58d-135">**two**</span></span>        | <span data-ttu-id="3b58d-136">Exibir sempre duas casas decimais.</span><span class="sxs-lookup"><span data-stu-id="3b58d-136">Always display two decimal places.</span></span>
| <span data-ttu-id="3b58d-137">**three**</span><span class="sxs-lookup"><span data-stu-id="3b58d-137">**three**</span></span>      | <span data-ttu-id="3b58d-138">Exibir sempre três casas decimais.</span><span class="sxs-lookup"><span data-stu-id="3b58d-138">Always display three decimal places.</span></span>
| <span data-ttu-id="3b58d-139">**four**</span><span class="sxs-lookup"><span data-stu-id="3b58d-139">**four**</span></span>       | <span data-ttu-id="3b58d-140">Exibir sempre quatro casas decimais.</span><span class="sxs-lookup"><span data-stu-id="3b58d-140">Always display four decimal places.</span></span>
| <span data-ttu-id="3b58d-141">**five**</span><span class="sxs-lookup"><span data-stu-id="3b58d-141">**five**</span></span>       | <span data-ttu-id="3b58d-142">Exibir sempre cinco casas decimais.</span><span class="sxs-lookup"><span data-stu-id="3b58d-142">Always display five decimal places.</span></span>

<span data-ttu-id="3b58d-143">Observação: **decimalPlaces** e **displayAs** aplicam-se a como os números são processados, não armazenados.</span><span class="sxs-lookup"><span data-stu-id="3b58d-143">Note: **decimalPlaces** and **displayAs** apply to how numbers are rendered, not stored.</span></span>
<span data-ttu-id="3b58d-144">Essas propriedades podem ser atualizadas.</span><span class="sxs-lookup"><span data-stu-id="3b58d-144">These properties may be updated.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/NumberColumn",
  "suppressions": [
    "Error: /api-reference/beta/resources/numberColumn.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
