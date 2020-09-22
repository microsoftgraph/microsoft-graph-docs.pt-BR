---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: ContentType
localization_priority: Normal
description: O recurso contentType representa um tipo de conteúdo no SharePoint.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 71652c2e314cd4f86a7bf0a957b1df937aa0d2e3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48056965"
---
# <a name="contenttype-resource-type"></a><span data-ttu-id="15d5f-103">Tipo de recurso ContentType</span><span class="sxs-lookup"><span data-stu-id="15d5f-103">ContentType resource type</span></span>

<span data-ttu-id="15d5f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="15d5f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="15d5f-105">O recurso **contentType** representa um _tipo de conteúdo_ no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="15d5f-105">The **contentType** resource represents a _content type_ in SharePoint.</span></span>
<span data-ttu-id="15d5f-106">Os tipos de conteúdo permitem que você defina um conjunto de colunas que deve estar presente em cada [**ListItem**][listItem] em uma [**lista**][list].</span><span class="sxs-lookup"><span data-stu-id="15d5f-106">Content types allow you to define a set of columns that must be present on every [**listItem**][listItem] in a [**list**][list].</span></span>

[list]: list.md
[listItem]: listitem.md

## <a name="json-representation"></a><span data-ttu-id="15d5f-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="15d5f-107">JSON representation</span></span>

<span data-ttu-id="15d5f-108">Aqui está uma representação JSON de um recurso **contentType**.</span><span class="sxs-lookup"><span data-stu-id="15d5f-108">Here is a JSON representation of a **contentType** resource.</span></span>
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

## <a name="properties"></a><span data-ttu-id="15d5f-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="15d5f-109">Properties</span></span>

