---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: FolderView
localization_priority: Normal
description: O recurso FolderView fornece ou define recomendações sobre a experiência do usuário de uma pasta.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 67ec2e079348cc45664804d39314e6c81f4548e3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032449"
---
# <a name="folderview-resource-type"></a><span data-ttu-id="62998-103">Tipo de recurso FolderView</span><span class="sxs-lookup"><span data-stu-id="62998-103">FolderView resource type</span></span>

<span data-ttu-id="62998-104">O recurso **FolderView** fornece ou define recomendações sobre a experiência do usuário de uma pasta.</span><span class="sxs-lookup"><span data-stu-id="62998-104">The **FolderView** resource provides or sets recommendations on the user-experience of a folder.</span></span>

<span data-ttu-id="62998-105">Está disponível a partir da propriedade [folder][folder-facet] dos recursos [driveItem][item-resource].</span><span class="sxs-lookup"><span data-stu-id="62998-105">It is available from the [folder][folder-facet] property of [driveItem][item-resource] resources.</span></span>

## <a name="json-representation"></a><span data-ttu-id="62998-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="62998-106">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.folderView" } -->

```json
{
  "sortBy": "default | name | type | size | takenOrCreatedDateTime | lastModifiedDateTime | sequence",
  "sortOrder": "ascending | descending",
  "viewType": "default | icons | details | thumbnails"
}
```

## <a name="properties"></a><span data-ttu-id="62998-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="62998-107">Properties</span></span>

| <span data-ttu-id="62998-108">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="62998-108">Property name</span></span>         | <span data-ttu-id="62998-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="62998-109">Type</span></span>   | <span data-ttu-id="62998-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="62998-110">Description</span></span>
|:----------------------|:-------|:--------------------------------------------
| <span data-ttu-id="62998-111">**sortBy**</span><span class="sxs-lookup"><span data-stu-id="62998-111">**sortBy**</span></span>            | <span data-ttu-id="62998-112">string</span><span class="sxs-lookup"><span data-stu-id="62998-112">string</span></span> | <span data-ttu-id="62998-113">O método pelo qual a pasta deve ser classificada.</span><span class="sxs-lookup"><span data-stu-id="62998-113">The method by which the folder should be sorted.</span></span>
| <span data-ttu-id="62998-114">**sortOrder**</span><span class="sxs-lookup"><span data-stu-id="62998-114">**sortOrder**</span></span>         | <span data-ttu-id="62998-115">string</span><span class="sxs-lookup"><span data-stu-id="62998-115">string</span></span> | <span data-ttu-id="62998-p101">Se for verdadeiro, indica que os itens devem ser classificados em ordem decrescente. Caso contrário, os itens devem ser classificados em ordem crescente.</span><span class="sxs-lookup"><span data-stu-id="62998-p101">If true, indicates that items should be sorted in descending order. Otherwise, items should be sorted ascending.</span></span>
| <span data-ttu-id="62998-118">**viewType**</span><span class="sxs-lookup"><span data-stu-id="62998-118">**viewType**</span></span>          | <span data-ttu-id="62998-119">string</span><span class="sxs-lookup"><span data-stu-id="62998-119">string</span></span> | <span data-ttu-id="62998-120">O tipo de modo de exibição que deve ser usado para representar a pasta.</span><span class="sxs-lookup"><span data-stu-id="62998-120">The type of view that should be used to represent the folder.</span></span>

<span data-ttu-id="62998-121">Você pode usar a propriedade _sortBy_ para controlar a ordem de classificação dos itens em aplicativos que respeitam a faceta **viewType**.</span><span class="sxs-lookup"><span data-stu-id="62998-121">You can use the _sortBy_ property to control the sort order of the items in applications that respect the **viewType** facet.</span></span>

### <a name="sortby-options"></a><span data-ttu-id="62998-122">opções de sortBy</span><span class="sxs-lookup"><span data-stu-id="62998-122">sortBy options</span></span>

<span data-ttu-id="62998-123">Os seguintes valores são definidos para a propriedade **sortBy**.</span><span class="sxs-lookup"><span data-stu-id="62998-123">The following values are defined for the **sortBy** property.</span></span>

