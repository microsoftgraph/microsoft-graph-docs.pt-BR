---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: FolderView
localization_priority: Normal
ms.openlocfilehash: 01b9860284f87ea31a969055fe2bfc7da624d3b6
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2019
ms.locfileid: "30482004"
---
# <a name="folderview-resource-type"></a><span data-ttu-id="af6ef-102">Tipo de recurso FolderView</span><span class="sxs-lookup"><span data-stu-id="af6ef-102">FolderView resource type</span></span>

<span data-ttu-id="af6ef-103">O recurso **FolderView** fornece ou define recomendações sobre a experiência do usuário de uma pasta.</span><span class="sxs-lookup"><span data-stu-id="af6ef-103">The **FolderView** resource provides or sets recommendations on the user-experience of a folder.</span></span>

<span data-ttu-id="af6ef-104">Está disponível a partir da propriedade [folder][folder-facet] dos recursos [driveItem][item-resource].</span><span class="sxs-lookup"><span data-stu-id="af6ef-104">It is available from the [folder][folder-facet] property of [driveItem][item-resource] resources.</span></span>

## <a name="json-representation"></a><span data-ttu-id="af6ef-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="af6ef-105">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.folderView" } -->

```json
{
  "sortBy": "default | name | type | size | takenOrCreatedDateTime | lastModifiedDateTime | sequence",
  "sortOrder": "ascending | descending",
  "viewType": "default | icons | details | thumbnails"
}
```

## <a name="properties"></a><span data-ttu-id="af6ef-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="af6ef-106">Properties</span></span>

| <span data-ttu-id="af6ef-107">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="af6ef-107">Property name</span></span>         | <span data-ttu-id="af6ef-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="af6ef-108">Type</span></span>   | <span data-ttu-id="af6ef-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="af6ef-109">Description</span></span>
|:----------------------|:-------|:--------------------------------------------
| <span data-ttu-id="af6ef-110">**sortBy**</span><span class="sxs-lookup"><span data-stu-id="af6ef-110">**sortBy**</span></span>            | <span data-ttu-id="af6ef-111">string</span><span class="sxs-lookup"><span data-stu-id="af6ef-111">string</span></span> | <span data-ttu-id="af6ef-112">O método pelo qual a pasta deve ser classificada.</span><span class="sxs-lookup"><span data-stu-id="af6ef-112">The method by which the folder should be sorted.</span></span>
| <span data-ttu-id="af6ef-113">**sortOrder**</span><span class="sxs-lookup"><span data-stu-id="af6ef-113">**sortOrder**</span></span>         | <span data-ttu-id="af6ef-114">string</span><span class="sxs-lookup"><span data-stu-id="af6ef-114">string</span></span> | <span data-ttu-id="af6ef-p101">Se for verdadeiro, indica que os itens devem ser classificados em ordem decrescente. Caso contrário, os itens devem ser classificados em ordem crescente.</span><span class="sxs-lookup"><span data-stu-id="af6ef-p101">If true, indicates that items should be sorted in descending order. Otherwise, items should be sorted ascending.</span></span>
| <span data-ttu-id="af6ef-117">**viewType**</span><span class="sxs-lookup"><span data-stu-id="af6ef-117">**viewType**</span></span>          | <span data-ttu-id="af6ef-118">string</span><span class="sxs-lookup"><span data-stu-id="af6ef-118">string</span></span> | <span data-ttu-id="af6ef-119">O tipo de modo de exibição que deve ser usado para representar a pasta.</span><span class="sxs-lookup"><span data-stu-id="af6ef-119">The type of view that should be used to represent the folder.</span></span>

<span data-ttu-id="af6ef-120">Você pode usar a propriedade _sortBy_ para controlar a ordem de classificação dos itens em aplicativos que respeitam a faceta **viewType**.</span><span class="sxs-lookup"><span data-stu-id="af6ef-120">You can use the _sortBy_ property to control the sort order of the items in applications that respect the **viewType** facet.</span></span>

### <a name="sortby-options"></a><span data-ttu-id="af6ef-121">opções de sortBy</span><span class="sxs-lookup"><span data-stu-id="af6ef-121">sortBy options</span></span>

<span data-ttu-id="af6ef-122">Os seguintes valores são definidos para a propriedade **sortBy**.</span><span class="sxs-lookup"><span data-stu-id="af6ef-122">The following values are defined for the **sortBy** property.</span></span>

