---
author: daspek
description: O recurso contentType representa um tipo de conteúdo no SharePoint.
title: contentType
localization_priority: Normal
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: 2af8291f33f62517e33349fb66408131f576e89a
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50444291"
---
# <a name="contenttype-resource-type"></a><span data-ttu-id="7b2fe-103">Tipo de recurso contentType</span><span class="sxs-lookup"><span data-stu-id="7b2fe-103">contentType resource type</span></span>

<span data-ttu-id="7b2fe-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7b2fe-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7b2fe-105">Representa um _tipo de conteúdo_ no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="7b2fe-105">Represents a _content type_ in SharePoint.</span></span>
<span data-ttu-id="7b2fe-106">Os tipos de conteúdo permitem definir um conjunto de colunas que devem estar presentes em cada [**listItem**][listItem] em uma [**lista**][list].</span><span class="sxs-lookup"><span data-stu-id="7b2fe-106">Content types allow you to define a set of columns that must be present on every [**listItem**][listItem] in a [**list**][list].</span></span>

## <a name="properties"></a><span data-ttu-id="7b2fe-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7b2fe-107">Properties</span></span>

| <span data-ttu-id="7b2fe-108">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="7b2fe-108">Property name</span></span>     | <span data-ttu-id="7b2fe-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="7b2fe-109">Type</span></span>                 | <span data-ttu-id="7b2fe-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="7b2fe-110">Description</span></span>
|:------------------|:---------------------|:----------------------------------
| <span data-ttu-id="7b2fe-111">**description**</span><span class="sxs-lookup"><span data-stu-id="7b2fe-111">**description**</span></span>   | <span data-ttu-id="7b2fe-112">string</span><span class="sxs-lookup"><span data-stu-id="7b2fe-112">string</span></span>               | <span data-ttu-id="7b2fe-113">O texto descritivo do item.</span><span class="sxs-lookup"><span data-stu-id="7b2fe-113">The descriptive text for the item.</span></span>
| <span data-ttu-id="7b2fe-114">**group**</span><span class="sxs-lookup"><span data-stu-id="7b2fe-114">**group**</span></span>         | <span data-ttu-id="7b2fe-115">string</span><span class="sxs-lookup"><span data-stu-id="7b2fe-115">string</span></span>               | <span data-ttu-id="7b2fe-116">O nome do grupo ao qual esse tipo de conteúdo pertence.</span><span class="sxs-lookup"><span data-stu-id="7b2fe-116">The name of the group this content type belongs to.</span></span> <span data-ttu-id="7b2fe-117">Ajuda a organizar os tipos de conteúdo relacionados.</span><span class="sxs-lookup"><span data-stu-id="7b2fe-117">Helps organize related content types.</span></span>
| <span data-ttu-id="7b2fe-118">**hidden**</span><span class="sxs-lookup"><span data-stu-id="7b2fe-118">**hidden**</span></span>        | <span data-ttu-id="7b2fe-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="7b2fe-119">Boolean</span></span>              | <span data-ttu-id="7b2fe-120">Indica se o tipo de conteúdo está oculto no menu “Novo” da lista.</span><span class="sxs-lookup"><span data-stu-id="7b2fe-120">Indicates whether the content type is hidden in the list's 'New' menu.</span></span>
| <span data-ttu-id="7b2fe-121">**id**</span><span class="sxs-lookup"><span data-stu-id="7b2fe-121">**id**</span></span>            | <span data-ttu-id="7b2fe-122">string</span><span class="sxs-lookup"><span data-stu-id="7b2fe-122">string</span></span>               | <span data-ttu-id="7b2fe-123">O identificador exclusivo do tipo de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="7b2fe-123">The unique identifier of the content type.</span></span>
| <span data-ttu-id="7b2fe-124">**inheritedFrom**</span><span class="sxs-lookup"><span data-stu-id="7b2fe-124">**inheritedFrom**</span></span> | <span data-ttu-id="7b2fe-125">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="7b2fe-125">[itemReference][]</span></span>    | <span data-ttu-id="7b2fe-126">Se esse tipo de conteúdo for herdado de outro escopo (como um site), fornece uma referência para o item no qual o tipo de conteúdo foi definido.</span><span class="sxs-lookup"><span data-stu-id="7b2fe-126">If this content type is inherited from another scope (like a site), provides a reference to the item where the content type is defined.</span></span>
| <span data-ttu-id="7b2fe-127">**name**</span><span class="sxs-lookup"><span data-stu-id="7b2fe-127">**name**</span></span>          | <span data-ttu-id="7b2fe-128">string</span><span class="sxs-lookup"><span data-stu-id="7b2fe-128">string</span></span>               | <span data-ttu-id="7b2fe-129">O nome do tipo de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="7b2fe-129">The name of the content type.</span></span>
| <span data-ttu-id="7b2fe-130">**order**</span><span class="sxs-lookup"><span data-stu-id="7b2fe-130">**order**</span></span>         | <span data-ttu-id="7b2fe-131">[contentTypeOrder][]</span><span class="sxs-lookup"><span data-stu-id="7b2fe-131">[contentTypeOrder][]</span></span> | <span data-ttu-id="7b2fe-132">Especifica a ordem na qual o tipo de conteúdo aparece na seleção da interface do usuário.</span><span class="sxs-lookup"><span data-stu-id="7b2fe-132">Specifies the order in which the content type appears in the selection UI.</span></span>
| <span data-ttu-id="7b2fe-133">**parentId**</span><span class="sxs-lookup"><span data-stu-id="7b2fe-133">**parentId**</span></span>      | <span data-ttu-id="7b2fe-134">string</span><span class="sxs-lookup"><span data-stu-id="7b2fe-134">string</span></span>               | <span data-ttu-id="7b2fe-135">O identificador exclusivo do tipo de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="7b2fe-135">The unique identifier of the content type.</span></span>
| <span data-ttu-id="7b2fe-136">**readOnly**</span><span class="sxs-lookup"><span data-stu-id="7b2fe-136">**readOnly**</span></span>      | <span data-ttu-id="7b2fe-137">Booliano</span><span class="sxs-lookup"><span data-stu-id="7b2fe-137">Boolean</span></span>              | <span data-ttu-id="7b2fe-138">Se `true`, o tipo de conteúdo não pode ser modificado, a menos que esse valor seja definido primeiro como `false`.</span><span class="sxs-lookup"><span data-stu-id="7b2fe-138">If `true`, the content type cannot be modified unless this value is first set to `false`.</span></span>
| <span data-ttu-id="7b2fe-139">**sealed**</span><span class="sxs-lookup"><span data-stu-id="7b2fe-139">**sealed**</span></span>        | <span data-ttu-id="7b2fe-140">Booliano</span><span class="sxs-lookup"><span data-stu-id="7b2fe-140">Boolean</span></span>              | <span data-ttu-id="7b2fe-141">Se `true`, o tipo de conteúdo não pode ser modificado por usuários ou por operações de push-down.</span><span class="sxs-lookup"><span data-stu-id="7b2fe-141">If `true`, the content type cannot be modified by users or through push-down operations.</span></span> <span data-ttu-id="7b2fe-142">Somente administradores de conjunto de sites podem lacrar ou retirar o lacre dos tipos de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="7b2fe-142">Only site collection administrators can seal or unseal content types.</span></span>
| <span data-ttu-id="7b2fe-143">**isBuiltIn**</span><span class="sxs-lookup"><span data-stu-id="7b2fe-143">**isBuiltIn**</span></span>            | <span data-ttu-id="7b2fe-144">Booliano</span><span class="sxs-lookup"><span data-stu-id="7b2fe-144">Boolean</span></span>| <span data-ttu-id="7b2fe-145">Especifica se um tipo de conteúdo é um tipo de conteúdo integrado.</span><span class="sxs-lookup"><span data-stu-id="7b2fe-145">Specifies if a content type is a built-in content type.</span></span> 
| <span data-ttu-id="7b2fe-146">**documentSet**</span><span class="sxs-lookup"><span data-stu-id="7b2fe-146">**documentSet**</span></span>       | <span data-ttu-id="7b2fe-147">[documentSet][]</span><span class="sxs-lookup"><span data-stu-id="7b2fe-147">[documentSet][]</span></span>      | <span data-ttu-id="7b2fe-148">[Metadados do Conjunto](https://docs.microsoft.com/sharepoint/governance/document-set-planning#about-document-sets) de Documentos.</span><span class="sxs-lookup"><span data-stu-id="7b2fe-148">[Document Set](https://docs.microsoft.com/sharepoint/governance/document-set-planning#about-document-sets) metadata.</span></span>
| <span data-ttu-id="7b2fe-149">**documentTemplate**</span><span class="sxs-lookup"><span data-stu-id="7b2fe-149">**documentTemplate**</span></span>  | <span data-ttu-id="7b2fe-150">[documentSetContent][]</span><span class="sxs-lookup"><span data-stu-id="7b2fe-150">[documentSetContent][]</span></span> | <span data-ttu-id="7b2fe-151">Metadados do modelo de documento.</span><span class="sxs-lookup"><span data-stu-id="7b2fe-151">Document template metadata.</span></span> <span data-ttu-id="7b2fe-152">Para garantir que os documentos tenham conteúdo consistente em um site e seus subsites, você pode associar um modelo do Word, Excel ou PowerPoint a um tipo de conteúdo de site.</span><span class="sxs-lookup"><span data-stu-id="7b2fe-152">To make sure that documents have consistent content across a site and its subsites, you can associate a Word, Excel, or PowerPoint template with a site content type.</span></span>
| <span data-ttu-id="7b2fe-153">**associatedHubsUrls**</span><span class="sxs-lookup"><span data-stu-id="7b2fe-153">**associatedHubsUrls**</span></span>       | <span data-ttu-id="7b2fe-154">Collection(string)</span><span class="sxs-lookup"><span data-stu-id="7b2fe-154">Collection(string)</span></span> | <span data-ttu-id="7b2fe-155">Lista de URLs canônicas para sites de hub aos quais esse tipo de conteúdo está associado.</span><span class="sxs-lookup"><span data-stu-id="7b2fe-155">List of canonical URLs for hub sites with which this content type is associated to.</span></span> <span data-ttu-id="7b2fe-156">Isso conterá todos os hubsites em que esse tipo de conteúdo está na fila para ser imposto ou já está imposto.</span><span class="sxs-lookup"><span data-stu-id="7b2fe-156">This will contain all hubsites where this content type is queued to be enforced or is already enforced.</span></span> <span data-ttu-id="7b2fe-157">Impor um tipo de conteúdo significa que o tipo de conteúdo será aplicado às listas nos sites imposto.</span><span class="sxs-lookup"><span data-stu-id="7b2fe-157">Enforcing a content type means that the content type will be applied to the lists in the enforced sites.</span></span>
| <span data-ttu-id="7b2fe-158">**propagateChanges**</span><span class="sxs-lookup"><span data-stu-id="7b2fe-158">**propagateChanges**</span></span>   | <span data-ttu-id="7b2fe-159">Booliano</span><span class="sxs-lookup"><span data-stu-id="7b2fe-159">Boolean</span></span>              | <span data-ttu-id="7b2fe-160">If `true` , any changes made to the content type will be pushed to inherited content types and lists that implement the content type.</span><span class="sxs-lookup"><span data-stu-id="7b2fe-160">If `true`, any changes made to the content type will be pushed to inherited content types and lists that implement the content type.</span></span>



## <a name="relationships"></a><span data-ttu-id="7b2fe-161">Relações</span><span class="sxs-lookup"><span data-stu-id="7b2fe-161">Relationships</span></span>

| <span data-ttu-id="7b2fe-162">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="7b2fe-162">Property name</span></span>   | <span data-ttu-id="7b2fe-163">Tipo</span><span class="sxs-lookup"><span data-stu-id="7b2fe-163">Type</span></span>                      | <span data-ttu-id="7b2fe-164">Descrição</span><span class="sxs-lookup"><span data-stu-id="7b2fe-164">Description</span></span>
|:----------------|:--------------------------|:-------------------------------
| <span data-ttu-id="7b2fe-165">**base**</span><span class="sxs-lookup"><span data-stu-id="7b2fe-165">**base**</span></span>   | <span data-ttu-id="7b2fe-166">[contentType][]</span><span class="sxs-lookup"><span data-stu-id="7b2fe-166">[contentType][]</span></span>  | <span data-ttu-id="7b2fe-167">ContentType pai do qual esse tipo de conteúdo é derivado.</span><span class="sxs-lookup"><span data-stu-id="7b2fe-167">Parent contentType from which this content type is derived.</span></span> 
| <span data-ttu-id="7b2fe-168">**columnLinks**</span><span class="sxs-lookup"><span data-stu-id="7b2fe-168">**columnLinks**</span></span> | <span data-ttu-id="7b2fe-169">Conjunto [columnLink][]</span><span class="sxs-lookup"><span data-stu-id="7b2fe-169">[columnLink][] collection</span></span> | <span data-ttu-id="7b2fe-170">O conjunto de colunas necessário para este tipo de conteúdo</span><span class="sxs-lookup"><span data-stu-id="7b2fe-170">The collection of columns that are required by this content type</span></span>
| <span data-ttu-id="7b2fe-171">**baseTypes**</span><span class="sxs-lookup"><span data-stu-id="7b2fe-171">**baseTypes**</span></span>   | <span data-ttu-id="7b2fe-172">Collection([contentType][])</span><span class="sxs-lookup"><span data-stu-id="7b2fe-172">Collection([contentType][])</span></span>     | <span data-ttu-id="7b2fe-173">A coleção de tipos de conteúdo que são ancestrais desse tipo de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="7b2fe-173">The collection of content types that are ancestors of this content type.</span></span>
| <span data-ttu-id="7b2fe-174">**columnPositions**</span><span class="sxs-lookup"><span data-stu-id="7b2fe-174">**columnPositions**</span></span>       | <span data-ttu-id="7b2fe-175">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="7b2fe-175">Collection([columnDefinition][])</span></span> | <span data-ttu-id="7b2fe-176">Informações de ordem de coluna em um tipo de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="7b2fe-176">Column order information in a content type.</span></span>
| <span data-ttu-id="7b2fe-177">**columns**</span><span class="sxs-lookup"><span data-stu-id="7b2fe-177">**columns**</span></span>     | <span data-ttu-id="7b2fe-178">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="7b2fe-178">Collection([columnDefinition][])</span></span>  | <span data-ttu-id="7b2fe-179">A coleção de definições de coluna para este contentType.</span><span class="sxs-lookup"><span data-stu-id="7b2fe-179">The collection of column definitions for this contentType.</span></span>

<span data-ttu-id="7b2fe-180">Consulte [Introdução a tipos de conteúdo e publicação de tipo de conteúdo][contentTypeIntro] para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="7b2fe-180">See [Introduction to content types and content type publishing][contentTypeIntro] for more information.</span></span>

[columnLink]: columnlink.md
[contentTypeIntro]: https://support.office.com/en-us/article/Introduction-to-content-types-and-content-type-publishing-e1277a2e-a1e8-4473-9126-91a0647766e5
[itemReference]: itemreference.md
[contentTypeOrder]: contenttypeorder.md
[columnDefinition]: columnDefinition.md
[contentType]: contentType.md
[documentSet]: documentSet.md
[documentSetContent]: documentSetContent.md

## <a name="json-representation"></a><span data-ttu-id="7b2fe-188">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7b2fe-188">JSON representation</span></span>

<span data-ttu-id="7b2fe-189">A seguir está uma representação JSON de um **recurso contentType.**</span><span class="sxs-lookup"><span data-stu-id="7b2fe-189">The following is a JSON representation of a **contentType** resource.</span></span>

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
  "columnLinks": [{ "@type": "microsoft.graph.columnLink" }],
  "base": { "@type": "microsoft.graph.contentType" },
  "columnPositions" : [{ "@type": "microsoft.graph.columnDefinition" }],
  "isBuiltIn" : false,
  "documentSet" : { "@type": "microsoft.graph.documentSet" },
  "documentTemplate" : { "@type": "microsoft.graph.documentSetContent" },
  "associatedHubsUrls" : ["string"],
  "propagateChanges" : false,
  "baseTypes" : [{ "@type": "microsoft.graph.contentType" }],
  "columns" : [{ "@type": "microsoft.graph.columnDefinition" }]
}
```

[list]: list.md
[listItem]: listitem.md
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


