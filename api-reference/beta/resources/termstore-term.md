---
title: tipo de recurso Term
description: Define uma entidade Term em um repositório de termos.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 71c22c86d2ebbb02587a20355adb1d461479297d
ms.sourcegitcommit: 3c0fa2d13ede0fdfa66d966d4ec32cb468c3befa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/25/2020
ms.locfileid: "48273569"
---
# <a name="term-resource-type"></a><span data-ttu-id="9494f-103">tipo de recurso Term</span><span class="sxs-lookup"><span data-stu-id="9494f-103">term resource type</span></span>

<span data-ttu-id="9494f-104">Namespace: Microsoft. Graph. termos</span><span class="sxs-lookup"><span data-stu-id="9494f-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9494f-105">Representa um termo usado em um [repositório]de termos.</span><span class="sxs-lookup"><span data-stu-id="9494f-105">Represents a term used in a term [store].</span></span> <span data-ttu-id="9494f-106">Um termo pode ser usado para representar um objeto que pode ser usado como metadados para marcar o conteúdo.</span><span class="sxs-lookup"><span data-stu-id="9494f-106">A term can be used to represent an object which can then be used as a metadata to tag content.</span></span> <span data-ttu-id="9494f-107">Vários termos podem ser organizados de maneira hierárquica dentro de um [conjunto].</span><span class="sxs-lookup"><span data-stu-id="9494f-107">Multiple terms can be organized in a hierarchical manner within a [set].</span></span>

<span data-ttu-id="9494f-108">Herda de [entidade](../resources/entity.md).</span><span class="sxs-lookup"><span data-stu-id="9494f-108">Inherits from [entity](../resources/entity.md).</span></span>

## <a name="methods"></a><span data-ttu-id="9494f-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="9494f-109">Methods</span></span>
|<span data-ttu-id="9494f-110">Método</span><span class="sxs-lookup"><span data-stu-id="9494f-110">Method</span></span>|<span data-ttu-id="9494f-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="9494f-111">Return type</span></span>|<span data-ttu-id="9494f-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="9494f-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9494f-113">Listar filhos</span><span class="sxs-lookup"><span data-stu-id="9494f-113">List children</span></span>](../api/termstore-term-list-children.md)|<span data-ttu-id="9494f-114">coleção [Microsoft. Graph. termos. Term](../resources/termstore-term.md)</span><span class="sxs-lookup"><span data-stu-id="9494f-114">[microsoft.graph.termStore.term](../resources/termstore-term.md) collection</span></span>|<span data-ttu-id="9494f-115">Obter os filhos de primeiro nível de um termo em um [repositório]de termos.</span><span class="sxs-lookup"><span data-stu-id="9494f-115">Get the first level children of a term in a term [store].</span></span>|
|[<span data-ttu-id="9494f-116">Listar relações</span><span class="sxs-lookup"><span data-stu-id="9494f-116">List relations</span></span>](../api/termstore-term-list-relations.md)|<span data-ttu-id="9494f-117">coleção [Microsoft. Graph. termos. relation](../resources/termstore-relation.md)</span><span class="sxs-lookup"><span data-stu-id="9494f-117">[microsoft.graph.termStore.relation](../resources/termstore-relation.md) collection</span></span>|<span data-ttu-id="9494f-118">Obter as relações de um termo em um [repositório]de termos.</span><span class="sxs-lookup"><span data-stu-id="9494f-118">Get the relations of a term in a term [store].</span></span>|
|[<span data-ttu-id="9494f-119">Criar relação</span><span class="sxs-lookup"><span data-stu-id="9494f-119">Create relation</span></span>](../api/termstore-relation-post.md)|[<span data-ttu-id="9494f-120">Microsoft. Graph. termos. relation</span><span class="sxs-lookup"><span data-stu-id="9494f-120">microsoft.graph.termStore.relation</span></span>](../resources/termstore-relation.md)|<span data-ttu-id="9494f-121">Crie uma nova relação para um termo ou um [conjunto] em um [repositório]de termos.</span><span class="sxs-lookup"><span data-stu-id="9494f-121">Create a new relation for a term or a [set] in a term [store].</span></span>|
|[<span data-ttu-id="9494f-122">Criar termo</span><span class="sxs-lookup"><span data-stu-id="9494f-122">Create term</span></span>](../api/termstore-term-post.md)|[<span data-ttu-id="9494f-123">Microsoft. Graph. termos. Term</span><span class="sxs-lookup"><span data-stu-id="9494f-123">microsoft.graph.termStore.term</span></span>](../resources/termstore-term.md)|<span data-ttu-id="9494f-124">Criar um novo objeto Term em um [repositório]de termos.</span><span class="sxs-lookup"><span data-stu-id="9494f-124">Create a new term object in a term [store].</span></span>|
|[<span data-ttu-id="9494f-125">Obter termo</span><span class="sxs-lookup"><span data-stu-id="9494f-125">Get term</span></span>](../api/termstore-term-get.md)|[<span data-ttu-id="9494f-126">Microsoft. Graph. termos. Term</span><span class="sxs-lookup"><span data-stu-id="9494f-126">microsoft.graph.termStore.term</span></span>](../resources/termstore-term.md)|<span data-ttu-id="9494f-127">Leia as propriedades e os relacionamentos de um objeto Term em um  [repositório]de termos.</span><span class="sxs-lookup"><span data-stu-id="9494f-127">Read the properties and relationships of a term object in a term  [store].</span></span>|
|[<span data-ttu-id="9494f-128">Atualizar termo</span><span class="sxs-lookup"><span data-stu-id="9494f-128">Update term</span></span>](../api/termstore-term-update.md)|[<span data-ttu-id="9494f-129">Microsoft. Graph. termos. Term</span><span class="sxs-lookup"><span data-stu-id="9494f-129">microsoft.graph.termStore.term</span></span>](../resources/termstore-term.md)|<span data-ttu-id="9494f-130">Atualizar as propriedades de um objeto Term em um [repositório]de termos.</span><span class="sxs-lookup"><span data-stu-id="9494f-130">Update the properties of a term object in a term [store].</span></span>|
|[<span data-ttu-id="9494f-131">Excluir termo</span><span class="sxs-lookup"><span data-stu-id="9494f-131">Delete term</span></span>](../api/termstore-term-delete.md)|<span data-ttu-id="9494f-132">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9494f-132">None</span></span>|<span data-ttu-id="9494f-133">Excluir um objeto Term em um [repositório]de termos.</span><span class="sxs-lookup"><span data-stu-id="9494f-133">Delete a term object in a term [store].</span></span>|

