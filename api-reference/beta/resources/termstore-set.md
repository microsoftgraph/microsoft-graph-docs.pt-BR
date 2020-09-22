---
title: definir tipo de recurso
description: Representa um conjunto em um repositório de termos.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 45436f1a20652555b17b553f96db60e5636d3d92
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47988792"
---
# <a name="set-resource-type"></a><span data-ttu-id="bb6e7-103">definir tipo de recurso</span><span class="sxs-lookup"><span data-stu-id="bb6e7-103">set resource type</span></span>

<span data-ttu-id="bb6e7-104">Namespace: Microsoft. Graph. termos</span><span class="sxs-lookup"><span data-stu-id="bb6e7-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bb6e7-105">Representa o conjunto usado em um [repositório]de termos.</span><span class="sxs-lookup"><span data-stu-id="bb6e7-105">Represents the set used in a term [store].</span></span> <span data-ttu-id="bb6e7-106">O conjunto representa uma unidade que contém uma coleção de termos hierárquicos.</span><span class="sxs-lookup"><span data-stu-id="bb6e7-106">The set represents a unit which contains a collection of hierarchical terms.</span></span> <span data-ttu-id="bb6e7-107">Um [grupo] pode conter vários conjuntos.</span><span class="sxs-lookup"><span data-stu-id="bb6e7-107">A [group] can contain multiple sets.</span></span>

<span data-ttu-id="bb6e7-108">Herda de [entidade](../resources/entity.md).</span><span class="sxs-lookup"><span data-stu-id="bb6e7-108">Inherits from [entity](../resources/entity.md).</span></span>

## <a name="methods"></a><span data-ttu-id="bb6e7-109">Methods</span><span class="sxs-lookup"><span data-stu-id="bb6e7-109">Methods</span></span>
|<span data-ttu-id="bb6e7-110">Método</span><span class="sxs-lookup"><span data-stu-id="bb6e7-110">Method</span></span>|<span data-ttu-id="bb6e7-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="bb6e7-111">Return type</span></span>|<span data-ttu-id="bb6e7-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="bb6e7-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="bb6e7-113">Listar conjuntos</span><span class="sxs-lookup"><span data-stu-id="bb6e7-113">List sets</span></span>](../api/termstore-group-list-sets.md)|<span data-ttu-id="bb6e7-114">coleção [Microsoft. Graph. termos. Set]</span><span class="sxs-lookup"><span data-stu-id="bb6e7-114">collection [microsoft.graph.termStore.set]</span></span> | <span data-ttu-id="bb6e7-115">Retorna uma lista de conjuntos contidos em um [grupo] de um [repositório] de termos</span><span class="sxs-lookup"><span data-stu-id="bb6e7-115">Returns list of sets contained within a [group] of a term [store]</span></span> |
|[<span data-ttu-id="bb6e7-116">Criar conjunto</span><span class="sxs-lookup"><span data-stu-id="bb6e7-116">Create set</span></span>](../api/termstore-set-post.md)|[<span data-ttu-id="bb6e7-117">Microsoft. Graph. termos. Set</span><span class="sxs-lookup"><span data-stu-id="bb6e7-117">microsoft.graph.termStore.set</span></span>](../resources/termstore-set.md)|<span data-ttu-id="bb6e7-118">Criar um novo objeto Set em um [repositório]de termos.</span><span class="sxs-lookup"><span data-stu-id="bb6e7-118">Create a new set object in a term [store].</span></span>|
|[<span data-ttu-id="bb6e7-119">Criar termo</span><span class="sxs-lookup"><span data-stu-id="bb6e7-119">Create term</span></span>](../api/termstore-term-post.md)|[<span data-ttu-id="bb6e7-120">Microsoft. Graph. termos. Term</span><span class="sxs-lookup"><span data-stu-id="bb6e7-120">microsoft.graph.termStore.term</span></span>](../resources/termstore-term.md)|<span data-ttu-id="bb6e7-121">Criar um novo objeto [Term] em um [repositório]de termos.</span><span class="sxs-lookup"><span data-stu-id="bb6e7-121">Create a new [term] object in a term [store].</span></span>|
|[<span data-ttu-id="bb6e7-122">Obter conjunto</span><span class="sxs-lookup"><span data-stu-id="bb6e7-122">Get set</span></span>](../api/termstore-set-get.md)|[<span data-ttu-id="bb6e7-123">Microsoft. Graph. termos. Set</span><span class="sxs-lookup"><span data-stu-id="bb6e7-123">microsoft.graph.termStore.set</span></span>](../resources/termstore-set.md)| <span data-ttu-id="bb6e7-124">Obter um objeto Set em um [repositório]de termos.</span><span class="sxs-lookup"><span data-stu-id="bb6e7-124">Get a set object in a term [store].</span></span>|
|[<span data-ttu-id="bb6e7-125">Obter termo</span><span class="sxs-lookup"><span data-stu-id="bb6e7-125">Get term</span></span>](../api/termstore-term-get.md)|[<span data-ttu-id="bb6e7-126">Microsoft. Graph. termos. Term</span><span class="sxs-lookup"><span data-stu-id="bb6e7-126">microsoft.graph.termStore.term</span></span>](../resources/termstore-term.md)| <span data-ttu-id="bb6e7-127">Obter um objeto [Term] em um [repositório]de termos.</span><span class="sxs-lookup"><span data-stu-id="bb6e7-127">Get a [term] object in a term [store].</span></span>|
|[<span data-ttu-id="bb6e7-128">Conjunto de atualização</span><span class="sxs-lookup"><span data-stu-id="bb6e7-128">Update set</span></span>](../api/termstore-set-update.md)|[<span data-ttu-id="bb6e7-129">Microsoft. Graph. termos. Set</span><span class="sxs-lookup"><span data-stu-id="bb6e7-129">microsoft.graph.termStore.set</span></span>](../resources/termstore-set.md)|<span data-ttu-id="bb6e7-130">Atualizar as propriedades de um objeto Set em um [repositório]de termos.</span><span class="sxs-lookup"><span data-stu-id="bb6e7-130">Update the properties of a set object in a term [store].</span></span>|
|[<span data-ttu-id="bb6e7-131">Excluir conjunto</span><span class="sxs-lookup"><span data-stu-id="bb6e7-131">Delete set</span></span>](../api/termstore-set-delete.md)|<span data-ttu-id="bb6e7-132">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bb6e7-132">None</span></span>|<span data-ttu-id="bb6e7-133">Exclui um objeto Set em um [repositório]de termos.</span><span class="sxs-lookup"><span data-stu-id="bb6e7-133">Deletes a set object in a term [store].</span></span>|

