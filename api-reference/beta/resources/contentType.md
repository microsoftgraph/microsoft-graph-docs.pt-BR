---
author: daspek
description: O recurso contentType representa um tipo de conteúdo no SharePoint.
ms.date: 09/12/2017
title: ContentType
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: b7376b431154595f9b3d2de1931918b629e74acb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36012860"
---
# <a name="contenttype-resource-type"></a><span data-ttu-id="d416c-103">Tipo de recurso ContentType</span><span class="sxs-lookup"><span data-stu-id="d416c-103">ContentType resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d416c-104">O recurso **contentType** representa um _tipo de conteúdo_ no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="d416c-104">The **contentType** resource represents a _content type_ in SharePoint.</span></span>
<span data-ttu-id="d416c-105">Os tipos de conteúdo permitem que você defina um conjunto de colunas que deve estar presente em cada [**ListItem**][listItem] em uma [**lista**][list].</span><span class="sxs-lookup"><span data-stu-id="d416c-105">Content types allow you to define a set of columns that must be present on every [**listItem**][listItem] in a [**list**][list].</span></span>

[list]: list.md
[listItem]: listitem.md

## <a name="json-representation"></a><span data-ttu-id="d416c-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d416c-106">JSON representation</span></span>

<span data-ttu-id="d416c-107">Aqui está uma representação JSON de um recurso **contentType**.</span><span class="sxs-lookup"><span data-stu-id="d416c-107">Here is a JSON representation of a **contentType** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.contentType","keyProperty":"id" } -->

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

## <a name="properties"></a><span data-ttu-id="d416c-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d416c-108">Properties</span></span>

| <span data-ttu-id="d416c-109">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="d416c-109">Property name</span></span>     | <span data-ttu-id="d416c-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="d416c-110">Type</span></span>                 | <span data-ttu-id="d416c-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d416c-111">Description</span></span>
|:------------------|:---------------------|:----------------------------------
| <span data-ttu-id="d416c-112">**description**</span><span class="sxs-lookup"><span data-stu-id="d416c-112">**description**</span></span>   | <span data-ttu-id="d416c-113">string</span><span class="sxs-lookup"><span data-stu-id="d416c-113">string</span></span>               | <span data-ttu-id="d416c-114">O texto descritivo do item.</span><span class="sxs-lookup"><span data-stu-id="d416c-114">The descriptive text for the item.</span></span>
| <span data-ttu-id="d416c-115">**group**</span><span class="sxs-lookup"><span data-stu-id="d416c-115">**group**</span></span>         | <span data-ttu-id="d416c-116">string</span><span class="sxs-lookup"><span data-stu-id="d416c-116">string</span></span>               | <span data-ttu-id="d416c-117">O nome do grupo ao qual esse tipo de conteúdo pertence.</span><span class="sxs-lookup"><span data-stu-id="d416c-117">The name of the group this content type belongs to.</span></span> <span data-ttu-id="d416c-118">Ajuda a organizar os tipos de conteúdo relacionados.</span><span class="sxs-lookup"><span data-stu-id="d416c-118">Helps organize related content types.</span></span>
| <span data-ttu-id="d416c-119">**hidden**</span><span class="sxs-lookup"><span data-stu-id="d416c-119">**hidden**</span></span>        | <span data-ttu-id="d416c-120">booliano</span><span class="sxs-lookup"><span data-stu-id="d416c-120">boolean</span></span>              | <span data-ttu-id="d416c-121">Indica se o tipo de conteúdo está oculto no menu “Novo” da lista.</span><span class="sxs-lookup"><span data-stu-id="d416c-121">Indicates whether the content type is hidden in the list's 'New' menu.</span></span>
| <span data-ttu-id="d416c-122">**id**</span><span class="sxs-lookup"><span data-stu-id="d416c-122">**id**</span></span>            | <span data-ttu-id="d416c-123">string</span><span class="sxs-lookup"><span data-stu-id="d416c-123">string</span></span>               | <span data-ttu-id="d416c-124">O identificador exclusivo do tipo de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="d416c-124">The unique identifier of the content type.</span></span>
| <span data-ttu-id="d416c-125">**inheritedFrom**</span><span class="sxs-lookup"><span data-stu-id="d416c-125">**inheritedFrom**</span></span> | <span data-ttu-id="d416c-126">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="d416c-126">[itemReference][]</span></span>    | <span data-ttu-id="d416c-127">Se esse tipo de conteúdo for herdado de outro escopo (como um site), fornece uma referência para o item no qual o tipo de conteúdo foi definido.</span><span class="sxs-lookup"><span data-stu-id="d416c-127">If this content type is inherited from another scope (like a site), provides a reference to the item where the content type is defined.</span></span>
| <span data-ttu-id="d416c-128">**name**</span><span class="sxs-lookup"><span data-stu-id="d416c-128">**name**</span></span>          | <span data-ttu-id="d416c-129">string</span><span class="sxs-lookup"><span data-stu-id="d416c-129">string</span></span>               | <span data-ttu-id="d416c-130">O nome do tipo de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="d416c-130">The name of the content type.</span></span>
| <span data-ttu-id="d416c-131">**order**</span><span class="sxs-lookup"><span data-stu-id="d416c-131">**order**</span></span>         | <span data-ttu-id="d416c-132">[contentTypeOrder][]</span><span class="sxs-lookup"><span data-stu-id="d416c-132">[contentTypeOrder][]</span></span> | <span data-ttu-id="d416c-133">Especifica a ordem na qual o tipo de conteúdo aparece na seleção da interface do usuário.</span><span class="sxs-lookup"><span data-stu-id="d416c-133">Specifies the order in which the content type appears in the selection UI.</span></span>
| <span data-ttu-id="d416c-134">**parentId**</span><span class="sxs-lookup"><span data-stu-id="d416c-134">**parentId**</span></span>      | <span data-ttu-id="d416c-135">string</span><span class="sxs-lookup"><span data-stu-id="d416c-135">string</span></span>               | <span data-ttu-id="d416c-136">O identificador exclusivo do tipo de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="d416c-136">The unique identifier of the content type.</span></span>
| <span data-ttu-id="d416c-137">**readOnly**</span><span class="sxs-lookup"><span data-stu-id="d416c-137">**readOnly**</span></span>      | <span data-ttu-id="d416c-138">booliano</span><span class="sxs-lookup"><span data-stu-id="d416c-138">boolean</span></span>              | <span data-ttu-id="d416c-139">Se `true`, o tipo de conteúdo não pode ser modificado, a menos que esse valor seja definido primeiro como `false`.</span><span class="sxs-lookup"><span data-stu-id="d416c-139">If `true`, the content type cannot be modified unless this value is first set to `false`.</span></span>
| <span data-ttu-id="d416c-140">**sealed**</span><span class="sxs-lookup"><span data-stu-id="d416c-140">**sealed**</span></span>        | <span data-ttu-id="d416c-141">booliano</span><span class="sxs-lookup"><span data-stu-id="d416c-141">boolean</span></span>              | <span data-ttu-id="d416c-142">Se `true`, o tipo de conteúdo não pode ser modificado por usuários ou por operações de push-down.</span><span class="sxs-lookup"><span data-stu-id="d416c-142">If `true`, the content type cannot be modified by users or through push-down operations.</span></span> <span data-ttu-id="d416c-143">Somente administradores de conjunto de sites podem lacrar ou retirar o lacre dos tipos de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="d416c-143">Only site collection administrators can seal or unseal content types.</span></span>

