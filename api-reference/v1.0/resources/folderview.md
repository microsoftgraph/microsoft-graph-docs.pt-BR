---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: FolderView
ms.openlocfilehash: 65fc0a6aa702e6cd08f18dc16957bb7a41589f40
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/28/2017
---
# <a name="folderview-resource-type"></a><span data-ttu-id="82e0d-102">Tipo de recurso FolderView</span><span class="sxs-lookup"><span data-stu-id="82e0d-102">FolderView resource type</span></span>

<span data-ttu-id="82e0d-103">O recurso **FolderView** fornece ou define recomendações sobre a experiência do usuário de uma pasta.</span><span class="sxs-lookup"><span data-stu-id="82e0d-103">The **folderView** facet provides or sets recommendations on the user-experience of a folder.</span></span>

<span data-ttu-id="82e0d-104">Está disponível a partir da propriedade [folder][folder-facet] dos recursos [driveItem][item-resource].</span><span class="sxs-lookup"><span data-stu-id="82e0d-104">It is available from the [folder][folder-facet] property of [driveItem][item-resource] resources.</span></span>

## <a name="json-representation"></a><span data-ttu-id="82e0d-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="82e0d-105">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.folderView" } -->

```json
{
  "sortBy": "default | name | type | size | takenOrCreatedDateTime | lastModifiedDateTime | sequence",
  "sortDescending": "ascending | descending",
  "viewType": "default | icons | details | thumbnails"
}
```

## <a name="properties"></a><span data-ttu-id="82e0d-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="82e0d-106">Properties</span></span>

| <span data-ttu-id="82e0d-107">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="82e0d-107">Property name</span></span>         | <span data-ttu-id="82e0d-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="82e0d-108">Type</span></span>   | <span data-ttu-id="82e0d-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="82e0d-109">Description</span></span>
|:----------------------|:-------|:--------------------------------------------
| <span data-ttu-id="82e0d-110">**sortBy**</span><span class="sxs-lookup"><span data-stu-id="82e0d-110">**sortBy**</span></span>            | <span data-ttu-id="82e0d-111">string</span><span class="sxs-lookup"><span data-stu-id="82e0d-111">string</span></span> | <span data-ttu-id="82e0d-112">O método pelo qual a pasta deve ser classificada.</span><span class="sxs-lookup"><span data-stu-id="82e0d-112">The method by which the folder should be sorted.</span></span>
| <span data-ttu-id="82e0d-113">**sortOrder**</span><span class="sxs-lookup"><span data-stu-id="82e0d-113">**sortOrder values**</span></span>         | <span data-ttu-id="82e0d-114">string</span><span class="sxs-lookup"><span data-stu-id="82e0d-114">string</span></span> | <span data-ttu-id="82e0d-115">Se for verdadeiro, indica que os itens devem ser classificados em ordem decrescente.</span><span class="sxs-lookup"><span data-stu-id="82e0d-115">If true, indicates that items should be sorted in descending order.</span></span> <span data-ttu-id="82e0d-116">Caso contrário, os itens devem ser classificados em ordem crescente.</span><span class="sxs-lookup"><span data-stu-id="82e0d-116">Otherwise, items should be sorted ascending.</span></span>
| <span data-ttu-id="82e0d-117">**viewType**</span><span class="sxs-lookup"><span data-stu-id="82e0d-117">**viewType**</span></span>          | <span data-ttu-id="82e0d-118">string</span><span class="sxs-lookup"><span data-stu-id="82e0d-118">string</span></span> | <span data-ttu-id="82e0d-119">O tipo de modo de exibição que deve ser usado para representar a pasta.</span><span class="sxs-lookup"><span data-stu-id="82e0d-119">The type of view that should be used to represent the folder.</span></span>

<span data-ttu-id="82e0d-120">Você pode usar a propriedade _sortBy_ para controlar a ordem de classificação dos itens em aplicativos que respeitam a faceta **viewType**.</span><span class="sxs-lookup"><span data-stu-id="82e0d-120">You can use the _sortBy_ property to control the sort order of the items in applications that respect the **viewType** facet.</span></span>

### <a name="sortby-values"></a><span data-ttu-id="82e0d-121">Valores sortBy</span><span class="sxs-lookup"><span data-stu-id="82e0d-121">sortBy values</span></span>

<span data-ttu-id="82e0d-122">Os seguintes valores são definidos para a propriedade **sortBy**.</span><span class="sxs-lookup"><span data-stu-id="82e0d-122">The following values are defined for the **sortBy** property.</span></span>