| <span data-ttu-id="62998-124">Valor</span><span class="sxs-lookup"><span data-stu-id="62998-124">Value</span></span>                    | <span data-ttu-id="62998-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="62998-125">Description</span></span>
| ------------------------ | --------------------------------------------------
| `default`                | <span data-ttu-id="62998-126">A ordem de classificação padrão do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="62998-126">The default sort order of the application.</span></span>
| `name`                   | <span data-ttu-id="62998-127">Os itens devem ser organizados pela propriedade **name** dos itens.</span><span class="sxs-lookup"><span data-stu-id="62998-127">Items should be arranged by the **name** property of the items.</span></span>
| `type`                   | <span data-ttu-id="62998-128">Os itens devem ser organizados pelo tipo de item.</span><span class="sxs-lookup"><span data-stu-id="62998-128">Items should be arranged by the type of item.</span></span>
| `size`                   | <span data-ttu-id="62998-129">Os itens devem ser organizados pela propriedade **size** dos itens.</span><span class="sxs-lookup"><span data-stu-id="62998-129">Items should be arranged by the **size** property of the items.</span></span>
| `takenOrCreatedDateTime` | <span data-ttu-id="62998-p102">Os itens devem ser organizados pela propriedade **takenDateTime** da faceta **photo**. Se não estiver disponível, a propriedade **createdDateTime** deverá ser usada.</span><span class="sxs-lookup"><span data-stu-id="62998-p102">Items should be arranged by the **takenDateTime** property of the **photo** facet. If not available, the **createdDateTime** property should be used.</span></span>
| `lastModifiedDateTime`   | <span data-ttu-id="62998-132">Os itens devem ser organizados pela propriedade **lastModifiedDateTime** dos itens.</span><span class="sxs-lookup"><span data-stu-id="62998-132">Items should be arranged by the **lastModifiedDateTime** property of the items.</span></span>
| `sequence`               | <span data-ttu-id="62998-133">Os itens seguem uma sequência personalizada especificada pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="62998-133">Items follow a custom sequence specified by the user.</span></span>


### <a name="sortorder-options"></a><span data-ttu-id="62998-134">opções de sortOrder</span><span class="sxs-lookup"><span data-stu-id="62998-134">sortOrder options</span></span>

<span data-ttu-id="62998-135">Os seguintes valores são definidos para a propriedade **sortOrder**.</span><span class="sxs-lookup"><span data-stu-id="62998-135">The following values are defined for the **sortOrder** property.</span></span>

| <span data-ttu-id="62998-136">Valor</span><span class="sxs-lookup"><span data-stu-id="62998-136">Value</span></span>        | <span data-ttu-id="62998-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="62998-137">Description</span></span>
| ------------ | --------------------------------------------------------------
| `ascending`  | <span data-ttu-id="62998-138">Os itens devem ser organizados em ordem crescente.</span><span class="sxs-lookup"><span data-stu-id="62998-138">Items should be arranged in ascending order.</span></span>
| `descending` | <span data-ttu-id="62998-139">Os itens devem ser organizados em ordem decrescente.</span><span class="sxs-lookup"><span data-stu-id="62998-139">Items should be arranged in descending order.</span></span>


### <a name="viewtype-options"></a><span data-ttu-id="62998-140">opções de ViewType</span><span class="sxs-lookup"><span data-stu-id="62998-140">viewType options</span></span>

<span data-ttu-id="62998-141">Os seguintes valores são definidos para a propriedade **viewType**.</span><span class="sxs-lookup"><span data-stu-id="62998-141">The following values are defined for the **viewType** property.</span></span>

| <span data-ttu-id="62998-142">Valor</span><span class="sxs-lookup"><span data-stu-id="62998-142">Value</span></span>        | <span data-ttu-id="62998-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="62998-143">Description</span></span>
| ------------ | --------------------------------------------------------------
| `default`    | <span data-ttu-id="62998-144">O tipo de exibição padrão para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="62998-144">The default view type for the application.</span></span>
| `icons`      | <span data-ttu-id="62998-145">Um modo de exibição que usa ícones para representar driveItems.</span><span class="sxs-lookup"><span data-stu-id="62998-145">A view that uses icons to represent driveItems.</span></span>
| `details`    | <span data-ttu-id="62998-146">Um modo de exibição com várias colunas que fornecem detalhes adicionais sobre cada item.</span><span class="sxs-lookup"><span data-stu-id="62998-146">A view with multiple columns that provide additional details about each item.</span></span>
| `thumbnails` | <span data-ttu-id="62998-147">Um modo de exibição que usa miniaturas maiores de driveItems para representar os itens.</span><span class="sxs-lookup"><span data-stu-id="62998-147">A view that uses larger thumbnails of driveItems to represent the items.</span></span>


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