## <a name="properties"></a><span data-ttu-id="9494f-134">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9494f-134">Properties</span></span>
|<span data-ttu-id="9494f-135">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9494f-135">Property</span></span>|<span data-ttu-id="9494f-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="9494f-136">Type</span></span>|<span data-ttu-id="9494f-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="9494f-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9494f-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9494f-138">createdDateTime</span></span>|<span data-ttu-id="9494f-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9494f-139">DateTimeOffset</span></span>|<span data-ttu-id="9494f-140">Data e hora da criação do termo.</span><span class="sxs-lookup"><span data-stu-id="9494f-140">Date and time of term creation.</span></span> <span data-ttu-id="9494f-141">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="9494f-141">Read-only</span></span>|
|<span data-ttu-id="9494f-142">descrições</span><span class="sxs-lookup"><span data-stu-id="9494f-142">descriptions</span></span>|<span data-ttu-id="9494f-143">coleção [Microsoft. Graph. termos. localizedDescription](../resources/termstore-localizeddescription.md)</span><span class="sxs-lookup"><span data-stu-id="9494f-143">[microsoft.graph.termStore.localizedDescription](../resources/termstore-localizeddescription.md) collection</span></span>|<span data-ttu-id="9494f-144">Descrição sobre o termo que é dependente do languageTag</span><span class="sxs-lookup"><span data-stu-id="9494f-144">Description about term that is dependent on the languageTag</span></span>|
|<span data-ttu-id="9494f-145">id</span><span class="sxs-lookup"><span data-stu-id="9494f-145">id</span></span>|<span data-ttu-id="9494f-146">String</span><span class="sxs-lookup"><span data-stu-id="9494f-146">String</span></span>|<span data-ttu-id="9494f-147">Identificador exclusivo do termo.</span><span class="sxs-lookup"><span data-stu-id="9494f-147">Unique identifier of term.</span></span> <span data-ttu-id="9494f-148">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="9494f-148">Read-Only</span></span>|
|<span data-ttu-id="9494f-149">Legendas</span><span class="sxs-lookup"><span data-stu-id="9494f-149">labels</span></span>|<span data-ttu-id="9494f-150">coleção [Microsoft. Graph. termos. localizedLabel](../resources/termstore-localizedlabel.md)</span><span class="sxs-lookup"><span data-stu-id="9494f-150">[microsoft.graph.termStore.localizedLabel](../resources/termstore-localizedlabel.md) collection</span></span>||<span data-ttu-id="9494f-151">Metadados de rótulo para um termo</span><span class="sxs-lookup"><span data-stu-id="9494f-151">Label metadata for a term</span></span>|
|<span data-ttu-id="9494f-152">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9494f-152">lastModifiedDateTime</span></span>|<span data-ttu-id="9494f-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9494f-153">DateTimeOffset</span></span>|<span data-ttu-id="9494f-154">Data e hora da última modificação do termo.</span><span class="sxs-lookup"><span data-stu-id="9494f-154">Last date and time of term modification.</span></span> <span data-ttu-id="9494f-155">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="9494f-155">Read-only</span></span>|
|<span data-ttu-id="9494f-156">properties</span><span class="sxs-lookup"><span data-stu-id="9494f-156">properties</span></span>|<span data-ttu-id="9494f-157">coleção [Microsoft. Graph. KeyValue](../resources/keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="9494f-157">[microsoft.graph.keyValue](../resources/keyvalue.md) collection</span></span>|<span data-ttu-id="9494f-158">Coleção de propriedades no termo</span><span class="sxs-lookup"><span data-stu-id="9494f-158">Collection of properties on the term</span></span>|

## <a name="relationships"></a><span data-ttu-id="9494f-159">Relações</span><span class="sxs-lookup"><span data-stu-id="9494f-159">Relationships</span></span>
|<span data-ttu-id="9494f-160">Relação</span><span class="sxs-lookup"><span data-stu-id="9494f-160">Relationship</span></span>|<span data-ttu-id="9494f-161">Tipo</span><span class="sxs-lookup"><span data-stu-id="9494f-161">Type</span></span>|<span data-ttu-id="9494f-162">Descrição</span><span class="sxs-lookup"><span data-stu-id="9494f-162">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9494f-163">filhos</span><span class="sxs-lookup"><span data-stu-id="9494f-163">children</span></span>|<span data-ttu-id="9494f-164">coleção [Microsoft. Graph. termos. Term](../resources/termstore-term.md)</span><span class="sxs-lookup"><span data-stu-id="9494f-164">[microsoft.graph.termStore.term](../resources/termstore-term.md) collection</span></span>|<span data-ttu-id="9494f-165">Filhos do termo atual</span><span class="sxs-lookup"><span data-stu-id="9494f-165">Children of current term</span></span>|
|<span data-ttu-id="9494f-166">Relations</span><span class="sxs-lookup"><span data-stu-id="9494f-166">relations</span></span>|<span data-ttu-id="9494f-167">coleção [Microsoft. Graph. termos. relation](../resources/termstore-relation.md)</span><span class="sxs-lookup"><span data-stu-id="9494f-167">[microsoft.graph.termStore.relation](../resources/termstore-relation.md) collection</span></span>|<span data-ttu-id="9494f-168">Para indicar quais termos estão relacionados ao termo atual como fixado ou reutilizado</span><span class="sxs-lookup"><span data-stu-id="9494f-168">To indicate which terms are related to the current term as either pinned or reused</span></span>|
|<span data-ttu-id="9494f-169">set</span><span class="sxs-lookup"><span data-stu-id="9494f-169">set</span></span>|[<span data-ttu-id="9494f-170">Microsoft. Graph. termos. Set</span><span class="sxs-lookup"><span data-stu-id="9494f-170">microsoft.graph.termStore.set</span></span>](../resources/termstore-set.md)|<span data-ttu-id="9494f-171">O [conjunto] em que o termo é criado</span><span class="sxs-lookup"><span data-stu-id="9494f-171">The [set] in which the term is created</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9494f-172">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9494f-172">JSON representation</span></span>
<span data-ttu-id="9494f-173">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9494f-173">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termStore.term",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termStore.term",
  "id": "String (identifier)",
  "labels": [
    {
      "@odata.type": "microsoft.graph.termStore.localizedLabel"
    }
  ],
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "descriptions": [
    {
      "@odata.type": "microsoft.graph.termStore.localizedDescription"
    }
  ],
  "properties": [
    {
      "@odata.type": "microsoft.graph.keyValue"
    }
  ]
}
```

[Guarde]: ../resources/termstore-store.md
[store]: ../resources/termstore-store.md
[set]: ../resources/termstore-set.md
[term]: ../resources/termstore-term.md
[group]: ../resources/termstore-group.md

<!--
{
  "type": "#page.annotation",
  "description": "Term is the entity used for tagging in termStore",
  "keywords": "term,facet,resource",
  "section": "documentation",
  "tocPath": "Terms",
  "tocBookmarks": {
    "Resources/termstore-term": "#"
  },
  "suppressions": []
}
-->


