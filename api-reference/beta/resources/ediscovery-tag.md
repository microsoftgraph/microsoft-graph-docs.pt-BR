---
title: tipo de recurso tag
description: Representa uma marca eDiscovery, que é usada para marcar documentos durante a revisão para separar conteúdo responsivo e não responsivo
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: dee53c5a7d8320822101addcf5764420456e703f
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445944"
---
# <a name="tag-resource-type"></a><span data-ttu-id="0584e-103">tipo de recurso tag</span><span class="sxs-lookup"><span data-stu-id="0584e-103">tag resource type</span></span>

<span data-ttu-id="0584e-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="0584e-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0584e-105">Representa uma marca eDiscovery, que é usada para marcar documentos durante a revisão para separar conteúdo responsivo e não responsivo.</span><span class="sxs-lookup"><span data-stu-id="0584e-105">Represents an eDiscovery tag, which is used to mark documents during review to separate responsive and non-responsive content.</span></span>

<span data-ttu-id="0584e-106">Herda da [entidade](../resources/entity.md).</span><span class="sxs-lookup"><span data-stu-id="0584e-106">Inherits from [entity](../resources/entity.md).</span></span>

## <a name="methods"></a><span data-ttu-id="0584e-107">Methods</span><span class="sxs-lookup"><span data-stu-id="0584e-107">Methods</span></span>

|<span data-ttu-id="0584e-108">Método</span><span class="sxs-lookup"><span data-stu-id="0584e-108">Method</span></span>|<span data-ttu-id="0584e-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="0584e-109">Return type</span></span>|<span data-ttu-id="0584e-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="0584e-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0584e-111">Listar marcas</span><span class="sxs-lookup"><span data-stu-id="0584e-111">List tags</span></span>](../api/ediscovery-case-list-tags.md)|<span data-ttu-id="0584e-112">[coleção microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md)</span><span class="sxs-lookup"><span data-stu-id="0584e-112">[microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md) collection</span></span>|<span data-ttu-id="0584e-113">Obter uma lista dos objetos **de marca** e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="0584e-113">Get a list of the **tag** objects and their properties.</span></span>|
|[<span data-ttu-id="0584e-114">Criar marca</span><span class="sxs-lookup"><span data-stu-id="0584e-114">Create tag</span></span>](../api/ediscovery-case-post-tags.md)|[<span data-ttu-id="0584e-115">microsoft.graph.ediscovery.tag</span><span class="sxs-lookup"><span data-stu-id="0584e-115">microsoft.graph.ediscovery.tag</span></span>](../resources/ediscovery-tag.md)|<span data-ttu-id="0584e-116">Crie um novo **objeto tag.**</span><span class="sxs-lookup"><span data-stu-id="0584e-116">Create a new **tag** object.</span></span>|
|[<span data-ttu-id="0584e-117">Obter marca</span><span class="sxs-lookup"><span data-stu-id="0584e-117">Get tag</span></span>](../api/ediscovery-tag-get.md)|[<span data-ttu-id="0584e-118">microsoft.graph.ediscovery.tag</span><span class="sxs-lookup"><span data-stu-id="0584e-118">microsoft.graph.ediscovery.tag</span></span>](../resources/ediscovery-tag.md)|<span data-ttu-id="0584e-119">Leia as propriedades e as relações de um **objeto tag.**</span><span class="sxs-lookup"><span data-stu-id="0584e-119">Read the properties and relationships of a **tag** object.</span></span>|
|[<span data-ttu-id="0584e-120">Marca de atualização</span><span class="sxs-lookup"><span data-stu-id="0584e-120">Update tag</span></span>](../api/ediscovery-tag-update.md)|[<span data-ttu-id="0584e-121">microsoft.graph.ediscovery.tag</span><span class="sxs-lookup"><span data-stu-id="0584e-121">microsoft.graph.ediscovery.tag</span></span>](../resources/ediscovery-tag.md)|<span data-ttu-id="0584e-122">Atualize as propriedades de um **objeto tag.**</span><span class="sxs-lookup"><span data-stu-id="0584e-122">Update the properties of a **tag** object.</span></span>|
|[<span data-ttu-id="0584e-123">Excluir marca</span><span class="sxs-lookup"><span data-stu-id="0584e-123">Delete tag</span></span>](../api/ediscovery-tag-delete.md)|<span data-ttu-id="0584e-124">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="0584e-124">None</span></span>|<span data-ttu-id="0584e-125">Exclua **um objeto tag.**</span><span class="sxs-lookup"><span data-stu-id="0584e-125">Delete a **tag** object.</span></span>|
|[<span data-ttu-id="0584e-126">asHierarchy</span><span class="sxs-lookup"><span data-stu-id="0584e-126">asHierarchy</span></span>](../api/ediscovery-tag-ashierarchy.md)|<span data-ttu-id="0584e-127">[coleção microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md)</span><span class="sxs-lookup"><span data-stu-id="0584e-127">[microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md) collection</span></span>|<span data-ttu-id="0584e-128">Lista todas as marcas, incluindo a hierarquia.</span><span class="sxs-lookup"><span data-stu-id="0584e-128">Lists all tags, including their hierarchy.</span></span>|
|[<span data-ttu-id="0584e-129">Listar childTags</span><span class="sxs-lookup"><span data-stu-id="0584e-129">List childTags</span></span>](../api/ediscovery-tag-childtags.md)|<span data-ttu-id="0584e-130">[coleção microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md)</span><span class="sxs-lookup"><span data-stu-id="0584e-130">[microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md) collection</span></span>|<span data-ttu-id="0584e-131">Obter uma lista de objetos **de marca** filho associados a uma marca.</span><span class="sxs-lookup"><span data-stu-id="0584e-131">Get a list of child **tag** objects associated with a tag.</span></span>|