## <a name="relationships"></a><span data-ttu-id="d416c-144">Relações</span><span class="sxs-lookup"><span data-stu-id="d416c-144">Relationships</span></span>

| <span data-ttu-id="d416c-145">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="d416c-145">Property name</span></span>   | <span data-ttu-id="d416c-146">Tipo</span><span class="sxs-lookup"><span data-stu-id="d416c-146">Type</span></span>                      | <span data-ttu-id="d416c-147">Descrição</span><span class="sxs-lookup"><span data-stu-id="d416c-147">Description</span></span>
|:----------------|:--------------------------|:-------------------------------
| <span data-ttu-id="d416c-148">**columnLinks**</span><span class="sxs-lookup"><span data-stu-id="d416c-148">**columnLinks**</span></span> | <span data-ttu-id="d416c-149">Conjunto [columnLink][]</span><span class="sxs-lookup"><span data-stu-id="d416c-149">[columnLink][] collection</span></span> | <span data-ttu-id="d416c-150">O conjunto de colunas necessário para este tipo de conteúdo</span><span class="sxs-lookup"><span data-stu-id="d416c-150">The collection of columns that are required by this content type</span></span>

<span data-ttu-id="d416c-151">Consulte [Introdução a tipos de conteúdo e publicação de tipo de conteúdo][contentTypeIntro] para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="d416c-151">See [Introduction to content types and content type publishing][contentTypeIntro] for more information.</span></span>

[columnLink]: columnlink.md
[contentTypeIntro]: https://support.office.com/en-us/article/Introduction-to-content-types-and-content-type-publishing-e1277a2e-a1e8-4473-9126-91a0647766e5
[itemReference]: itemreference.md
[contentTypeOrder]: contenttypeorder.md

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ContentType",
  "suppressions": []
}
-->