| <span data-ttu-id="15d5f-110">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="15d5f-110">Property name</span></span>     | <span data-ttu-id="15d5f-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="15d5f-111">Type</span></span>                 | <span data-ttu-id="15d5f-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="15d5f-112">Description</span></span>
|:------------------|:---------------------|:----------------------------------
| <span data-ttu-id="15d5f-113">**description**</span><span class="sxs-lookup"><span data-stu-id="15d5f-113">**description**</span></span>   | <span data-ttu-id="15d5f-114">string</span><span class="sxs-lookup"><span data-stu-id="15d5f-114">string</span></span>               | <span data-ttu-id="15d5f-115">O texto descritivo do item.</span><span class="sxs-lookup"><span data-stu-id="15d5f-115">The descriptive text for the item.</span></span>
| <span data-ttu-id="15d5f-116">**group**</span><span class="sxs-lookup"><span data-stu-id="15d5f-116">**group**</span></span>         | <span data-ttu-id="15d5f-117">string</span><span class="sxs-lookup"><span data-stu-id="15d5f-117">string</span></span>               | <span data-ttu-id="15d5f-118">O nome do grupo ao qual esse tipo de conteúdo pertence.</span><span class="sxs-lookup"><span data-stu-id="15d5f-118">The name of the group this content type belongs to.</span></span> <span data-ttu-id="15d5f-119">Ajuda a organizar os tipos de conteúdo relacionados.</span><span class="sxs-lookup"><span data-stu-id="15d5f-119">Helps organize related content types.</span></span>
| <span data-ttu-id="15d5f-120">**hidden**</span><span class="sxs-lookup"><span data-stu-id="15d5f-120">**hidden**</span></span>        | <span data-ttu-id="15d5f-121">booliano</span><span class="sxs-lookup"><span data-stu-id="15d5f-121">boolean</span></span>              | <span data-ttu-id="15d5f-122">Indica se o tipo de conteúdo está oculto no menu “Novo” da lista.</span><span class="sxs-lookup"><span data-stu-id="15d5f-122">Indicates whether the content type is hidden in the list's 'New' menu.</span></span>
| <span data-ttu-id="15d5f-123">**id**</span><span class="sxs-lookup"><span data-stu-id="15d5f-123">**id**</span></span>            | <span data-ttu-id="15d5f-124">string</span><span class="sxs-lookup"><span data-stu-id="15d5f-124">string</span></span>               | <span data-ttu-id="15d5f-125">O identificador exclusivo do tipo de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="15d5f-125">The unique identifier of the content type.</span></span>
| <span data-ttu-id="15d5f-126">**inheritedFrom**</span><span class="sxs-lookup"><span data-stu-id="15d5f-126">**inheritedFrom**</span></span> | <span data-ttu-id="15d5f-127">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="15d5f-127">[itemReference][]</span></span>    | <span data-ttu-id="15d5f-128">Se esse tipo de conteúdo for herdado de outro escopo (como um site), fornece uma referência para o item no qual o tipo de conteúdo foi definido.</span><span class="sxs-lookup"><span data-stu-id="15d5f-128">If this content type is inherited from another scope (like a site), provides a reference to the item where the content type is defined.</span></span>
| <span data-ttu-id="15d5f-129">**name**</span><span class="sxs-lookup"><span data-stu-id="15d5f-129">**name**</span></span>          | <span data-ttu-id="15d5f-130">string</span><span class="sxs-lookup"><span data-stu-id="15d5f-130">string</span></span>               | <span data-ttu-id="15d5f-131">O nome do tipo de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="15d5f-131">The name of the content type.</span></span>
| <span data-ttu-id="15d5f-132">**order**</span><span class="sxs-lookup"><span data-stu-id="15d5f-132">**order**</span></span>         | <span data-ttu-id="15d5f-133">[contentTypeOrder][]</span><span class="sxs-lookup"><span data-stu-id="15d5f-133">[contentTypeOrder][]</span></span> | <span data-ttu-id="15d5f-134">Especifica a ordem na qual o tipo de conteúdo aparece na seleção da interface do usuário.</span><span class="sxs-lookup"><span data-stu-id="15d5f-134">Specifies the order in which the content type appears in the selection UI.</span></span>
| <span data-ttu-id="15d5f-135">**parentId**</span><span class="sxs-lookup"><span data-stu-id="15d5f-135">**parentId**</span></span>      | <span data-ttu-id="15d5f-136">string</span><span class="sxs-lookup"><span data-stu-id="15d5f-136">string</span></span>               | <span data-ttu-id="15d5f-137">O identificador exclusivo do tipo de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="15d5f-137">The unique identifier of the content type.</span></span>
| <span data-ttu-id="15d5f-138">**readOnly**</span><span class="sxs-lookup"><span data-stu-id="15d5f-138">**readOnly**</span></span>      | <span data-ttu-id="15d5f-139">booliano</span><span class="sxs-lookup"><span data-stu-id="15d5f-139">boolean</span></span>              | <span data-ttu-id="15d5f-140">Se `true`, o tipo de conteúdo não pode ser modificado, a menos que esse valor seja definido primeiro como `false`.</span><span class="sxs-lookup"><span data-stu-id="15d5f-140">If `true`, the content type cannot be modified unless this value is first set to `false`.</span></span>
| <span data-ttu-id="15d5f-141">**sealed**</span><span class="sxs-lookup"><span data-stu-id="15d5f-141">**sealed**</span></span>        | <span data-ttu-id="15d5f-142">booliano</span><span class="sxs-lookup"><span data-stu-id="15d5f-142">boolean</span></span>              | <span data-ttu-id="15d5f-143">Se `true`, o tipo de conteúdo não pode ser modificado por usuários ou por operações de push-down.</span><span class="sxs-lookup"><span data-stu-id="15d5f-143">If `true`, the content type cannot be modified by users or through push-down operations.</span></span> <span data-ttu-id="15d5f-144">Somente administradores de conjunto de sites podem lacrar ou retirar o lacre dos tipos de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="15d5f-144">Only site collection administrators can seal or unseal content types.</span></span>

## <a name="relationships"></a><span data-ttu-id="15d5f-145">Relações</span><span class="sxs-lookup"><span data-stu-id="15d5f-145">Relationships</span></span>

| <span data-ttu-id="15d5f-146">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="15d5f-146">Property name</span></span>   | <span data-ttu-id="15d5f-147">Tipo</span><span class="sxs-lookup"><span data-stu-id="15d5f-147">Type</span></span>                      | <span data-ttu-id="15d5f-148">Descrição</span><span class="sxs-lookup"><span data-stu-id="15d5f-148">Description</span></span>
|:----------------|:--------------------------|:-------------------------------
| <span data-ttu-id="15d5f-149">**columnLinks**</span><span class="sxs-lookup"><span data-stu-id="15d5f-149">**columnLinks**</span></span> | <span data-ttu-id="15d5f-150">Conjunto [columnLink][]</span><span class="sxs-lookup"><span data-stu-id="15d5f-150">[columnLink][] collection</span></span> | <span data-ttu-id="15d5f-151">O conjunto de colunas necessário para este tipo de conteúdo</span><span class="sxs-lookup"><span data-stu-id="15d5f-151">The collection of columns that are required by this content type</span></span>

<span data-ttu-id="15d5f-152">Consulte [Introdução a tipos de conteúdo e publicação de tipo de conteúdo][contentTypeIntro] para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="15d5f-152">See [Introduction to content types and content type publishing][contentTypeIntro] for more information.</span></span>

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