| <span data-ttu-id="82e0d-123">Valor</span><span class="sxs-lookup"><span data-stu-id="82e0d-123">Value</span></span>                    | <span data-ttu-id="82e0d-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="82e0d-124">Description</span></span>
| ------------------------ | --------------------------------------------------
| `default`                | <span data-ttu-id="82e0d-125">A ordem de classificação padrão do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="82e0d-125">The default sort order of the application.</span></span>
| `name`                   | <span data-ttu-id="82e0d-126">Os itens devem ser organizados pela propriedade **name** dos itens.</span><span class="sxs-lookup"><span data-stu-id="82e0d-126">Items should be arranged by the **name** property of the items.</span></span>
| `type`                   | <span data-ttu-id="82e0d-127">Os itens devem ser organizados pelo tipo de item.</span><span class="sxs-lookup"><span data-stu-id="82e0d-127">Items should be arranged by the type of item.</span></span>
| `size`                   | <span data-ttu-id="82e0d-128">Os itens devem ser organizados pela propriedade **size** dos itens.</span><span class="sxs-lookup"><span data-stu-id="82e0d-128">Items should be arranged by the **size** property of the items.</span></span>
| `takenOrCreatedDateTime` | <span data-ttu-id="82e0d-129">Os itens devem ser organizados pela propriedade **takenDateTime** da faceta **photo**.</span><span class="sxs-lookup"><span data-stu-id="82e0d-129">Items should be arranged by the **takenDateTime** property of the **photo** facet.</span></span> <span data-ttu-id="82e0d-130">Se não estiver disponível, a propriedade **createdDateTime** deverá ser usada.</span><span class="sxs-lookup"><span data-stu-id="82e0d-130">If not available, the **createdDateTime** property should be used.</span></span>
| `lastModifiedDateTime`   | <span data-ttu-id="82e0d-131">Os itens devem ser organizados pela propriedade **lastModifiedDateTime** dos itens.</span><span class="sxs-lookup"><span data-stu-id="82e0d-131">Items should be arranged by the **lastModifiedDateTime** property of the items.</span></span>
| `sequence`               | <span data-ttu-id="82e0d-132">Os itens seguem uma sequência personalizada especificada pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="82e0d-132">Items follow a custom sequence specified by the user.</span></span>


### <a name="sortorder-values"></a><span data-ttu-id="82e0d-133">Valores sortOrder</span><span class="sxs-lookup"><span data-stu-id="82e0d-133">sortOrder values</span></span>

<span data-ttu-id="82e0d-134">Os seguintes valores são definidos para a propriedade **sortOrder**.</span><span class="sxs-lookup"><span data-stu-id="82e0d-134">The following values are defined for the **sortOrder** property.</span></span>

| <span data-ttu-id="82e0d-135">Valor</span><span class="sxs-lookup"><span data-stu-id="82e0d-135">Value</span></span>        | <span data-ttu-id="82e0d-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="82e0d-136">Description</span></span>
| ------------ | --------------------------------------------------------------
| `ascending`  | <span data-ttu-id="82e0d-137">Os itens devem ser organizados em ordem crescente.</span><span class="sxs-lookup"><span data-stu-id="82e0d-137">Items should be arranged in ascending order.</span></span>
| `descending` | <span data-ttu-id="82e0d-138">Os itens devem ser organizados em ordem decrescente.</span><span class="sxs-lookup"><span data-stu-id="82e0d-138">Items should be arranged in descending order.</span></span>


### <a name="viewtype-values"></a><span data-ttu-id="82e0d-139">Valores viewType</span><span class="sxs-lookup"><span data-stu-id="82e0d-139">viewType values</span></span>

<span data-ttu-id="82e0d-140">Os seguintes valores são definidos para a propriedade **viewType**.</span><span class="sxs-lookup"><span data-stu-id="82e0d-140">The following values are defined for the **viewType** property.</span></span>

| <span data-ttu-id="82e0d-141">Valor</span><span class="sxs-lookup"><span data-stu-id="82e0d-141">Value</span></span>        | <span data-ttu-id="82e0d-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="82e0d-142">Description</span></span>
| ------------ | --------------------------------------------------------------
| `default`    | <span data-ttu-id="82e0d-143">O tipo de exibição padrão para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="82e0d-143">The default view type for the application.</span></span>
| `icons`      | <span data-ttu-id="82e0d-144">Um modo de exibição que usa ícones para representar driveItems.</span><span class="sxs-lookup"><span data-stu-id="82e0d-144">A view that uses icons to represent driveItems.</span></span>
| `details`    | <span data-ttu-id="82e0d-145">Um modo de exibição com várias colunas que fornecem detalhes adicionais sobre cada item.</span><span class="sxs-lookup"><span data-stu-id="82e0d-145">A view with multiple columns that provide additional details about each item.</span></span>
| `thumbnails` | <span data-ttu-id="82e0d-146">Um modo de exibição que usa miniaturas maiores de driveItems para representar os itens.</span><span class="sxs-lookup"><span data-stu-id="82e0d-146">A view that uses larger thumbnails of driveItems to represent the items.</span></span>


[item-resource]: driveitem.md
[folder-facet]: folder.md

<!-- {
  "type": "#page.annotation",
  "description": "The FolderView facet provides or sets recommendations on the user-experience of a folder.",
  "keywords": "view, folderview, sortby, sortorder, viewtype, coversourceid, folder",
  "section": "documentation",
  "tocPath": "Facets/FolderView"
} -->
