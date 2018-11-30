---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: ContentType
ms.openlocfilehash: cda50c2f20df14c733d3bf71e1b84d5b0df225a0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039608"
---
# <a name="contenttype-resource-type"></a><span data-ttu-id="99c0d-102">Tipo de recurso ContentType</span><span class="sxs-lookup"><span data-stu-id="99c0d-102">ContentType resource type</span></span>

> <span data-ttu-id="99c0d-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="99c0d-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="99c0d-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="99c0d-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="99c0d-105">O recurso **contentType** representa um _tipo de conteúdo_ no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="99c0d-105">The **contentType** resource represents a _content type_ in SharePoint.</span></span>
<span data-ttu-id="99c0d-106">Os tipos de conteúdo permitem definir um conjunto de colunas que devem estar presentes em cada [**listItem**][listItem] em uma [**lista**][list].</span><span class="sxs-lookup"><span data-stu-id="99c0d-106">Content types allow you to define a set of columns that must be present on every [**listItem**][listItem] in a [**list**][list].</span></span>

[list]: list.md
[listItem]: listitem.md

## <a name="json-representation"></a><span data-ttu-id="99c0d-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="99c0d-107">JSON representation</span></span>

<span data-ttu-id="99c0d-108">Aqui está uma representação JSON de um recurso **contentType**.</span><span class="sxs-lookup"><span data-stu-id="99c0d-108">Here is a JSON representation of a **contentType** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.contentType" } -->

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

## <a name="properties"></a><span data-ttu-id="99c0d-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="99c0d-109">Properties</span></span>