## <a name="properties"></a><span data-ttu-id="bb6e7-134">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bb6e7-134">Properties</span></span>
|<span data-ttu-id="bb6e7-135">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bb6e7-135">Property</span></span>|<span data-ttu-id="bb6e7-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="bb6e7-136">Type</span></span>|<span data-ttu-id="bb6e7-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="bb6e7-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb6e7-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bb6e7-138">createdDateTime</span></span>|<span data-ttu-id="bb6e7-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bb6e7-139">DateTimeOffset</span></span>|<span data-ttu-id="bb6e7-140">Data e hora da criação do conjunto.</span><span class="sxs-lookup"><span data-stu-id="bb6e7-140">Date and time of set creation.</span></span> <span data-ttu-id="bb6e7-141">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bb6e7-141">Read-only.</span></span>|
|<span data-ttu-id="bb6e7-142">description</span><span class="sxs-lookup"><span data-stu-id="bb6e7-142">description</span></span>|<span data-ttu-id="bb6e7-143">String</span><span class="sxs-lookup"><span data-stu-id="bb6e7-143">String</span></span>|<span data-ttu-id="bb6e7-144">Descrição que oferece detalhes sobre o uso de termos.</span><span class="sxs-lookup"><span data-stu-id="bb6e7-144">Description giving details on the term usage.</span></span>|
|<span data-ttu-id="bb6e7-145">id</span><span class="sxs-lookup"><span data-stu-id="bb6e7-145">id</span></span>|<span data-ttu-id="bb6e7-146">String</span><span class="sxs-lookup"><span data-stu-id="bb6e7-146">String</span></span>|<span data-ttu-id="bb6e7-147">Identificador exclusivo.</span><span class="sxs-lookup"><span data-stu-id="bb6e7-147">Unique identifier.</span></span> <span data-ttu-id="bb6e7-148">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bb6e7-148">Read-only.</span></span>|
|<span data-ttu-id="bb6e7-149">localizadores</span><span class="sxs-lookup"><span data-stu-id="bb6e7-149">localizedNames</span></span>|<span data-ttu-id="bb6e7-150">coleção [Microsoft. Graph. termos.](../resources/termstore-localizedname.md) undeleble</span><span class="sxs-lookup"><span data-stu-id="bb6e7-150">[microsoft.graph.termStore.localizedName](../resources/termstore-localizedname.md) collection</span></span>|<span data-ttu-id="bb6e7-151">Nome do conjunto para cada languageTag.</span><span class="sxs-lookup"><span data-stu-id="bb6e7-151">Name of the set for each languageTag.</span></span>|
|<span data-ttu-id="bb6e7-152">properties</span><span class="sxs-lookup"><span data-stu-id="bb6e7-152">properties</span></span>|<span data-ttu-id="bb6e7-153">coleção [Microsoft. Graph. KeyValue](../resources/keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="bb6e7-153">[microsoft.graph.keyValue](../resources/keyvalue.md) collection</span></span>|<span data-ttu-id="bb6e7-154">Propriedades personalizadas para o conjunto.</span><span class="sxs-lookup"><span data-stu-id="bb6e7-154">Custom properties for the set.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bb6e7-155">Relações</span><span class="sxs-lookup"><span data-stu-id="bb6e7-155">Relationships</span></span>
|<span data-ttu-id="bb6e7-156">Relação</span><span class="sxs-lookup"><span data-stu-id="bb6e7-156">Relationship</span></span>|<span data-ttu-id="bb6e7-157">Tipo</span><span class="sxs-lookup"><span data-stu-id="bb6e7-157">Type</span></span>|<span data-ttu-id="bb6e7-158">Descrição</span><span class="sxs-lookup"><span data-stu-id="bb6e7-158">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb6e7-159">filhos</span><span class="sxs-lookup"><span data-stu-id="bb6e7-159">children</span></span>|<span data-ttu-id="bb6e7-160">coleção [Microsoft. Graph. termos. Term](../resources/termstore-term.md)</span><span class="sxs-lookup"><span data-stu-id="bb6e7-160">[microsoft.graph.termStore.term](../resources/termstore-term.md) collection</span></span>|<span data-ttu-id="bb6e7-161">Termos filhos de Set no [repositório]de termos.</span><span class="sxs-lookup"><span data-stu-id="bb6e7-161">Children terms of set in term [store].</span></span>|
|<span data-ttu-id="bb6e7-162">parentGroup</span><span class="sxs-lookup"><span data-stu-id="bb6e7-162">parentGroup</span></span>|[<span data-ttu-id="bb6e7-163">Microsoft. Graph. termos. Group</span><span class="sxs-lookup"><span data-stu-id="bb6e7-163">microsoft.graph.termStore.group</span></span>](../resources/termstore-group.md)|<span data-ttu-id="bb6e7-164">O [grupo] pai que contém o conjunto.</span><span class="sxs-lookup"><span data-stu-id="bb6e7-164">The parent [group] that contains the set.</span></span>|
|<span data-ttu-id="bb6e7-165">Relations</span><span class="sxs-lookup"><span data-stu-id="bb6e7-165">relations</span></span>|<span data-ttu-id="bb6e7-166">coleção [Microsoft. Graph. termos. relation](../resources/termstore-relation.md)</span><span class="sxs-lookup"><span data-stu-id="bb6e7-166">[microsoft.graph.termStore.relation](../resources/termstore-relation.md) collection</span></span>|<span data-ttu-id="bb6e7-167">Indica quais termos foram afixados ou reutilizados diretamente sob o conjunto.</span><span class="sxs-lookup"><span data-stu-id="bb6e7-167">Indicates which terms have been pinned or reused directly under the set.</span></span>|
|<span data-ttu-id="bb6e7-168">termos</span><span class="sxs-lookup"><span data-stu-id="bb6e7-168">terms</span></span>|<span data-ttu-id="bb6e7-169">coleção [Microsoft. Graph. termos. Term](../resources/termstore-term.md)</span><span class="sxs-lookup"><span data-stu-id="bb6e7-169">[microsoft.graph.termStore.term](../resources/termstore-term.md) collection</span></span>|<span data-ttu-id="bb6e7-170">Todos os termos do conjunto.</span><span class="sxs-lookup"><span data-stu-id="bb6e7-170">All the terms under the set.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bb6e7-171">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bb6e7-171">JSON representation</span></span>
<span data-ttu-id="bb6e7-172">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bb6e7-172">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termStore.set",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termStore.set",
  "id": "String (identifier)",
  "localizedNames": [
    {
      "@odata.type": "microsoft.graph.termStore.localizedName"
    }
  ],
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "properties": [
    {
      "@odata.type": "microsoft.graph.termStore.keyValue"
    }
  ]
}
```

[microsoft.graph.termStore.term]: termstore-term.md
[Microsoft. Graph. termos. Set]: termstore-set.md
[microsoft.graph.termStore.set]: termstore-set.md
[microsoft.graph.termStore.group]: termstore-group.md
[microsoft.graph.termStore.relation]: termstore-relation.md
[microsoft.graph.termStore.store]: termstore-store.md
[microsoft.graph.termStore.localizedName]: termstore-localizedname.md
[loja]: ../resources/termstore-store.md
[store]: ../resources/termstore-store.md
[group]: ../resources/termstore-group.md
[set]: ../resources/termstore-set.md
[terminal]: ../resources/termstore-term.md
[term]: ../resources/termstore-term.md


<!--
{
  "type": "#page.annotation",
  "description": "TermSet is the entity containing the particular taxonomy for a tenant",
  "keywords": "termSet,facet,resource",
  "section": "documentation",
  "tocPath": "TermSet",
  "tocBookmarks": {
    "Resources/termStore.set": "#"
  },
  "suppressions": []
}
-->