| <span data-ttu-id="af6ef-123">Valor</span><span class="sxs-lookup"><span data-stu-id="af6ef-123">Value</span></span>                    | <span data-ttu-id="af6ef-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="af6ef-124">Description</span></span>
| ------------------------ | --------------------------------------------------
| `default`                | <span data-ttu-id="af6ef-125">A ordem de classificação padrão do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="af6ef-125">The default sort order of the application.</span></span>
| `name`                   | <span data-ttu-id="af6ef-126">Os itens devem ser organizados pela propriedade **name** dos itens.</span><span class="sxs-lookup"><span data-stu-id="af6ef-126">Items should be arranged by the **name** property of the items.</span></span>
| `type`                   | <span data-ttu-id="af6ef-127">Os itens devem ser organizados pelo tipo de item.</span><span class="sxs-lookup"><span data-stu-id="af6ef-127">Items should be arranged by the type of item.</span></span>
| `size`                   | <span data-ttu-id="af6ef-128">Os itens devem ser organizados pela propriedade **size** dos itens.</span><span class="sxs-lookup"><span data-stu-id="af6ef-128">Items should be arranged by the **size** property of the items.</span></span>
| `takenOrCreatedDateTime` | <span data-ttu-id="af6ef-p102">Os itens devem ser organizados pela propriedade **takenDateTime** da faceta **photo**. Se não estiver disponível, a propriedade **createdDateTime** deverá ser usada.</span><span class="sxs-lookup"><span data-stu-id="af6ef-p102">Items should be arranged by the **takenDateTime** property of the **photo** facet. If not available, the **createdDateTime** property should be used.</span></span>
| `lastModifiedDateTime`   | <span data-ttu-id="af6ef-131">Os itens devem ser organizados pela propriedade **lastModifiedDateTime** dos itens.</span><span class="sxs-lookup"><span data-stu-id="af6ef-131">Items should be arranged by the **lastModifiedDateTime** property of the items.</span></span>
| `sequence`               | <span data-ttu-id="af6ef-132">Os itens seguem uma sequência personalizada especificada pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="af6ef-132">Items follow a custom sequence specified by the user.</span></span>


### <a name="sortorder-options"></a><span data-ttu-id="af6ef-133">opções de sortOrder</span><span class="sxs-lookup"><span data-stu-id="af6ef-133">sortOrder options</span></span>

<span data-ttu-id="af6ef-134">Os seguintes valores são definidos para a propriedade **sortOrder**.</span><span class="sxs-lookup"><span data-stu-id="af6ef-134">The following values are defined for the **sortOrder** property.</span></span>

| <span data-ttu-id="af6ef-135">Valor</span><span class="sxs-lookup"><span data-stu-id="af6ef-135">Value</span></span>        | <span data-ttu-id="af6ef-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="af6ef-136">Description</span></span>
| ------------ | --------------------------------------------------------------
| `ascending`  | <span data-ttu-id="af6ef-137">Os itens devem ser organizados em ordem crescente.</span><span class="sxs-lookup"><span data-stu-id="af6ef-137">Items should be arranged in ascending order.</span></span>
| `descending` | <span data-ttu-id="af6ef-138">Os itens devem ser organizados em ordem decrescente.</span><span class="sxs-lookup"><span data-stu-id="af6ef-138">Items should be arranged in descending order.</span></span>


### <a name="viewtype-options"></a><span data-ttu-id="af6ef-139">opções de ViewType</span><span class="sxs-lookup"><span data-stu-id="af6ef-139">viewType options</span></span>

<span data-ttu-id="af6ef-140">Os seguintes valores são definidos para a propriedade **viewType**.</span><span class="sxs-lookup"><span data-stu-id="af6ef-140">The following values are defined for the **viewType** property.</span></span>

| <span data-ttu-id="af6ef-141">Valor</span><span class="sxs-lookup"><span data-stu-id="af6ef-141">Value</span></span>        | <span data-ttu-id="af6ef-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="af6ef-142">Description</span></span>
| ------------ | --------------------------------------------------------------
| `default`    | <span data-ttu-id="af6ef-143">O tipo de exibição padrão para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="af6ef-143">The default view type for the application.</span></span>
| `icons`      | <span data-ttu-id="af6ef-144">Um modo de exibição que usa ícones para representar driveItems.</span><span class="sxs-lookup"><span data-stu-id="af6ef-144">A view that uses icons to represent driveItems.</span></span>
| `details`    | <span data-ttu-id="af6ef-145">Um modo de exibição com várias colunas que fornecem detalhes adicionais sobre cada item.</span><span class="sxs-lookup"><span data-stu-id="af6ef-145">A view with multiple columns that provide additional details about each item.</span></span>
| `thumbnails` | <span data-ttu-id="af6ef-146">Um modo de exibição que usa miniaturas maiores de driveItems para representar os itens.</span><span class="sxs-lookup"><span data-stu-id="af6ef-146">A view that uses larger thumbnails of driveItems to represent the items.</span></span>


[item-resource]: driveitem.md
[folder-facet]: folder.md

<!-- {
  "type": "#page.annotation",
  "description": "The FolderView facet provides or sets recommendations on the user-experience of a folder.",
  "keywords": "view, folderview, sortby, sortorder, viewtype, coversourceid, folder",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/folderview.md:
      Found potential enums in resource example that weren't defined in a table:(default,icons,details,thumbnails) are in resource, but () are in table",
    "Warning: /api-reference/v1.0/resources/folderview.md:
      Found potential enums in resource example that weren't defined in a table:(default,name,type,size,takenOrCreatedDateTime,lastModifiedDateTime,sequence) are in resource, but () are in table",
    "Warning: /api-reference/v1.0/resources/folderview.md:
      Found potential enums in resource example that weren't defined in a table:(ascending,descending) are in resource, but () are in table"
  ],
  "tocPath": "Facets/FolderView"
} -->
