---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: FolderView
localization_priority: Normal
ms.openlocfilehash: f82242da39ebc13d769a0a3471b60dd4ac9df8dc
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2019
ms.locfileid: "30480919"
---
# <a name="folderview-resource-type"></a><span data-ttu-id="62fc4-102">Tipo de recurso FolderView</span><span class="sxs-lookup"><span data-stu-id="62fc4-102">FolderView resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="62fc4-103">O recurso **FolderView** fornece ou define recomendações sobre a experiência do usuário de uma pasta.</span><span class="sxs-lookup"><span data-stu-id="62fc4-103">The **FolderView** resource provides or sets recommendations on the user-experience of a folder.</span></span>

<span data-ttu-id="62fc4-104">Está disponível a partir da propriedade [folder][folder-facet] dos recursos [driveItem][item-resource].</span><span class="sxs-lookup"><span data-stu-id="62fc4-104">It is available from the [folder][folder-facet] property of [driveItem][item-resource] resources.</span></span>

## <a name="json-representation"></a><span data-ttu-id="62fc4-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="62fc4-105">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.folderView" } -->

```json
{
  "sortBy": "default | name | type | size | takenOrCreatedDateTime | lastModifiedDateTime | sequence",
  "sortDescending": "ascending | descending",
  "viewType": "default | icons | details | thumbnails"
}
```

## <a name="properties"></a><span data-ttu-id="62fc4-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="62fc4-106">Properties</span></span>

| <span data-ttu-id="62fc4-107">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="62fc4-107">Property name</span></span>         | <span data-ttu-id="62fc4-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="62fc4-108">Type</span></span>   | <span data-ttu-id="62fc4-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="62fc4-109">Description</span></span>
|:----------------------|:-------|:--------------------------------------------
| <span data-ttu-id="62fc4-110">**sortBy**</span><span class="sxs-lookup"><span data-stu-id="62fc4-110">**sortBy**</span></span>            | <span data-ttu-id="62fc4-111">string</span><span class="sxs-lookup"><span data-stu-id="62fc4-111">string</span></span> | <span data-ttu-id="62fc4-112">O método pelo qual a pasta deve ser classificada.</span><span class="sxs-lookup"><span data-stu-id="62fc4-112">The method by which the folder should be sorted.</span></span>
| <span data-ttu-id="62fc4-113">**sortOrder**</span><span class="sxs-lookup"><span data-stu-id="62fc4-113">**sortOrder**</span></span>         | <span data-ttu-id="62fc4-114">string</span><span class="sxs-lookup"><span data-stu-id="62fc4-114">string</span></span> | <span data-ttu-id="62fc4-p101">Se for verdadeiro, indica que os itens devem ser classificados em ordem decrescente. Caso contrário, os itens devem ser classificados em ordem crescente.</span><span class="sxs-lookup"><span data-stu-id="62fc4-p101">If true, indicates that items should be sorted in descending order. Otherwise, items should be sorted ascending.</span></span>
| <span data-ttu-id="62fc4-117">**viewType**</span><span class="sxs-lookup"><span data-stu-id="62fc4-117">**viewType**</span></span>          | <span data-ttu-id="62fc4-118">string</span><span class="sxs-lookup"><span data-stu-id="62fc4-118">string</span></span> | <span data-ttu-id="62fc4-119">O tipo de modo de exibição que deve ser usado para representar a pasta.</span><span class="sxs-lookup"><span data-stu-id="62fc4-119">The type of view that should be used to represent the folder.</span></span>

<span data-ttu-id="62fc4-120">Você pode usar a propriedade _sortBy_ para controlar a ordem de classificação dos itens em aplicativos que respeitam a faceta **viewType**.</span><span class="sxs-lookup"><span data-stu-id="62fc4-120">You can use the _sortBy_ property to control the sort order of the items in applications that respect the **viewType** facet.</span></span>

### <a name="sortby-values"></a><span data-ttu-id="62fc4-121">Valores sortBy</span><span class="sxs-lookup"><span data-stu-id="62fc4-121">sortBy values</span></span>

<span data-ttu-id="62fc4-122">Os seguintes valores são definidos para a propriedade **sortBy**.</span><span class="sxs-lookup"><span data-stu-id="62fc4-122">The following values are defined for the **sortBy** property.</span></span>

