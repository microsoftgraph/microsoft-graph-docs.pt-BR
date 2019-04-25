---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: ContentType
localization_priority: Normal
ms.openlocfilehash: c90dd8889d07f903a7d3c79d9e4e5db3b9f2a30b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535402"
---
# <a name="contenttype-resource-type"></a><span data-ttu-id="44ffa-102">Tipo de recurso ContentType</span><span class="sxs-lookup"><span data-stu-id="44ffa-102">ContentType resource type</span></span>

<span data-ttu-id="44ffa-103">O recurso **contentType** representa um _tipo de conteúdo_ no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="44ffa-103">The **contentType** resource represents a _content type_ in SharePoint.</span></span>
<span data-ttu-id="44ffa-104">Os tipos de conteúdo permitem definir um conjunto de colunas que devem estar presentes em cada [**listItem**][listItem] em uma [**lista**][list].</span><span class="sxs-lookup"><span data-stu-id="44ffa-104">Content types allow you to define a set of columns that must be present on every [**listItem**][listItem] in a [**list**][list].</span></span>

[list]: list.md
[listItem]: listitem.md

## <a name="json-representation"></a><span data-ttu-id="44ffa-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="44ffa-105">JSON representation</span></span>

<span data-ttu-id="44ffa-106">Aqui está uma representação JSON de um recurso **contentType**.</span><span class="sxs-lookup"><span data-stu-id="44ffa-106">Here is a JSON representation of a **contentType** resource.</span></span>
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

## <a name="properties"></a><span data-ttu-id="44ffa-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="44ffa-107">Properties</span></span>

