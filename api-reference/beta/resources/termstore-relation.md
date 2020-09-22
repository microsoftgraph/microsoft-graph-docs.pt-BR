---
title: tipo de recurso relation
description: Representa a relação entre os termos em um repositório de termos.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 2e8f4dc8b82c496909f5b150829d9fb4e114ba59
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47973586"
---
# <a name="relation-resource-type"></a><span data-ttu-id="fdb2a-103">tipo de recurso relation</span><span class="sxs-lookup"><span data-stu-id="fdb2a-103">relation resource type</span></span>

<span data-ttu-id="fdb2a-104">Namespace: Microsoft. Graph. termos</span><span class="sxs-lookup"><span data-stu-id="fdb2a-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fdb2a-105">Representa a relação entre os [termos](../resources/termstore-term.md) em um [repositório]de termos.</span><span class="sxs-lookup"><span data-stu-id="fdb2a-105">Represents the relationship between [terms](../resources/termstore-term.md) in a term [store].</span></span> <span data-ttu-id="fdb2a-106">Atualmente, dois tipos de relações têm suporte: PIN e reutilização.</span><span class="sxs-lookup"><span data-stu-id="fdb2a-106">Currently two types of relationships are supported: pin and reuse.</span></span> 

<span data-ttu-id="fdb2a-107">Em um relacionamento de PIN, um termo pode ser fixado em um termo diferente em um conjunto de termos diferente.</span><span class="sxs-lookup"><span data-stu-id="fdb2a-107">In a pin relationship, a term can be pinned under a different term in a different term set.</span></span> <span data-ttu-id="fdb2a-108">Em uma relação fixa, só é possível adicionar novos filhos ao termo no conjunto de termos em que o termo foi criado.</span><span class="sxs-lookup"><span data-stu-id="fdb2a-108">In a pinned relationship, new children to the term can only be added in the term set in which the term was created.</span></span> <span data-ttu-id="fdb2a-109">Qualquer alteração na hierarquia sob o termo é refletida nos conjuntos em que o termo foi fixado.</span><span class="sxs-lookup"><span data-stu-id="fdb2a-109">Any change in the hierarchy under the term is reflected across the sets in which the term was pinned.</span></span> 

<span data-ttu-id="fdb2a-110">A relação de reutilização é semelhante à relação fixa, exceto que as alterações no termo reutilizado podem ser feitas de qualquer hierarquia na qual o termo é reutilizado.</span><span class="sxs-lookup"><span data-stu-id="fdb2a-110">The reuse relationship is similar to the pinned relationship except that changes to the reused term can be made from any hierarchy in which the term is reused.</span></span> <span data-ttu-id="fdb2a-111">Além disso, uma alteração na hierarquia feita no termo reutilizado não é refletida nos outros conjuntos de termos nos quais o termo é reutilizado.</span><span class="sxs-lookup"><span data-stu-id="fdb2a-111">Also, a change in hierarchy made to the reused term does not get reflected in the other term sets in which the term is reused.</span></span>

<span data-ttu-id="fdb2a-112">Herda de [entidade](../resources/entity.md).</span><span class="sxs-lookup"><span data-stu-id="fdb2a-112">Inherits from [entity](../resources/entity.md).</span></span>

## <a name="methods"></a><span data-ttu-id="fdb2a-113">Methods</span><span class="sxs-lookup"><span data-stu-id="fdb2a-113">Methods</span></span>
|<span data-ttu-id="fdb2a-114">Método</span><span class="sxs-lookup"><span data-stu-id="fdb2a-114">Method</span></span>|<span data-ttu-id="fdb2a-115">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="fdb2a-115">Return type</span></span>|<span data-ttu-id="fdb2a-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="fdb2a-116">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="fdb2a-117">Listar relações</span><span class="sxs-lookup"><span data-stu-id="fdb2a-117">List relations</span></span>](../api/termstore-term-list-relations.md)|<span data-ttu-id="fdb2a-118">coleção [Microsoft. Graph. termos. relation](../resources/termstore-relation.md)</span><span class="sxs-lookup"><span data-stu-id="fdb2a-118">[microsoft.graph.termstore.relation](../resources/termstore-relation.md) collection</span></span>|<span data-ttu-id="fdb2a-119">Recupere uma lista de objetos **relation** .</span><span class="sxs-lookup"><span data-stu-id="fdb2a-119">Retrieve a list of **relation** objects.</span></span>|
|[<span data-ttu-id="fdb2a-120">Criar relação</span><span class="sxs-lookup"><span data-stu-id="fdb2a-120">Create relation</span></span>](../api/termstore-relation-post.md)|[<span data-ttu-id="fdb2a-121">Microsoft. Graph. termos. relation</span><span class="sxs-lookup"><span data-stu-id="fdb2a-121">microsoft.graph.termstore.relation</span></span>](../resources/termstore-relation.md)|<span data-ttu-id="fdb2a-122">Criar um novo objeto **relation** .</span><span class="sxs-lookup"><span data-stu-id="fdb2a-122">Create a new **relation** object.</span></span>|


