---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: FolderView
localization_priority: Normal
ms.openlocfilehash: 717dd93d82f109926cabf0168e4e176d7c68cd35
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27861534"
---
# <a name="folderview-resource-type"></a><span data-ttu-id="6f8a8-102">Tipo de recurso FolderView</span><span class="sxs-lookup"><span data-stu-id="6f8a8-102">FolderView resource type</span></span>

> <span data-ttu-id="6f8a8-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="6f8a8-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6f8a8-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="6f8a8-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6f8a8-105">O recurso **FolderView** fornece ou define recomendações sobre a experiência do usuário de uma pasta.</span><span class="sxs-lookup"><span data-stu-id="6f8a8-105">The **FolderView** resource provides or sets recommendations on the user-experience of a folder.</span></span>

<span data-ttu-id="6f8a8-106">Está disponível a partir da propriedade [folder][folder-facet] dos recursos [driveItem][item-resource].</span><span class="sxs-lookup"><span data-stu-id="6f8a8-106">It is available from the [folder][folder-facet] property of [driveItem][item-resource] resources.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6f8a8-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6f8a8-107">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.folderView" } -->

```json
{
  "sortBy": "default | name | type | size | takenOrCreatedDateTime | lastModifiedDateTime | sequence",
  "sortDescending": "ascending | descending",
  "viewType": "default | icons | details | thumbnails"
}
```

## <a name="properties"></a><span data-ttu-id="6f8a8-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6f8a8-108">Properties</span></span>

| <span data-ttu-id="6f8a8-109">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="6f8a8-109">Property name</span></span>         | <span data-ttu-id="6f8a8-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="6f8a8-110">Type</span></span>   | <span data-ttu-id="6f8a8-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="6f8a8-111">Description</span></span>
|:----------------------|:-------|:--------------------------------------------
| <span data-ttu-id="6f8a8-112">**sortBy**</span><span class="sxs-lookup"><span data-stu-id="6f8a8-112">**sortBy**</span></span>            | <span data-ttu-id="6f8a8-113">string</span><span class="sxs-lookup"><span data-stu-id="6f8a8-113">string</span></span> | <span data-ttu-id="6f8a8-114">O método pelo qual a pasta deve ser classificada.</span><span class="sxs-lookup"><span data-stu-id="6f8a8-114">The method by which the folder should be sorted.</span></span>
| <span data-ttu-id="6f8a8-115">**sortOrder**</span><span class="sxs-lookup"><span data-stu-id="6f8a8-115">**sortOrder**</span></span>         | <span data-ttu-id="6f8a8-116">string</span><span class="sxs-lookup"><span data-stu-id="6f8a8-116">string</span></span> | <span data-ttu-id="6f8a8-117">Se for verdadeiro, indica que os itens devem ser classificados em ordem decrescente.</span><span class="sxs-lookup"><span data-stu-id="6f8a8-117">If true, indicates that items should be sorted in descending order.</span></span> <span data-ttu-id="6f8a8-118">Caso contrário, os itens devem ser classificados em ordem crescente.</span><span class="sxs-lookup"><span data-stu-id="6f8a8-118">Otherwise, items should be sorted ascending.</span></span>
| <span data-ttu-id="6f8a8-119">**viewType**</span><span class="sxs-lookup"><span data-stu-id="6f8a8-119">**viewType**</span></span>          | <span data-ttu-id="6f8a8-120">string</span><span class="sxs-lookup"><span data-stu-id="6f8a8-120">string</span></span> | <span data-ttu-id="6f8a8-121">O tipo de modo de exibição que deve ser usado para representar a pasta.</span><span class="sxs-lookup"><span data-stu-id="6f8a8-121">The type of view that should be used to represent the folder.</span></span>

<span data-ttu-id="6f8a8-122">Você pode usar a propriedade _sortBy_ para controlar a ordem de classificação dos itens em aplicativos que respeitam a faceta **viewType**.</span><span class="sxs-lookup"><span data-stu-id="6f8a8-122">You can use the _sortBy_ property to control the sort order of the items in applications that respect the **viewType** facet.</span></span>

### <a name="sortby-values"></a><span data-ttu-id="6f8a8-123">Valores sortBy</span><span class="sxs-lookup"><span data-stu-id="6f8a8-123">sortBy values</span></span>

<span data-ttu-id="6f8a8-124">Os seguintes valores são definidos para a propriedade **sortBy**.</span><span class="sxs-lookup"><span data-stu-id="6f8a8-124">The following values are defined for the **sortBy** property.</span></span>

