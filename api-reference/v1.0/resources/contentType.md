---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: ContentType
localization_priority: Normal
ms.openlocfilehash: c7d4b3222ec64432d6a2c9921e53ce409de3f139
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876731"
---
# <a name="contenttype-resource-type"></a><span data-ttu-id="7eccb-102">Tipo de recurso ContentType</span><span class="sxs-lookup"><span data-stu-id="7eccb-102">ContentType resource type</span></span>

<span data-ttu-id="7eccb-103">O recurso **contentType** representa um _tipo de conteúdo_ no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="7eccb-103">The **contentType** resource represents a _content type_ in SharePoint.</span></span>
<span data-ttu-id="7eccb-104">Os tipos de conteúdo permitem definir um conjunto de colunas que devem estar presentes em cada [**listItem**][listItem] em uma [**lista**][list].</span><span class="sxs-lookup"><span data-stu-id="7eccb-104">Content types allow you to define a set of columns that must be present on every [**listItem**][listItem] in a [**list**][list].</span></span>

[list]: list.md
[listItem]: listitem.md

## <a name="json-representation"></a><span data-ttu-id="7eccb-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7eccb-105">JSON representation</span></span>

<span data-ttu-id="7eccb-106">Aqui está uma representação JSON de um recurso **contentType**.</span><span class="sxs-lookup"><span data-stu-id="7eccb-106">Here is a JSON representation of a **contentType** resource.</span></span>
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

## <a name="properties"></a><span data-ttu-id="7eccb-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7eccb-107">Properties</span></span>