## <a name="properties"></a><span data-ttu-id="0584e-132">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0584e-132">Properties</span></span>

|<span data-ttu-id="0584e-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0584e-133">Property</span></span>|<span data-ttu-id="0584e-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="0584e-134">Type</span></span>|<span data-ttu-id="0584e-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="0584e-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0584e-136">childSelectability</span><span class="sxs-lookup"><span data-stu-id="0584e-136">childSelectability</span></span>|[<span data-ttu-id="0584e-137">microsoft.graph.ediscovery.childSelectability</span><span class="sxs-lookup"><span data-stu-id="0584e-137">microsoft.graph.ediscovery.childSelectability</span></span>](../resources/ediscovery-tag.md#childselectability-values)|<span data-ttu-id="0584e-138">Indica se uma única ou várias marcas filho podem ser associadas a um documento.</span><span class="sxs-lookup"><span data-stu-id="0584e-138">Indicates whether a single or multiple child tags can be associated with a document.</span></span> <span data-ttu-id="0584e-139">Os valores possíveis são: `One` e `Many`.</span><span class="sxs-lookup"><span data-stu-id="0584e-139">Possible values are: `One`, `Many`.</span></span>  <span data-ttu-id="0584e-140">Esse valor controla se o UX apresenta as marcas como caixas de seleção ou um grupo de botões de rádio.</span><span class="sxs-lookup"><span data-stu-id="0584e-140">This value controls whether the UX presents the tags as checkboxes or a radio button group.</span></span>|
|<span data-ttu-id="0584e-141">createdBy</span><span class="sxs-lookup"><span data-stu-id="0584e-141">createdBy</span></span>|[<span data-ttu-id="0584e-142">identitySet</span><span class="sxs-lookup"><span data-stu-id="0584e-142">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="0584e-143">O usuário que criou a marca.</span><span class="sxs-lookup"><span data-stu-id="0584e-143">The user who created the tag.</span></span>|
|<span data-ttu-id="0584e-144">descrição</span><span class="sxs-lookup"><span data-stu-id="0584e-144">description</span></span>|<span data-ttu-id="0584e-145">String</span><span class="sxs-lookup"><span data-stu-id="0584e-145">String</span></span>|<span data-ttu-id="0584e-146">A descrição da marca.</span><span class="sxs-lookup"><span data-stu-id="0584e-146">The description for the tag.</span></span>|
|<span data-ttu-id="0584e-147">displayName</span><span class="sxs-lookup"><span data-stu-id="0584e-147">displayName</span></span>|<span data-ttu-id="0584e-148">String</span><span class="sxs-lookup"><span data-stu-id="0584e-148">String</span></span>|<span data-ttu-id="0584e-149">Nome de exibição da marca.</span><span class="sxs-lookup"><span data-stu-id="0584e-149">Display name of the tag.</span></span>|
|<span data-ttu-id="0584e-150">id</span><span class="sxs-lookup"><span data-stu-id="0584e-150">id</span></span>|<span data-ttu-id="0584e-151">String</span><span class="sxs-lookup"><span data-stu-id="0584e-151">String</span></span>|<span data-ttu-id="0584e-152">Identificador exclusivo da marca.</span><span class="sxs-lookup"><span data-stu-id="0584e-152">Unique identifier for the tag.</span></span>|
|<span data-ttu-id="0584e-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0584e-153">lastModifiedDateTime</span></span>|<span data-ttu-id="0584e-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0584e-154">DateTimeOffset</span></span>|<span data-ttu-id="0584e-155">A data e a hora em que a marca foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="0584e-155">The date and time the tag was last modified.</span></span>|

### <a name="childselectability-values"></a><span data-ttu-id="0584e-156">valores childSelectability</span><span class="sxs-lookup"><span data-stu-id="0584e-156">childSelectability values</span></span>

|<span data-ttu-id="0584e-157">Member</span><span class="sxs-lookup"><span data-stu-id="0584e-157">Member</span></span>|<span data-ttu-id="0584e-158">Descrição</span><span class="sxs-lookup"><span data-stu-id="0584e-158">Description</span></span>|
|:----|-----------|
|<span data-ttu-id="0584e-159">Um</span><span class="sxs-lookup"><span data-stu-id="0584e-159">One</span></span>|<span data-ttu-id="0584e-160">Somente um filho pode ser selecionado.</span><span class="sxs-lookup"><span data-stu-id="0584e-160">Only one child can be selected.</span></span> <span data-ttu-id="0584e-161">Isso corresponde a uma interface do usuário que apresenta as marcas com botões de rádio.</span><span class="sxs-lookup"><span data-stu-id="0584e-161">This corresponds to a UI that presents the tags with radio buttons.</span></span>|
|<span data-ttu-id="0584e-162">Muitos</span><span class="sxs-lookup"><span data-stu-id="0584e-162">Many</span></span>|<span data-ttu-id="0584e-163">Zero ou muitos filhos podem ser selecionados.</span><span class="sxs-lookup"><span data-stu-id="0584e-163">Zero or many children can be selected.</span></span> <span data-ttu-id="0584e-164">Isso corresponde a uma interface do usuário que apresenta as marcas com caixas de seleção.</span><span class="sxs-lookup"><span data-stu-id="0584e-164">This corresponds to a UI that presents the tags with checkboxes.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0584e-165">Relações</span><span class="sxs-lookup"><span data-stu-id="0584e-165">Relationships</span></span>

|<span data-ttu-id="0584e-166">Relação</span><span class="sxs-lookup"><span data-stu-id="0584e-166">Relationship</span></span>|<span data-ttu-id="0584e-167">Tipo</span><span class="sxs-lookup"><span data-stu-id="0584e-167">Type</span></span>|<span data-ttu-id="0584e-168">Descrição</span><span class="sxs-lookup"><span data-stu-id="0584e-168">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0584e-169">childTags</span><span class="sxs-lookup"><span data-stu-id="0584e-169">childTags</span></span>|<span data-ttu-id="0584e-170">[coleção microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md)</span><span class="sxs-lookup"><span data-stu-id="0584e-170">[microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md) collection</span></span>|<span data-ttu-id="0584e-171">Retorna as marcas que são filho de uma marca.</span><span class="sxs-lookup"><span data-stu-id="0584e-171">Returns the tags that are a child of a tag.</span></span>|
|<span data-ttu-id="0584e-172">primário</span><span class="sxs-lookup"><span data-stu-id="0584e-172">parent</span></span>|[<span data-ttu-id="0584e-173">microsoft.graph.ediscovery.tag</span><span class="sxs-lookup"><span data-stu-id="0584e-173">microsoft.graph.ediscovery.tag</span></span>](../resources/ediscovery-tag.md)|<span data-ttu-id="0584e-174">Retorna a marca pai da marca especificada.</span><span class="sxs-lookup"><span data-stu-id="0584e-174">Returns the parent tag of the specified tag.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0584e-175">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0584e-175">JSON representation</span></span>

<span data-ttu-id="0584e-176">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0584e-176">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ediscovery.tag",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.tag",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "childSelectability": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)"
}
```
