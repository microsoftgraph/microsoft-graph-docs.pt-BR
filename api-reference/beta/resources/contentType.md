---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: ContentType
localization_priority: Normal
ms.openlocfilehash: 75c6bd39c62b55fee45f82240c37aee61b080c99
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27856792"
---
# <a name="contenttype-resource-type"></a><span data-ttu-id="3a538-102">Tipo de recurso ContentType</span><span class="sxs-lookup"><span data-stu-id="3a538-102">ContentType resource type</span></span>

> <span data-ttu-id="3a538-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="3a538-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3a538-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3a538-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3a538-105">O recurso **contentType** representa um _tipo de conteúdo_ no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="3a538-105">The **contentType** resource represents a _content type_ in SharePoint.</span></span>
<span data-ttu-id="3a538-106">Os tipos de conteúdo permitem definir um conjunto de colunas que devem estar presentes em cada [**listItem**][listItem] em uma [**lista**][list].</span><span class="sxs-lookup"><span data-stu-id="3a538-106">Content types allow you to define a set of columns that must be present on every [**listItem**][listItem] in a [**list**][list].</span></span>

[list]: list.md
[listItem]: listitem.md

## <a name="json-representation"></a><span data-ttu-id="3a538-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3a538-107">JSON representation</span></span>

<span data-ttu-id="3a538-108">Aqui está uma representação JSON de um recurso **contentType**.</span><span class="sxs-lookup"><span data-stu-id="3a538-108">Here is a JSON representation of a **contentType** resource.</span></span>
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

## <a name="properties"></a><span data-ttu-id="3a538-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3a538-109">Properties</span></span>

