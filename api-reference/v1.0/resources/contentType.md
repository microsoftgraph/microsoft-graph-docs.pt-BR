---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: ContentType
localization_priority: Normal
description: O recurso contentType representa um tipo de conteúdo no SharePoint.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: b26f9b7a3bafb7b6185aa781c1f842f7c20adab3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029635"
---
# <a name="contenttype-resource-type"></a><span data-ttu-id="37b0f-103">Tipo de recurso ContentType</span><span class="sxs-lookup"><span data-stu-id="37b0f-103">ContentType resource type</span></span>

<span data-ttu-id="37b0f-104">O recurso **contentType** representa um _tipo de conteúdo_ no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="37b0f-104">The **contentType** resource represents a _content type_ in SharePoint.</span></span>
<span data-ttu-id="37b0f-105">Os tipos de conteúdo permitem que você defina um conjunto de colunas que deve estar presente em cada [**ListItem**][listItem] em uma [**lista**][list].</span><span class="sxs-lookup"><span data-stu-id="37b0f-105">Content types allow you to define a set of columns that must be present on every [**listItem**][listItem] in a [**list**][list].</span></span>

[list]: list.md
[listItem]: listitem.md

## <a name="json-representation"></a><span data-ttu-id="37b0f-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="37b0f-106">JSON representation</span></span>

<span data-ttu-id="37b0f-107">Aqui está uma representação JSON de um recurso **contentType**.</span><span class="sxs-lookup"><span data-stu-id="37b0f-107">Here is a JSON representation of a **contentType** resource.</span></span>
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

## <a name="properties"></a><span data-ttu-id="37b0f-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="37b0f-108">Properties</span></span>