| <span data-ttu-id="44ffa-108">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="44ffa-108">Property name</span></span>     | <span data-ttu-id="44ffa-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="44ffa-109">Type</span></span>                 | <span data-ttu-id="44ffa-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="44ffa-110">Description</span></span>
|:------------------|:---------------------|:----------------------------------
| <span data-ttu-id="44ffa-111">**description**</span><span class="sxs-lookup"><span data-stu-id="44ffa-111">**description**</span></span>   | <span data-ttu-id="44ffa-112">string</span><span class="sxs-lookup"><span data-stu-id="44ffa-112">string</span></span>               | <span data-ttu-id="44ffa-113">O texto descritivo do item.</span><span class="sxs-lookup"><span data-stu-id="44ffa-113">The descriptive text for the item.</span></span>
| <span data-ttu-id="44ffa-114">**group**</span><span class="sxs-lookup"><span data-stu-id="44ffa-114">**group**</span></span>         | <span data-ttu-id="44ffa-115">string</span><span class="sxs-lookup"><span data-stu-id="44ffa-115">string</span></span>               | <span data-ttu-id="44ffa-116">O nome do grupo ao qual esse tipo de conteúdo pertence.</span><span class="sxs-lookup"><span data-stu-id="44ffa-116">The name of the group this content type belongs to.</span></span> <span data-ttu-id="44ffa-117">Ajuda a organizar os tipos de conteúdo relacionados.</span><span class="sxs-lookup"><span data-stu-id="44ffa-117">Helps organize related content types.</span></span>
| <span data-ttu-id="44ffa-118">**hidden**</span><span class="sxs-lookup"><span data-stu-id="44ffa-118">**hidden**</span></span>        | <span data-ttu-id="44ffa-119">booliano</span><span class="sxs-lookup"><span data-stu-id="44ffa-119">boolean</span></span>              | <span data-ttu-id="44ffa-120">Indica se o tipo de conteúdo está oculto no menu “Novo” da lista.</span><span class="sxs-lookup"><span data-stu-id="44ffa-120">Indicates whether the content type is hidden in the list's 'New' menu.</span></span>
| <span data-ttu-id="44ffa-121">**id**</span><span class="sxs-lookup"><span data-stu-id="44ffa-121">**id**</span></span>            | <span data-ttu-id="44ffa-122">string</span><span class="sxs-lookup"><span data-stu-id="44ffa-122">string</span></span>               | <span data-ttu-id="44ffa-123">O identificador exclusivo do tipo de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="44ffa-123">The unique identifier of the content type.</span></span>
| <span data-ttu-id="44ffa-124">**inheritedFrom**</span><span class="sxs-lookup"><span data-stu-id="44ffa-124">**inheritedFrom**</span></span> | <span data-ttu-id="44ffa-125">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="44ffa-125">[itemReference][]</span></span>    | <span data-ttu-id="44ffa-126">Se esse tipo de conteúdo for herdado de outro escopo (como um site), fornece uma referência para o item no qual o tipo de conteúdo foi definido.</span><span class="sxs-lookup"><span data-stu-id="44ffa-126">If this content type is inherited from another scope (like a site), provides a reference to the item where the content type is defined.</span></span>
| <span data-ttu-id="44ffa-127">**name**</span><span class="sxs-lookup"><span data-stu-id="44ffa-127">**name**</span></span>          | <span data-ttu-id="44ffa-128">string</span><span class="sxs-lookup"><span data-stu-id="44ffa-128">string</span></span>               | <span data-ttu-id="44ffa-129">O nome do tipo de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="44ffa-129">The name of the content type.</span></span>
| <span data-ttu-id="44ffa-130">**order**</span><span class="sxs-lookup"><span data-stu-id="44ffa-130">**order**</span></span>         | <span data-ttu-id="44ffa-131">[contentTypeOrder][]</span><span class="sxs-lookup"><span data-stu-id="44ffa-131">[contentTypeOrder][]</span></span> | <span data-ttu-id="44ffa-132">Especifica a ordem na qual o tipo de conteúdo aparece na seleção da interface do usuário.</span><span class="sxs-lookup"><span data-stu-id="44ffa-132">Specifies the order in which the content type appears in the selection UI.</span></span>
| <span data-ttu-id="44ffa-133">**parentId**</span><span class="sxs-lookup"><span data-stu-id="44ffa-133">**parentId**</span></span>      | <span data-ttu-id="44ffa-134">string</span><span class="sxs-lookup"><span data-stu-id="44ffa-134">string</span></span>               | <span data-ttu-id="44ffa-135">O identificador exclusivo do tipo de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="44ffa-135">The unique identifier of the content type.</span></span>
| <span data-ttu-id="44ffa-136">**readOnly**</span><span class="sxs-lookup"><span data-stu-id="44ffa-136">**readOnly**</span></span>      | <span data-ttu-id="44ffa-137">booliano</span><span class="sxs-lookup"><span data-stu-id="44ffa-137">boolean</span></span>              | <span data-ttu-id="44ffa-138">Se `true`, o tipo de conteúdo não pode ser modificado, a menos que esse valor seja definido primeiro como `false`.</span><span class="sxs-lookup"><span data-stu-id="44ffa-138">If `true`, the content type cannot be modified unless this value is first set to `false`.</span></span>
| <span data-ttu-id="44ffa-139">**sealed**</span><span class="sxs-lookup"><span data-stu-id="44ffa-139">**sealed**</span></span>        | <span data-ttu-id="44ffa-140">booliano</span><span class="sxs-lookup"><span data-stu-id="44ffa-140">boolean</span></span>              | <span data-ttu-id="44ffa-141">Se `true`, o tipo de conteúdo não pode ser modificado por usuários ou por operações de push-down.</span><span class="sxs-lookup"><span data-stu-id="44ffa-141">If `true`, the content type cannot be modified by users or through push-down operations.</span></span> <span data-ttu-id="44ffa-142">Somente administradores de conjunto de sites podem lacrar ou retirar o lacre dos tipos de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="44ffa-142">Only site collection administrators can seal or unseal content types.</span></span>

## <a name="relationships"></a><span data-ttu-id="44ffa-143">Relações</span><span class="sxs-lookup"><span data-stu-id="44ffa-143">Relationships</span></span>

| <span data-ttu-id="44ffa-144">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="44ffa-144">Property name</span></span>   | <span data-ttu-id="44ffa-145">Tipo</span><span class="sxs-lookup"><span data-stu-id="44ffa-145">Type</span></span>                      | <span data-ttu-id="44ffa-146">Descrição</span><span class="sxs-lookup"><span data-stu-id="44ffa-146">Description</span></span>
|:----------------|:--------------------------|:-------------------------------
| <span data-ttu-id="44ffa-147">**columnLinks**</span><span class="sxs-lookup"><span data-stu-id="44ffa-147">**columnLinks**</span></span> | <span data-ttu-id="44ffa-148">Conjunto [columnLink][]</span><span class="sxs-lookup"><span data-stu-id="44ffa-148">[columnLink][] collection</span></span> | <span data-ttu-id="44ffa-149">O conjunto de colunas necessário para este tipo de conteúdo</span><span class="sxs-lookup"><span data-stu-id="44ffa-149">The collection of columns that are required by this content type</span></span>

<span data-ttu-id="44ffa-150">Consulte [Introdução a tipos de conteúdo e publicação de tipo de conteúdo][contentTypeIntro] para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="44ffa-150">See [Introduction to content types and content type publishing][contentTypeIntro] for more information.</span></span>

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