| <span data-ttu-id="99c0d-110">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="99c0d-110">Property name</span></span>     | <span data-ttu-id="99c0d-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="99c0d-111">Type</span></span>                 | <span data-ttu-id="99c0d-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="99c0d-112">Description</span></span>
|:------------------|:---------------------|:----------------------------------
| <span data-ttu-id="99c0d-113">**description**</span><span class="sxs-lookup"><span data-stu-id="99c0d-113">**description**</span></span>   | <span data-ttu-id="99c0d-114">string</span><span class="sxs-lookup"><span data-stu-id="99c0d-114">string</span></span>               | <span data-ttu-id="99c0d-115">O texto descritivo do item.</span><span class="sxs-lookup"><span data-stu-id="99c0d-115">The descriptive text for the item.</span></span>
| <span data-ttu-id="99c0d-116">**group**</span><span class="sxs-lookup"><span data-stu-id="99c0d-116">**group**</span></span>         | <span data-ttu-id="99c0d-117">string</span><span class="sxs-lookup"><span data-stu-id="99c0d-117">string</span></span>               | <span data-ttu-id="99c0d-118">O nome do grupo ao qual esse tipo de conteúdo pertence.</span><span class="sxs-lookup"><span data-stu-id="99c0d-118">The name of the group this content type belongs to.</span></span> <span data-ttu-id="99c0d-119">Ajuda a organizar os tipos de conteúdo relacionados.</span><span class="sxs-lookup"><span data-stu-id="99c0d-119">Helps organize related content types.</span></span>
| <span data-ttu-id="99c0d-120">**hidden**</span><span class="sxs-lookup"><span data-stu-id="99c0d-120">**hidden**</span></span>        | <span data-ttu-id="99c0d-121">booliano</span><span class="sxs-lookup"><span data-stu-id="99c0d-121">boolean</span></span>              | <span data-ttu-id="99c0d-122">Indica se o tipo de conteúdo está oculto no menu “Novo” da lista.</span><span class="sxs-lookup"><span data-stu-id="99c0d-122">Indicates whether the content type is hidden in the list's 'New' menu.</span></span>
| <span data-ttu-id="99c0d-123">**id**</span><span class="sxs-lookup"><span data-stu-id="99c0d-123">**id**</span></span>            | <span data-ttu-id="99c0d-124">string</span><span class="sxs-lookup"><span data-stu-id="99c0d-124">string</span></span>               | <span data-ttu-id="99c0d-125">O identificador exclusivo do tipo de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="99c0d-125">The unique identifier of the content type.</span></span>
| <span data-ttu-id="99c0d-126">**inheritedFrom**</span><span class="sxs-lookup"><span data-stu-id="99c0d-126">**inheritedFrom**</span></span> | <span data-ttu-id="99c0d-127">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="99c0d-127">[itemReference][]</span></span>    | <span data-ttu-id="99c0d-128">Se esse tipo de conteúdo for herdado de outro escopo (como um site), fornece uma referência para o item no qual o tipo de conteúdo foi definido.</span><span class="sxs-lookup"><span data-stu-id="99c0d-128">If this content type is inherited from another scope (like a site), provides a reference to the item where the content type is defined.</span></span>
| <span data-ttu-id="99c0d-129">**name**</span><span class="sxs-lookup"><span data-stu-id="99c0d-129">**name**</span></span>          | <span data-ttu-id="99c0d-130">string</span><span class="sxs-lookup"><span data-stu-id="99c0d-130">string</span></span>               | <span data-ttu-id="99c0d-131">O nome do tipo de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="99c0d-131">The name of the content type.</span></span>
| <span data-ttu-id="99c0d-132">**order**</span><span class="sxs-lookup"><span data-stu-id="99c0d-132">**order**</span></span>         | <span data-ttu-id="99c0d-133">[contentTypeOrder][]</span><span class="sxs-lookup"><span data-stu-id="99c0d-133">[contentTypeOrder][]</span></span> | <span data-ttu-id="99c0d-134">Especifica a ordem na qual o tipo de conteúdo aparece na seleção da interface do usuário.</span><span class="sxs-lookup"><span data-stu-id="99c0d-134">Specifies the order in which the content type appears in the selection UI.</span></span>
| <span data-ttu-id="99c0d-135">**parentId**</span><span class="sxs-lookup"><span data-stu-id="99c0d-135">**parentId**</span></span>      | <span data-ttu-id="99c0d-136">string</span><span class="sxs-lookup"><span data-stu-id="99c0d-136">string</span></span>               | <span data-ttu-id="99c0d-137">O identificador exclusivo do tipo de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="99c0d-137">The unique identifier of the content type.</span></span>
| <span data-ttu-id="99c0d-138">**readOnly**</span><span class="sxs-lookup"><span data-stu-id="99c0d-138">**readOnly**</span></span>      | <span data-ttu-id="99c0d-139">booliano</span><span class="sxs-lookup"><span data-stu-id="99c0d-139">boolean</span></span>              | <span data-ttu-id="99c0d-140">Se `true`, o tipo de conteúdo não pode ser modificado, a menos que esse valor seja definido primeiro como `false`.</span><span class="sxs-lookup"><span data-stu-id="99c0d-140">If `true`, the content type cannot be modified unless this value is first set to `false`.</span></span>
| <span data-ttu-id="99c0d-141">**sealed**</span><span class="sxs-lookup"><span data-stu-id="99c0d-141">**sealed**</span></span>        | <span data-ttu-id="99c0d-142">booliano</span><span class="sxs-lookup"><span data-stu-id="99c0d-142">boolean</span></span>              | <span data-ttu-id="99c0d-143">Se `true`, o tipo de conteúdo não pode ser modificado por usuários ou por operações de push-down.</span><span class="sxs-lookup"><span data-stu-id="99c0d-143">If `true`, the content type cannot be modified by users or through push-down operations.</span></span> <span data-ttu-id="99c0d-144">Somente administradores de conjunto de sites podem lacrar ou retirar o lacre dos tipos de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="99c0d-144">Only site collection administrators can seal or unseal content types.</span></span>

## <a name="relationships"></a><span data-ttu-id="99c0d-145">Relações</span><span class="sxs-lookup"><span data-stu-id="99c0d-145">Relationships</span></span>

| <span data-ttu-id="99c0d-146">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="99c0d-146">Property name</span></span>   | <span data-ttu-id="99c0d-147">Tipo</span><span class="sxs-lookup"><span data-stu-id="99c0d-147">Type</span></span>                      | <span data-ttu-id="99c0d-148">Descrição</span><span class="sxs-lookup"><span data-stu-id="99c0d-148">Description</span></span>
|:----------------|:--------------------------|:-------------------------------
| <span data-ttu-id="99c0d-149">**columnLinks**</span><span class="sxs-lookup"><span data-stu-id="99c0d-149">**columnLinks**</span></span> | <span data-ttu-id="99c0d-150">Conjunto [columnLink][]</span><span class="sxs-lookup"><span data-stu-id="99c0d-150">[columnLink][] collection</span></span> | <span data-ttu-id="99c0d-151">O conjunto de colunas necessário para este tipo de conteúdo</span><span class="sxs-lookup"><span data-stu-id="99c0d-151">The collection of columns that are required by this content type</span></span>

<span data-ttu-id="99c0d-152">Consulte [Introdução a tipos de conteúdo e publicação de tipo de conteúdo][contentTypeIntro] para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="99c0d-152">See [Introduction to content types and content type publishing][contentTypeIntro] for more information.</span></span>

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