| <span data-ttu-id="62fc4-123">Valor</span><span class="sxs-lookup"><span data-stu-id="62fc4-123">Value</span></span>                    | <span data-ttu-id="62fc4-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="62fc4-124">Description</span></span>
| ------------------------ | --------------------------------------------------
| `default`                | <span data-ttu-id="62fc4-125">A ordem de classificação padrão do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="62fc4-125">The default sort order of the application.</span></span>
| `name`                   | <span data-ttu-id="62fc4-126">Os itens devem ser organizados pela propriedade **name** dos itens.</span><span class="sxs-lookup"><span data-stu-id="62fc4-126">Items should be arranged by the **name** property of the items.</span></span>
| `type`                   | <span data-ttu-id="62fc4-127">Os itens devem ser organizados pelo tipo de item.</span><span class="sxs-lookup"><span data-stu-id="62fc4-127">Items should be arranged by the type of item.</span></span>
| `size`                   | <span data-ttu-id="62fc4-128">Os itens devem ser organizados pela propriedade **size** dos itens.</span><span class="sxs-lookup"><span data-stu-id="62fc4-128">Items should be arranged by the **size** property of the items.</span></span>
| `takenOrCreatedDateTime` | <span data-ttu-id="62fc4-p102">Os itens devem ser organizados pela propriedade **takenDateTime** da faceta **photo**. Se não estiver disponível, a propriedade **createdDateTime** deverá ser usada.</span><span class="sxs-lookup"><span data-stu-id="62fc4-p102">Items should be arranged by the **takenDateTime** property of the **photo** facet. If not available, the **createdDateTime** property should be used.</span></span>
| `lastModifiedDateTime`   | <span data-ttu-id="62fc4-131">Os itens devem ser organizados pela propriedade **lastModifiedDateTime** dos itens.</span><span class="sxs-lookup"><span data-stu-id="62fc4-131">Items should be arranged by the **lastModifiedDateTime** property of the items.</span></span>
| `sequence`               | <span data-ttu-id="62fc4-132">Os itens seguem uma sequência personalizada especificada pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="62fc4-132">Items follow a custom sequence specified by the user.</span></span>


### <a name="sortorder-values"></a><span data-ttu-id="62fc4-133">Valores sortOrder</span><span class="sxs-lookup"><span data-stu-id="62fc4-133">sortOrder values</span></span>

<span data-ttu-id="62fc4-134">Os seguintes valores são definidos para a propriedade **sortOrder**.</span><span class="sxs-lookup"><span data-stu-id="62fc4-134">The following values are defined for the **sortOrder** property.</span></span>

| <span data-ttu-id="62fc4-135">Valor</span><span class="sxs-lookup"><span data-stu-id="62fc4-135">Value</span></span>        | <span data-ttu-id="62fc4-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="62fc4-136">Description</span></span>
| ------------ | --------------------------------------------------------------
| `ascending`  | <span data-ttu-id="62fc4-137">Os itens devem ser organizados em ordem crescente.</span><span class="sxs-lookup"><span data-stu-id="62fc4-137">Items should be arranged in ascending order.</span></span>
| `descending` | <span data-ttu-id="62fc4-138">Os itens devem ser organizados em ordem decrescente.</span><span class="sxs-lookup"><span data-stu-id="62fc4-138">Items should be arranged in descending order.</span></span>


### <a name="viewtype-values"></a><span data-ttu-id="62fc4-139">Valores viewType</span><span class="sxs-lookup"><span data-stu-id="62fc4-139">viewType values</span></span>

<span data-ttu-id="62fc4-140">Os seguintes valores são definidos para a propriedade **viewType**.</span><span class="sxs-lookup"><span data-stu-id="62fc4-140">The following values are defined for the **viewType** property.</span></span>

| <span data-ttu-id="62fc4-141">Valor</span><span class="sxs-lookup"><span data-stu-id="62fc4-141">Value</span></span>        | <span data-ttu-id="62fc4-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="62fc4-142">Description</span></span>
| ------------ | --------------------------------------------------------------
| `default`    | <span data-ttu-id="62fc4-143">O tipo de exibição padrão para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="62fc4-143">The default view type for the application.</span></span>
| `icons`      | <span data-ttu-id="62fc4-144">Um modo de exibição que usa ícones para representar driveItems.</span><span class="sxs-lookup"><span data-stu-id="62fc4-144">A view that uses icons to represent driveItems.</span></span>
| `details`    | <span data-ttu-id="62fc4-145">Um modo de exibição com várias colunas que fornecem detalhes adicionais sobre cada item.</span><span class="sxs-lookup"><span data-stu-id="62fc4-145">A view with multiple columns that provide additional details about each item.</span></span>
| `thumbnails` | <span data-ttu-id="62fc4-146">Um modo de exibição que usa miniaturas maiores de driveItems para representar os itens.</span><span class="sxs-lookup"><span data-stu-id="62fc4-146">A view that uses larger thumbnails of driveItems to represent the items.</span></span>


[item-resource]: driveitem.md
[folder-facet]: folder.md

<!-- uuid: f9e446fd-190b-4692-a605-bb60e78f1f19
2017-05-03 02:34:40 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "folderView resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/folderview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