| <span data-ttu-id="3a538-110">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="3a538-110">Property name</span></span>     | <span data-ttu-id="3a538-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="3a538-111">Type</span></span>                 | <span data-ttu-id="3a538-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="3a538-112">Description</span></span>
|:------------------|:---------------------|:----------------------------------
| <span data-ttu-id="3a538-113">**description**</span><span class="sxs-lookup"><span data-stu-id="3a538-113">**description**</span></span>   | <span data-ttu-id="3a538-114">string</span><span class="sxs-lookup"><span data-stu-id="3a538-114">string</span></span>               | <span data-ttu-id="3a538-115">O texto descritivo do item.</span><span class="sxs-lookup"><span data-stu-id="3a538-115">The descriptive text for the item.</span></span>
| <span data-ttu-id="3a538-116">**group**</span><span class="sxs-lookup"><span data-stu-id="3a538-116">**group**</span></span>         | <span data-ttu-id="3a538-117">string</span><span class="sxs-lookup"><span data-stu-id="3a538-117">string</span></span>               | <span data-ttu-id="3a538-118">O nome do grupo ao qual esse tipo de conteúdo pertence.</span><span class="sxs-lookup"><span data-stu-id="3a538-118">The name of the group this content type belongs to.</span></span> <span data-ttu-id="3a538-119">Ajuda a organizar os tipos de conteúdo relacionados.</span><span class="sxs-lookup"><span data-stu-id="3a538-119">Helps organize related content types.</span></span>
| <span data-ttu-id="3a538-120">**hidden**</span><span class="sxs-lookup"><span data-stu-id="3a538-120">**hidden**</span></span>        | <span data-ttu-id="3a538-121">booliano</span><span class="sxs-lookup"><span data-stu-id="3a538-121">boolean</span></span>              | <span data-ttu-id="3a538-122">Indica se o tipo de conteúdo está oculto no menu “Novo” da lista.</span><span class="sxs-lookup"><span data-stu-id="3a538-122">Indicates whether the content type is hidden in the list's 'New' menu.</span></span>
| <span data-ttu-id="3a538-123">**id**</span><span class="sxs-lookup"><span data-stu-id="3a538-123">**id**</span></span>            | <span data-ttu-id="3a538-124">string</span><span class="sxs-lookup"><span data-stu-id="3a538-124">string</span></span>               | <span data-ttu-id="3a538-125">O identificador exclusivo do tipo de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="3a538-125">The unique identifier of the content type.</span></span>
| <span data-ttu-id="3a538-126">**inheritedFrom**</span><span class="sxs-lookup"><span data-stu-id="3a538-126">**inheritedFrom**</span></span> | <span data-ttu-id="3a538-127">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="3a538-127">[itemReference][]</span></span>    | <span data-ttu-id="3a538-128">Se esse tipo de conteúdo for herdado de outro escopo (como um site), fornece uma referência para o item no qual o tipo de conteúdo foi definido.</span><span class="sxs-lookup"><span data-stu-id="3a538-128">If this content type is inherited from another scope (like a site), provides a reference to the item where the content type is defined.</span></span>
| <span data-ttu-id="3a538-129">**name**</span><span class="sxs-lookup"><span data-stu-id="3a538-129">**name**</span></span>          | <span data-ttu-id="3a538-130">string</span><span class="sxs-lookup"><span data-stu-id="3a538-130">string</span></span>               | <span data-ttu-id="3a538-131">O nome do tipo de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="3a538-131">The name of the content type.</span></span>
| <span data-ttu-id="3a538-132">**order**</span><span class="sxs-lookup"><span data-stu-id="3a538-132">**order**</span></span>         | <span data-ttu-id="3a538-133">[contentTypeOrder][]</span><span class="sxs-lookup"><span data-stu-id="3a538-133">[contentTypeOrder][]</span></span> | <span data-ttu-id="3a538-134">Especifica a ordem na qual o tipo de conteúdo aparece na seleção da interface do usuário.</span><span class="sxs-lookup"><span data-stu-id="3a538-134">Specifies the order in which the content type appears in the selection UI.</span></span>
| <span data-ttu-id="3a538-135">**parentId**</span><span class="sxs-lookup"><span data-stu-id="3a538-135">**parentId**</span></span>      | <span data-ttu-id="3a538-136">string</span><span class="sxs-lookup"><span data-stu-id="3a538-136">string</span></span>               | <span data-ttu-id="3a538-137">O identificador exclusivo do tipo de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="3a538-137">The unique identifier of the content type.</span></span>
| <span data-ttu-id="3a538-138">**readOnly**</span><span class="sxs-lookup"><span data-stu-id="3a538-138">**readOnly**</span></span>      | <span data-ttu-id="3a538-139">booliano</span><span class="sxs-lookup"><span data-stu-id="3a538-139">boolean</span></span>              | <span data-ttu-id="3a538-140">Se `true`, o tipo de conteúdo não pode ser modificado, a menos que esse valor seja definido primeiro como `false`.</span><span class="sxs-lookup"><span data-stu-id="3a538-140">If `true`, the content type cannot be modified unless this value is first set to `false`.</span></span>
| <span data-ttu-id="3a538-141">**sealed**</span><span class="sxs-lookup"><span data-stu-id="3a538-141">**sealed**</span></span>        | <span data-ttu-id="3a538-142">booliano</span><span class="sxs-lookup"><span data-stu-id="3a538-142">boolean</span></span>              | <span data-ttu-id="3a538-143">Se `true`, o tipo de conteúdo não pode ser modificado por usuários ou por operações de push-down.</span><span class="sxs-lookup"><span data-stu-id="3a538-143">If `true`, the content type cannot be modified by users or through push-down operations.</span></span> <span data-ttu-id="3a538-144">Somente administradores de conjunto de sites podem lacrar ou retirar o lacre dos tipos de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="3a538-144">Only site collection administrators can seal or unseal content types.</span></span>

## <a name="relationships"></a><span data-ttu-id="3a538-145">Relações</span><span class="sxs-lookup"><span data-stu-id="3a538-145">Relationships</span></span>

| <span data-ttu-id="3a538-146">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="3a538-146">Property name</span></span>   | <span data-ttu-id="3a538-147">Tipo</span><span class="sxs-lookup"><span data-stu-id="3a538-147">Type</span></span>                      | <span data-ttu-id="3a538-148">Descrição</span><span class="sxs-lookup"><span data-stu-id="3a538-148">Description</span></span>
|:----------------|:--------------------------|:-------------------------------
| <span data-ttu-id="3a538-149">**columnLinks**</span><span class="sxs-lookup"><span data-stu-id="3a538-149">**columnLinks**</span></span> | <span data-ttu-id="3a538-150">Conjunto [columnLink][]</span><span class="sxs-lookup"><span data-stu-id="3a538-150">[columnLink][] collection</span></span> | <span data-ttu-id="3a538-151">O conjunto de colunas necessário para este tipo de conteúdo</span><span class="sxs-lookup"><span data-stu-id="3a538-151">The collection of columns that are required by this content type</span></span>

<span data-ttu-id="3a538-152">Consulte [Introdução a tipos de conteúdo e publicação de tipo de conteúdo][contentTypeIntro] para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="3a538-152">See [Introduction to content types and content type publishing][contentTypeIntro] for more information.</span></span>

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