| <span data-ttu-id="6f8a8-125">Valor</span><span class="sxs-lookup"><span data-stu-id="6f8a8-125">Value</span></span>                    | <span data-ttu-id="6f8a8-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="6f8a8-126">Description</span></span>
| ------------------------ | --------------------------------------------------
| `default`                | <span data-ttu-id="6f8a8-127">A ordem de classificação padrão do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6f8a8-127">The default sort order of the application.</span></span>
| `name`                   | <span data-ttu-id="6f8a8-128">Os itens devem ser organizados pela propriedade **name** dos itens.</span><span class="sxs-lookup"><span data-stu-id="6f8a8-128">Items should be arranged by the **name** property of the items.</span></span>
| `type`                   | <span data-ttu-id="6f8a8-129">Os itens devem ser organizados pelo tipo de item.</span><span class="sxs-lookup"><span data-stu-id="6f8a8-129">Items should be arranged by the type of item.</span></span>
| `size`                   | <span data-ttu-id="6f8a8-130">Os itens devem ser organizados pela propriedade **size** dos itens.</span><span class="sxs-lookup"><span data-stu-id="6f8a8-130">Items should be arranged by the **size** property of the items.</span></span>
| `takenOrCreatedDateTime` | <span data-ttu-id="6f8a8-131">Os itens devem ser organizados pela propriedade **takenDateTime** da faceta **photo**.</span><span class="sxs-lookup"><span data-stu-id="6f8a8-131">Items should be arranged by the **takenDateTime** property of the **photo** facet.</span></span> <span data-ttu-id="6f8a8-132">Se não estiver disponível, a propriedade **createdDateTime** deverá ser usada.</span><span class="sxs-lookup"><span data-stu-id="6f8a8-132">If not available, the **createdDateTime** property should be used.</span></span>
| `lastModifiedDateTime`   | <span data-ttu-id="6f8a8-133">Os itens devem ser organizados pela propriedade **lastModifiedDateTime** dos itens.</span><span class="sxs-lookup"><span data-stu-id="6f8a8-133">Items should be arranged by the **lastModifiedDateTime** property of the items.</span></span>
| `sequence`               | <span data-ttu-id="6f8a8-134">Os itens seguem uma sequência personalizada especificada pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="6f8a8-134">Items follow a custom sequence specified by the user.</span></span>


### <a name="sortorder-values"></a><span data-ttu-id="6f8a8-135">Valores sortOrder</span><span class="sxs-lookup"><span data-stu-id="6f8a8-135">sortOrder values</span></span>

<span data-ttu-id="6f8a8-136">Os seguintes valores são definidos para a propriedade **sortOrder**.</span><span class="sxs-lookup"><span data-stu-id="6f8a8-136">The following values are defined for the **sortOrder** property.</span></span>

| <span data-ttu-id="6f8a8-137">Valor</span><span class="sxs-lookup"><span data-stu-id="6f8a8-137">Value</span></span>        | <span data-ttu-id="6f8a8-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="6f8a8-138">Description</span></span>
| ------------ | --------------------------------------------------------------
| `ascending`  | <span data-ttu-id="6f8a8-139">Os itens devem ser organizados em ordem crescente.</span><span class="sxs-lookup"><span data-stu-id="6f8a8-139">Items should be arranged in ascending order.</span></span>
| `descending` | <span data-ttu-id="6f8a8-140">Os itens devem ser organizados em ordem decrescente.</span><span class="sxs-lookup"><span data-stu-id="6f8a8-140">Items should be arranged in descending order.</span></span>


### <a name="viewtype-values"></a><span data-ttu-id="6f8a8-141">Valores viewType</span><span class="sxs-lookup"><span data-stu-id="6f8a8-141">viewType values</span></span>

<span data-ttu-id="6f8a8-142">Os seguintes valores são definidos para a propriedade **viewType**.</span><span class="sxs-lookup"><span data-stu-id="6f8a8-142">The following values are defined for the **viewType** property.</span></span>

| <span data-ttu-id="6f8a8-143">Valor</span><span class="sxs-lookup"><span data-stu-id="6f8a8-143">Value</span></span>        | <span data-ttu-id="6f8a8-144">Descrição</span><span class="sxs-lookup"><span data-stu-id="6f8a8-144">Description</span></span>
| ------------ | --------------------------------------------------------------
| `default`    | <span data-ttu-id="6f8a8-145">O tipo de exibição padrão para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6f8a8-145">The default view type for the application.</span></span>
| `icons`      | <span data-ttu-id="6f8a8-146">Um modo de exibição que usa ícones para representar driveItems.</span><span class="sxs-lookup"><span data-stu-id="6f8a8-146">A view that uses icons to represent driveItems.</span></span>
| `details`    | <span data-ttu-id="6f8a8-147">Um modo de exibição com várias colunas que fornecem detalhes adicionais sobre cada item.</span><span class="sxs-lookup"><span data-stu-id="6f8a8-147">A view with multiple columns that provide additional details about each item.</span></span>
| `thumbnails` | <span data-ttu-id="6f8a8-148">Um modo de exibição que usa miniaturas maiores de driveItems para representar os itens.</span><span class="sxs-lookup"><span data-stu-id="6f8a8-148">A view that uses larger thumbnails of driveItems to represent the items.</span></span>


[item-resource]: driveitem.md
[folder-facet]: folder.md

<!-- uuid: f9e446fd-190b-4692-a605-bb60e78f1f19
2017-05-03 02:34:40 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "folderView resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
