---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: ContentType
localization_priority: Normal
description: O recurso contentType representa um tipo de conteúdo no SharePoint.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: c05ed39c0f92b209925fc9a722c5562999ae438c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531786"
---
# <a name="contenttype-resource-type"></a><span data-ttu-id="65bd0-103">Tipo de recurso ContentType</span><span class="sxs-lookup"><span data-stu-id="65bd0-103">ContentType resource type</span></span>

<span data-ttu-id="65bd0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="65bd0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="65bd0-105">O recurso **contentType** representa um _tipo de conteúdo_ no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="65bd0-105">The **contentType** resource represents a _content type_ in SharePoint.</span></span>
<span data-ttu-id="65bd0-106">Os tipos de conteúdo permitem que você defina um conjunto de colunas que deve estar presente em cada [**ListItem**][listItem] em uma [**lista**][list].</span><span class="sxs-lookup"><span data-stu-id="65bd0-106">Content types allow you to define a set of columns that must be present on every [**listItem**][listItem] in a [**list**][list].</span></span>

[list]: list.md
[listItem]: listitem.md

## <a name="json-representation"></a><span data-ttu-id="65bd0-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="65bd0-107">JSON representation</span></span>

<span data-ttu-id="65bd0-108">Aqui está uma representação JSON de um recurso **contentType**.</span><span class="sxs-lookup"><span data-stu-id="65bd0-108">Here is a JSON representation of a **contentType** resource.</span></span>
<!-- {
  "blockType": "resource",
 "baseType": "microsoft.graph.entity",
 "@odata.type": "microsoft.graph.contentType" } -->

```json
{
  "description": "string",
  "group": "string",
  "hidden": false,
  "id": "string",
  "inheritedFrom": { "@type": "microsoft.graph.itemReference" },
  "name": "string",
  "order": { "@type": "microsoft.graph.contentTypeOrder" },
  "parentId": "string",
  "readOnly": false,
  "sealed": false,

  "columnLinks": [{ "@type": "microsoft.graph.columnLink" }]
}
```

## <a name="properties"></a><span data-ttu-id="65bd0-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="65bd0-109">Properties</span></span>