| <span data-ttu-id="7eccb-108">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="7eccb-108">Property name</span></span>     | <span data-ttu-id="7eccb-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="7eccb-109">Type</span></span>                 | <span data-ttu-id="7eccb-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="7eccb-110">Description</span></span>
|:------------------|:---------------------|:----------------------------------
| <span data-ttu-id="7eccb-111">**description**</span><span class="sxs-lookup"><span data-stu-id="7eccb-111">**description**</span></span>   | <span data-ttu-id="7eccb-112">string</span><span class="sxs-lookup"><span data-stu-id="7eccb-112">string</span></span>               | <span data-ttu-id="7eccb-113">O texto descritivo do item.</span><span class="sxs-lookup"><span data-stu-id="7eccb-113">The descriptive text for the item.</span></span>
| <span data-ttu-id="7eccb-114">**group**</span><span class="sxs-lookup"><span data-stu-id="7eccb-114">**group**</span></span>         | <span data-ttu-id="7eccb-115">string</span><span class="sxs-lookup"><span data-stu-id="7eccb-115">string</span></span>               | <span data-ttu-id="7eccb-116">O nome do grupo ao qual esse tipo de conteúdo pertence.</span><span class="sxs-lookup"><span data-stu-id="7eccb-116">The name of the group this content type belongs to.</span></span> <span data-ttu-id="7eccb-117">Ajuda a organizar os tipos de conteúdo relacionados.</span><span class="sxs-lookup"><span data-stu-id="7eccb-117">Helps organize related content types.</span></span>
| <span data-ttu-id="7eccb-118">**hidden**</span><span class="sxs-lookup"><span data-stu-id="7eccb-118">**hidden**</span></span>        | <span data-ttu-id="7eccb-119">booliano</span><span class="sxs-lookup"><span data-stu-id="7eccb-119">boolean</span></span>              | <span data-ttu-id="7eccb-120">Indica se o tipo de conteúdo está oculto no menu “Novo” da lista.</span><span class="sxs-lookup"><span data-stu-id="7eccb-120">Indicates whether the content type is hidden in the list's 'New' menu.</span></span>
| <span data-ttu-id="7eccb-121">**id**</span><span class="sxs-lookup"><span data-stu-id="7eccb-121">**id**</span></span>            | <span data-ttu-id="7eccb-122">string</span><span class="sxs-lookup"><span data-stu-id="7eccb-122">string</span></span>               | <span data-ttu-id="7eccb-123">O identificador exclusivo do tipo de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="7eccb-123">The unique identifier of the content type.</span></span>
| <span data-ttu-id="7eccb-124">**inheritedFrom**</span><span class="sxs-lookup"><span data-stu-id="7eccb-124">**inheritedFrom**</span></span> | <span data-ttu-id="7eccb-125">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="7eccb-125">[itemReference][]</span></span>    | <span data-ttu-id="7eccb-126">Se esse tipo de conteúdo for herdado de outro escopo (como um site), fornece uma referência para o item no qual o tipo de conteúdo foi definido.</span><span class="sxs-lookup"><span data-stu-id="7eccb-126">If this content type is inherited from another scope (like a site), provides a reference to the item where the content type is defined.</span></span>
| <span data-ttu-id="7eccb-127">**name**</span><span class="sxs-lookup"><span data-stu-id="7eccb-127">**name**</span></span>          | <span data-ttu-id="7eccb-128">string</span><span class="sxs-lookup"><span data-stu-id="7eccb-128">string</span></span>               | <span data-ttu-id="7eccb-129">O nome do tipo de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="7eccb-129">The name of the content type.</span></span>
| <span data-ttu-id="7eccb-130">**order**</span><span class="sxs-lookup"><span data-stu-id="7eccb-130">**order**</span></span>         | <span data-ttu-id="7eccb-131">[contentTypeOrder][]</span><span class="sxs-lookup"><span data-stu-id="7eccb-131">[contentTypeOrder][]</span></span> | <span data-ttu-id="7eccb-132">Especifica a ordem na qual o tipo de conteúdo aparece na seleção da interface do usuário.</span><span class="sxs-lookup"><span data-stu-id="7eccb-132">Specifies the order in which the content type appears in the selection UI.</span></span>
| <span data-ttu-id="7eccb-133">**parentId**</span><span class="sxs-lookup"><span data-stu-id="7eccb-133">**parentId**</span></span>      | <span data-ttu-id="7eccb-134">string</span><span class="sxs-lookup"><span data-stu-id="7eccb-134">string</span></span>               | <span data-ttu-id="7eccb-135">O identificador exclusivo do tipo de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="7eccb-135">The unique identifier of the content type.</span></span>
| <span data-ttu-id="7eccb-136">**readOnly**</span><span class="sxs-lookup"><span data-stu-id="7eccb-136">**readOnly**</span></span>      | <span data-ttu-id="7eccb-137">booliano</span><span class="sxs-lookup"><span data-stu-id="7eccb-137">boolean</span></span>              | <span data-ttu-id="7eccb-138">Se `true`, o tipo de conteúdo não pode ser modificado, a menos que esse valor seja definido primeiro como `false`.</span><span class="sxs-lookup"><span data-stu-id="7eccb-138">If `true`, the content type cannot be modified unless this value is first set to `false`.</span></span>
| <span data-ttu-id="7eccb-139">**sealed**</span><span class="sxs-lookup"><span data-stu-id="7eccb-139">**sealed**</span></span>        | <span data-ttu-id="7eccb-140">booliano</span><span class="sxs-lookup"><span data-stu-id="7eccb-140">boolean</span></span>              | <span data-ttu-id="7eccb-141">Se `true`, o tipo de conteúdo não pode ser modificado por usuários ou por operações de push-down.</span><span class="sxs-lookup"><span data-stu-id="7eccb-141">If `true`, the content type cannot be modified by users or through push-down operations.</span></span> <span data-ttu-id="7eccb-142">Somente administradores de conjunto de sites podem lacrar ou retirar o lacre dos tipos de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="7eccb-142">Only site collection administrators can seal or unseal content types.</span></span>

## <a name="relationships"></a><span data-ttu-id="7eccb-143">Relações</span><span class="sxs-lookup"><span data-stu-id="7eccb-143">Relationships</span></span>

| <span data-ttu-id="7eccb-144">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="7eccb-144">Property name</span></span>   | <span data-ttu-id="7eccb-145">Tipo</span><span class="sxs-lookup"><span data-stu-id="7eccb-145">Type</span></span>                      | <span data-ttu-id="7eccb-146">Descrição</span><span class="sxs-lookup"><span data-stu-id="7eccb-146">Description</span></span>
|:----------------|:--------------------------|:-------------------------------
| <span data-ttu-id="7eccb-147">**columnLinks**</span><span class="sxs-lookup"><span data-stu-id="7eccb-147">**columnLinks**</span></span> | <span data-ttu-id="7eccb-148">Conjunto [columnLink][]</span><span class="sxs-lookup"><span data-stu-id="7eccb-148">[columnLink][] collection</span></span> | <span data-ttu-id="7eccb-149">O conjunto de colunas necessário para este tipo de conteúdo</span><span class="sxs-lookup"><span data-stu-id="7eccb-149">The collection of columns that are required by this content type</span></span>

<span data-ttu-id="7eccb-150">Consulte [Introdução a tipos de conteúdo e publicação de tipo de conteúdo][contentTypeIntro] para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="7eccb-150">See [Introduction to content types and content type publishing][contentTypeIntro] for more information.</span></span>

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