## <a name="properties"></a><span data-ttu-id="fdb2a-123">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fdb2a-123">Properties</span></span>
|<span data-ttu-id="fdb2a-124">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fdb2a-124">Property</span></span>|<span data-ttu-id="fdb2a-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="fdb2a-125">Type</span></span>|<span data-ttu-id="fdb2a-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="fdb2a-126">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fdb2a-127">id</span><span class="sxs-lookup"><span data-stu-id="fdb2a-127">id</span></span>|<span data-ttu-id="fdb2a-128">String</span><span class="sxs-lookup"><span data-stu-id="fdb2a-128">String</span></span>|<span data-ttu-id="fdb2a-129">A ID da relação.</span><span class="sxs-lookup"><span data-stu-id="fdb2a-129">The ID of the relation.</span></span>|
|<span data-ttu-id="fdb2a-130">relação</span><span class="sxs-lookup"><span data-stu-id="fdb2a-130">relationship</span></span>|<span data-ttu-id="fdb2a-131">String</span><span class="sxs-lookup"><span data-stu-id="fdb2a-131">String</span></span>|<span data-ttu-id="fdb2a-132">O tipo de relação.</span><span class="sxs-lookup"><span data-stu-id="fdb2a-132">The type of relation.</span></span> <span data-ttu-id="fdb2a-133">Os valores possíveis são: `pin`, `reuse`.</span><span class="sxs-lookup"><span data-stu-id="fdb2a-133">Possible values are: `pin`, `reuse`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fdb2a-134">Relações</span><span class="sxs-lookup"><span data-stu-id="fdb2a-134">Relationships</span></span>
|<span data-ttu-id="fdb2a-135">Relação</span><span class="sxs-lookup"><span data-stu-id="fdb2a-135">Relationship</span></span>|<span data-ttu-id="fdb2a-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="fdb2a-136">Type</span></span>|<span data-ttu-id="fdb2a-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="fdb2a-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fdb2a-138">fromTerm</span><span class="sxs-lookup"><span data-stu-id="fdb2a-138">fromTerm</span></span>|[<span data-ttu-id="fdb2a-139">Microsoft. Graph. termos. Term</span><span class="sxs-lookup"><span data-stu-id="fdb2a-139">microsoft.graph.termStore.term</span></span>](../resources/termstore-term.md)|<span data-ttu-id="fdb2a-140">O [termo] de da relação.</span><span class="sxs-lookup"><span data-stu-id="fdb2a-140">The from [term] of the relation.</span></span> <span data-ttu-id="fdb2a-141">O termo a partir do qual a relação é definida.</span><span class="sxs-lookup"><span data-stu-id="fdb2a-141">The term from which the relationship is defined.</span></span> <span data-ttu-id="fdb2a-142">Um valor nulo indicaria que a relação é diretamente com o [conjunto].</span><span class="sxs-lookup"><span data-stu-id="fdb2a-142">A null value would indicate the relation is directly with the [set].</span></span> |
|<span data-ttu-id="fdb2a-143">set</span><span class="sxs-lookup"><span data-stu-id="fdb2a-143">set</span></span>|[<span data-ttu-id="fdb2a-144">Microsoft. Graph. termos. Set</span><span class="sxs-lookup"><span data-stu-id="fdb2a-144">microsoft.graph.termStore.set</span></span>](../resources/termstore-set.md)|<span data-ttu-id="fdb2a-145">O [conjunto] em que a relação é relevante.</span><span class="sxs-lookup"><span data-stu-id="fdb2a-145">The [set] in which the relation is relevant.</span></span>|
|<span data-ttu-id="fdb2a-146">toterm</span><span class="sxs-lookup"><span data-stu-id="fdb2a-146">toTerm</span></span>|[<span data-ttu-id="fdb2a-147">Microsoft. Graph. termos. Term</span><span class="sxs-lookup"><span data-stu-id="fdb2a-147">microsoft.graph.termStore.term</span></span>](../resources/termstore-term.md)|<span data-ttu-id="fdb2a-148">O [termo] to da relação.</span><span class="sxs-lookup"><span data-stu-id="fdb2a-148">The to [term] of the relation.</span></span> <span data-ttu-id="fdb2a-149">O termo para o qual o realtionship está definido.</span><span class="sxs-lookup"><span data-stu-id="fdb2a-149">The term to which the realtionship is defined.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fdb2a-150">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fdb2a-150">JSON representation</span></span>
<span data-ttu-id="fdb2a-151">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fdb2a-151">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termStore.relation",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termStore.relation",
  "id": "String (identifier)",
  "relationship": "String"
}
```

[microsoft.graph.termStore.term]: termstore-term.md
[microsoft.graph.termStore.set]: termstore-set.md
[microsoft.graph.termStore.relations]: termstore-relation.md
[microsoft.graph.termStore.relation]: termstore-relation.md
[loja]: ../resources/termstore-store.md
[store]: ../resources/termstore-store.md
[terminal]: ../resources/termstore-term.md
[term]: ../resources/termstore-term.md
[set]: ../resources/termstore-set.md

<!--
{
  "type": "#page.annotation",
  "description": "TermRelation is the entity for mapping relations between different terms",
  "keywords": "termRelation,facet,resource",
  "section": "documentation",
  "tocPath": "TermRelation",
  "tocBookmarks": {
    "Resources/termStore.relation": "#"
  },
  "suppressions": []
}
-->