| <span data-ttu-id="65bd0-110">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="65bd0-110">Property name</span></span>     | <span data-ttu-id="65bd0-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="65bd0-111">Type</span></span>                 | <span data-ttu-id="65bd0-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="65bd0-112">Description</span></span>
|:------------------|:---------------------|:----------------------------------
| <span data-ttu-id="65bd0-113">**description**</span><span class="sxs-lookup"><span data-stu-id="65bd0-113">**description**</span></span>   | <span data-ttu-id="65bd0-114">string</span><span class="sxs-lookup"><span data-stu-id="65bd0-114">string</span></span>               | <span data-ttu-id="65bd0-115">O texto descritivo do item.</span><span class="sxs-lookup"><span data-stu-id="65bd0-115">The descriptive text for the item.</span></span>
| <span data-ttu-id="65bd0-116">**group**</span><span class="sxs-lookup"><span data-stu-id="65bd0-116">**group**</span></span>         | <span data-ttu-id="65bd0-117">string</span><span class="sxs-lookup"><span data-stu-id="65bd0-117">string</span></span>               | <span data-ttu-id="65bd0-118">O nome do grupo ao qual esse tipo de conteúdo pertence.</span><span class="sxs-lookup"><span data-stu-id="65bd0-118">The name of the group this content type belongs to.</span></span> <span data-ttu-id="65bd0-119">Ajuda a organizar os tipos de conteúdo relacionados.</span><span class="sxs-lookup"><span data-stu-id="65bd0-119">Helps organize related content types.</span></span>
| <span data-ttu-id="65bd0-120">**hidden**</span><span class="sxs-lookup"><span data-stu-id="65bd0-120">**hidden**</span></span>        | <span data-ttu-id="65bd0-121">booliano</span><span class="sxs-lookup"><span data-stu-id="65bd0-121">boolean</span></span>              | <span data-ttu-id="65bd0-122">Indica se o tipo de conteúdo está oculto no menu “Novo” da lista.</span><span class="sxs-lookup"><span data-stu-id="65bd0-122">Indicates whether the content type is hidden in the list's 'New' menu.</span></span>
| <span data-ttu-id="65bd0-123">**id**</span><span class="sxs-lookup"><span data-stu-id="65bd0-123">**id**</span></span>            | <span data-ttu-id="65bd0-124">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="65bd0-124">string</span></span>               | <span data-ttu-id="65bd0-125">O identificador exclusivo do tipo de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="65bd0-125">The unique identifier of the content type.</span></span>
| <span data-ttu-id="65bd0-126">**inheritedFrom**</span><span class="sxs-lookup"><span data-stu-id="65bd0-126">**inheritedFrom**</span></span> | <span data-ttu-id="65bd0-127">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="65bd0-127">[itemReference][]</span></span>    | <span data-ttu-id="65bd0-128">Se esse tipo de conteúdo for herdado de outro escopo (como um site), fornece uma referência para o item no qual o tipo de conteúdo foi definido.</span><span class="sxs-lookup"><span data-stu-id="65bd0-128">If this content type is inherited from another scope (like a site), provides a reference to the item where the content type is defined.</span></span>
| <span data-ttu-id="65bd0-129">**name**</span><span class="sxs-lookup"><span data-stu-id="65bd0-129">**name**</span></span>          | <span data-ttu-id="65bd0-130">string</span><span class="sxs-lookup"><span data-stu-id="65bd0-130">string</span></span>               | <span data-ttu-id="65bd0-131">O nome do tipo de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="65bd0-131">The name of the content type.</span></span>
| <span data-ttu-id="65bd0-132">**order**</span><span class="sxs-lookup"><span data-stu-id="65bd0-132">**order**</span></span>         | <span data-ttu-id="65bd0-133">[contentTypeOrder][]</span><span class="sxs-lookup"><span data-stu-id="65bd0-133">[contentTypeOrder][]</span></span> | <span data-ttu-id="65bd0-134">Especifica a ordem na qual o tipo de conteúdo aparece na seleção da interface do usuário.</span><span class="sxs-lookup"><span data-stu-id="65bd0-134">Specifies the order in which the content type appears in the selection UI.</span></span>
| <span data-ttu-id="65bd0-135">**parentId**</span><span class="sxs-lookup"><span data-stu-id="65bd0-135">**parentId**</span></span>      | <span data-ttu-id="65bd0-136">string</span><span class="sxs-lookup"><span data-stu-id="65bd0-136">string</span></span>               | <span data-ttu-id="65bd0-137">O identificador exclusivo do tipo de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="65bd0-137">The unique identifier of the content type.</span></span>
| <span data-ttu-id="65bd0-138">**readOnly**</span><span class="sxs-lookup"><span data-stu-id="65bd0-138">**readOnly**</span></span>      | <span data-ttu-id="65bd0-139">booliano</span><span class="sxs-lookup"><span data-stu-id="65bd0-139">boolean</span></span>              | <span data-ttu-id="65bd0-140">Se `true`, o tipo de conteúdo não pode ser modificado, a menos que esse valor seja definido primeiro como `false`.</span><span class="sxs-lookup"><span data-stu-id="65bd0-140">If `true`, the content type cannot be modified unless this value is first set to `false`.</span></span>
| <span data-ttu-id="65bd0-141">**sealed**</span><span class="sxs-lookup"><span data-stu-id="65bd0-141">**sealed**</span></span>        | <span data-ttu-id="65bd0-142">booliano</span><span class="sxs-lookup"><span data-stu-id="65bd0-142">boolean</span></span>              | <span data-ttu-id="65bd0-143">Se `true`, o tipo de conteúdo não pode ser modificado por usuários ou por operações de push-down.</span><span class="sxs-lookup"><span data-stu-id="65bd0-143">If `true`, the content type cannot be modified by users or through push-down operations.</span></span> <span data-ttu-id="65bd0-144">Somente administradores de conjunto de sites podem lacrar ou retirar o lacre dos tipos de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="65bd0-144">Only site collection administrators can seal or unseal content types.</span></span>

## <a name="relationships"></a><span data-ttu-id="65bd0-145">Relações</span><span class="sxs-lookup"><span data-stu-id="65bd0-145">Relationships</span></span>

| <span data-ttu-id="65bd0-146">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="65bd0-146">Property name</span></span>   | <span data-ttu-id="65bd0-147">Tipo</span><span class="sxs-lookup"><span data-stu-id="65bd0-147">Type</span></span>                      | <span data-ttu-id="65bd0-148">Descrição</span><span class="sxs-lookup"><span data-stu-id="65bd0-148">Description</span></span>
|:----------------|:--------------------------|:-------------------------------
| <span data-ttu-id="65bd0-149">**columnLinks**</span><span class="sxs-lookup"><span data-stu-id="65bd0-149">**columnLinks**</span></span> | <span data-ttu-id="65bd0-150">Conjunto [columnLink][]</span><span class="sxs-lookup"><span data-stu-id="65bd0-150">[columnLink][] collection</span></span> | <span data-ttu-id="65bd0-151">O conjunto de colunas necessário para este tipo de conteúdo</span><span class="sxs-lookup"><span data-stu-id="65bd0-151">The collection of columns that are required by this content type</span></span>

<span data-ttu-id="65bd0-152">Consulte [Introdução a tipos de conteúdo e publicação de tipo de conteúdo][contentTypeIntro] para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="65bd0-152">See [Introduction to content types and content type publishing][contentTypeIntro] for more information.</span></span>

[columnLink]: columnlink.md
[contentTypeIntro]: https://support.office.com/en-us/article/Introduction-to-content-types-and-content-type-publishing-e1277a2e-a1e8-4473-9126-91a0647766e5
[itemReference]: itemreference.md
[contentTypeOrder]: contenttypeorder.md

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ContentType"
} -->