| <span data-ttu-id="37b0f-109">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="37b0f-109">Property name</span></span>     | <span data-ttu-id="37b0f-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="37b0f-110">Type</span></span>                 | <span data-ttu-id="37b0f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="37b0f-111">Description</span></span>
|:------------------|:---------------------|:----------------------------------
| <span data-ttu-id="37b0f-112">**description**</span><span class="sxs-lookup"><span data-stu-id="37b0f-112">**description**</span></span>   | <span data-ttu-id="37b0f-113">string</span><span class="sxs-lookup"><span data-stu-id="37b0f-113">string</span></span>               | <span data-ttu-id="37b0f-114">O texto descritivo do item.</span><span class="sxs-lookup"><span data-stu-id="37b0f-114">The descriptive text for the item.</span></span>
| <span data-ttu-id="37b0f-115">**group**</span><span class="sxs-lookup"><span data-stu-id="37b0f-115">**group**</span></span>         | <span data-ttu-id="37b0f-116">string</span><span class="sxs-lookup"><span data-stu-id="37b0f-116">string</span></span>               | <span data-ttu-id="37b0f-117">O nome do grupo ao qual esse tipo de conteúdo pertence.</span><span class="sxs-lookup"><span data-stu-id="37b0f-117">The name of the group this content type belongs to.</span></span> <span data-ttu-id="37b0f-118">Ajuda a organizar os tipos de conteúdo relacionados.</span><span class="sxs-lookup"><span data-stu-id="37b0f-118">Helps organize related content types.</span></span>
| <span data-ttu-id="37b0f-119">**hidden**</span><span class="sxs-lookup"><span data-stu-id="37b0f-119">**hidden**</span></span>        | <span data-ttu-id="37b0f-120">booliano</span><span class="sxs-lookup"><span data-stu-id="37b0f-120">boolean</span></span>              | <span data-ttu-id="37b0f-121">Indica se o tipo de conteúdo está oculto no menu “Novo” da lista.</span><span class="sxs-lookup"><span data-stu-id="37b0f-121">Indicates whether the content type is hidden in the list's 'New' menu.</span></span>
| <span data-ttu-id="37b0f-122">**id**</span><span class="sxs-lookup"><span data-stu-id="37b0f-122">**id**</span></span>            | <span data-ttu-id="37b0f-123">string</span><span class="sxs-lookup"><span data-stu-id="37b0f-123">string</span></span>               | <span data-ttu-id="37b0f-124">O identificador exclusivo do tipo de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="37b0f-124">The unique identifier of the content type.</span></span>
| <span data-ttu-id="37b0f-125">**inheritedFrom**</span><span class="sxs-lookup"><span data-stu-id="37b0f-125">**inheritedFrom**</span></span> | <span data-ttu-id="37b0f-126">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="37b0f-126">[itemReference][]</span></span>    | <span data-ttu-id="37b0f-127">Se esse tipo de conteúdo for herdado de outro escopo (como um site), fornece uma referência para o item no qual o tipo de conteúdo foi definido.</span><span class="sxs-lookup"><span data-stu-id="37b0f-127">If this content type is inherited from another scope (like a site), provides a reference to the item where the content type is defined.</span></span>
| <span data-ttu-id="37b0f-128">**name**</span><span class="sxs-lookup"><span data-stu-id="37b0f-128">**name**</span></span>          | <span data-ttu-id="37b0f-129">string</span><span class="sxs-lookup"><span data-stu-id="37b0f-129">string</span></span>               | <span data-ttu-id="37b0f-130">O nome do tipo de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="37b0f-130">The name of the content type.</span></span>
| <span data-ttu-id="37b0f-131">**order**</span><span class="sxs-lookup"><span data-stu-id="37b0f-131">**order**</span></span>         | <span data-ttu-id="37b0f-132">[contentTypeOrder][]</span><span class="sxs-lookup"><span data-stu-id="37b0f-132">[contentTypeOrder][]</span></span> | <span data-ttu-id="37b0f-133">Especifica a ordem na qual o tipo de conteúdo aparece na seleção da interface do usuário.</span><span class="sxs-lookup"><span data-stu-id="37b0f-133">Specifies the order in which the content type appears in the selection UI.</span></span>
| <span data-ttu-id="37b0f-134">**parentId**</span><span class="sxs-lookup"><span data-stu-id="37b0f-134">**parentId**</span></span>      | <span data-ttu-id="37b0f-135">string</span><span class="sxs-lookup"><span data-stu-id="37b0f-135">string</span></span>               | <span data-ttu-id="37b0f-136">O identificador exclusivo do tipo de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="37b0f-136">The unique identifier of the content type.</span></span>
| <span data-ttu-id="37b0f-137">**readOnly**</span><span class="sxs-lookup"><span data-stu-id="37b0f-137">**readOnly**</span></span>      | <span data-ttu-id="37b0f-138">booliano</span><span class="sxs-lookup"><span data-stu-id="37b0f-138">boolean</span></span>              | <span data-ttu-id="37b0f-139">Se `true`, o tipo de conteúdo não pode ser modificado, a menos que esse valor seja definido primeiro como `false`.</span><span class="sxs-lookup"><span data-stu-id="37b0f-139">If `true`, the content type cannot be modified unless this value is first set to `false`.</span></span>
| <span data-ttu-id="37b0f-140">**sealed**</span><span class="sxs-lookup"><span data-stu-id="37b0f-140">**sealed**</span></span>        | <span data-ttu-id="37b0f-141">booliano</span><span class="sxs-lookup"><span data-stu-id="37b0f-141">boolean</span></span>              | <span data-ttu-id="37b0f-142">Se `true`, o tipo de conteúdo não pode ser modificado por usuários ou por operações de push-down.</span><span class="sxs-lookup"><span data-stu-id="37b0f-142">If `true`, the content type cannot be modified by users or through push-down operations.</span></span> <span data-ttu-id="37b0f-143">Somente administradores de conjunto de sites podem lacrar ou retirar o lacre dos tipos de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="37b0f-143">Only site collection administrators can seal or unseal content types.</span></span>

## <a name="relationships"></a><span data-ttu-id="37b0f-144">Relações</span><span class="sxs-lookup"><span data-stu-id="37b0f-144">Relationships</span></span>

| <span data-ttu-id="37b0f-145">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="37b0f-145">Property name</span></span>   | <span data-ttu-id="37b0f-146">Tipo</span><span class="sxs-lookup"><span data-stu-id="37b0f-146">Type</span></span>                      | <span data-ttu-id="37b0f-147">Descrição</span><span class="sxs-lookup"><span data-stu-id="37b0f-147">Description</span></span>
|:----------------|:--------------------------|:-------------------------------
| <span data-ttu-id="37b0f-148">**columnLinks**</span><span class="sxs-lookup"><span data-stu-id="37b0f-148">**columnLinks**</span></span> | <span data-ttu-id="37b0f-149">Conjunto [columnLink][]</span><span class="sxs-lookup"><span data-stu-id="37b0f-149">[columnLink][] collection</span></span> | <span data-ttu-id="37b0f-150">O conjunto de colunas necessário para este tipo de conteúdo</span><span class="sxs-lookup"><span data-stu-id="37b0f-150">The collection of columns that are required by this content type</span></span>

<span data-ttu-id="37b0f-151">Consulte [Introdução a tipos de conteúdo e publicação de tipo de conteúdo][contentTypeIntro] para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="37b0f-151">See [Introduction to content types and content type publishing][contentTypeIntro] for more information.</span></span>

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
