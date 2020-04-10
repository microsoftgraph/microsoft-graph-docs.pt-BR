---
title: tipo de recurso attributeDefinition
description: Descreve um atributo de um objeto.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ac3f6e18c4775f45f6a36814ea09b16914e139d3
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/10/2020
ms.locfileid: "43218447"
---
# <a name="attributedefinition-resource-type"></a><span data-ttu-id="ef38b-103">tipo de recurso attributeDefinition</span><span class="sxs-lookup"><span data-stu-id="ef38b-103">attributeDefinition resource type</span></span>

<span data-ttu-id="ef38b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ef38b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ef38b-105">Descreve um atributo de um objeto.</span><span class="sxs-lookup"><span data-stu-id="ef38b-105">Describes an attribute of an object.</span></span>

## <a name="properties"></a><span data-ttu-id="ef38b-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ef38b-106">Properties</span></span>

| <span data-ttu-id="ef38b-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ef38b-107">Property</span></span>      | <span data-ttu-id="ef38b-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="ef38b-108">Type</span></span>      | <span data-ttu-id="ef38b-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="ef38b-109">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="ef38b-110">Core</span><span class="sxs-lookup"><span data-stu-id="ef38b-110">anchor</span></span>         |<span data-ttu-id="ef38b-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="ef38b-111">Boolean</span></span>    | <span data-ttu-id="ef38b-112">`true`Se o atributo deve ser usado como a âncora do objeto.</span><span class="sxs-lookup"><span data-stu-id="ef38b-112">`true` if the attribute should be used as the anchor for the object.</span></span> <span data-ttu-id="ef38b-113">Atributos de âncora devem ter um valor exclusivo que identifica um objeto e deve ser imutável.</span><span class="sxs-lookup"><span data-stu-id="ef38b-113">Anchor attributes must have a unique value identifying an object, and must be immutable.</span></span> <span data-ttu-id="ef38b-114">O padrão é `false`.</span><span class="sxs-lookup"><span data-stu-id="ef38b-114">Default is `false`.</span></span> <span data-ttu-id="ef38b-115">Um, e apenas um, dos atributos do objeto deve ser designado como a âncora para dar suporte à sincronização.</span><span class="sxs-lookup"><span data-stu-id="ef38b-115">One, and only one, of the object's attributes must be designated as the anchor to support synchronization.</span></span> |
|<span data-ttu-id="ef38b-116">caseExact</span><span class="sxs-lookup"><span data-stu-id="ef38b-116">caseExact</span></span>      |<span data-ttu-id="ef38b-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="ef38b-117">Boolean</span></span>    |<span data-ttu-id="ef38b-118">`true`Se o valor desse atributo deve ser tratado como diferencia maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="ef38b-118">`true` if value of this attribute should be treated as case-sensitive.</span></span> <span data-ttu-id="ef38b-119">Essa configuração afeta como o mecanismo de sincronização detecta alterações para o atributo.</span><span class="sxs-lookup"><span data-stu-id="ef38b-119">This setting affects how the synchronization engine detects changes for the attribute.</span></span>|
|<span data-ttu-id="ef38b-120">los</span><span class="sxs-lookup"><span data-stu-id="ef38b-120">metadata</span></span>       |<span data-ttu-id="ef38b-121">coleção [metadataEntry](../resources/synchronization-metadataentry.md)</span><span class="sxs-lookup"><span data-stu-id="ef38b-121">[metadataEntry](../resources/synchronization-metadataentry.md) collection</span></span>   |<span data-ttu-id="ef38b-122">Propriedades de extensão adicionais.</span><span class="sxs-lookup"><span data-stu-id="ef38b-122">Additional extension properties.</span></span> <span data-ttu-id="ef38b-123">A menos que seja mencionado explicitamente, os valores de metadados não devem ser alterados.</span><span class="sxs-lookup"><span data-stu-id="ef38b-123">Unless mentioned explicitly, metadata values should not be changed.</span></span>|
|<span data-ttu-id="ef38b-124">múltiplos valores</span><span class="sxs-lookup"><span data-stu-id="ef38b-124">multivalued</span></span>    |<span data-ttu-id="ef38b-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="ef38b-125">Boolean</span></span>    |<span data-ttu-id="ef38b-126">`true`se um atributo puder ter vários valores.</span><span class="sxs-lookup"><span data-stu-id="ef38b-126">`true` if an attribute can have multiple values.</span></span> <span data-ttu-id="ef38b-127">O padrão é `false`.</span><span class="sxs-lookup"><span data-stu-id="ef38b-127">Default is `false`.</span></span>|
|<span data-ttu-id="ef38b-128">Imutabilidade</span><span class="sxs-lookup"><span data-stu-id="ef38b-128">mutability</span></span>     |<span data-ttu-id="ef38b-129">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="ef38b-129">String</span></span>     |<span data-ttu-id="ef38b-130">Uma imutabilidade de atributo.</span><span class="sxs-lookup"><span data-stu-id="ef38b-130">An attribute's mutability.</span></span> <span data-ttu-id="ef38b-131">Os valores possíveis são `ReadWrite`: `ReadOnly`, `Immutable`, `WriteOnly`,.</span><span class="sxs-lookup"><span data-stu-id="ef38b-131">Possible values are:  `ReadWrite`, `ReadOnly`, `Immutable`, `WriteOnly`.</span></span> <span data-ttu-id="ef38b-132">O padrão é `ReadWrite`.</span><span class="sxs-lookup"><span data-stu-id="ef38b-132">Default is `ReadWrite`.</span></span>|
|<span data-ttu-id="ef38b-133">nome</span><span class="sxs-lookup"><span data-stu-id="ef38b-133">name</span></span>           |<span data-ttu-id="ef38b-134">String</span><span class="sxs-lookup"><span data-stu-id="ef38b-134">String</span></span>     |<span data-ttu-id="ef38b-135">Nome do atributo.</span><span class="sxs-lookup"><span data-stu-id="ef38b-135">Name of the attribute.</span></span> <span data-ttu-id="ef38b-136">Deve ser exclusivo dentro da definição do objeto.</span><span class="sxs-lookup"><span data-stu-id="ef38b-136">Must be unique within the object definition.</span></span> <span data-ttu-id="ef38b-137">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="ef38b-137">Not nullable.</span></span>|
|<span data-ttu-id="ef38b-138">obrigatório</span><span class="sxs-lookup"><span data-stu-id="ef38b-138">required</span></span>       |<span data-ttu-id="ef38b-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="ef38b-139">Boolean</span></span>    |<span data-ttu-id="ef38b-140">`true`Se o atributo for necessário.</span><span class="sxs-lookup"><span data-stu-id="ef38b-140">`true` if attribute is required.</span></span> <span data-ttu-id="ef38b-141">Objeto não pode ser criado se qualquer um dos atributos necessários estiver ausente.</span><span class="sxs-lookup"><span data-stu-id="ef38b-141">Object can not be created if any of the required attributes are missing.</span></span> <span data-ttu-id="ef38b-142">Se durante a sincronização, o atributo Required não tem valor, o valor padrão será usado.</span><span class="sxs-lookup"><span data-stu-id="ef38b-142">If during synchronization, the required attribute has no value, the default value will be used.</span></span> <span data-ttu-id="ef38b-143">Se o valor padrão não foi definido, a sincronização registrará um erro.</span><span class="sxs-lookup"><span data-stu-id="ef38b-143">If default the value was not set, synchronization will record an error.</span></span>|
|<span data-ttu-id="ef38b-144">referencedObjects</span><span class="sxs-lookup"><span data-stu-id="ef38b-144">referencedObjects</span></span>|<span data-ttu-id="ef38b-145">coleção [referenciable](../resources/synchronization-referencedobject.md)</span><span class="sxs-lookup"><span data-stu-id="ef38b-145">[referencedObject](../resources/synchronization-referencedobject.md) collection</span></span> |<span data-ttu-id="ef38b-146">Para atributos com `reference` tipo, lista objetos referenciados (por exemplo, `manager` o atributo seria `User` List como o objeto referenciado).</span><span class="sxs-lookup"><span data-stu-id="ef38b-146">For attributes with `reference` type, lists referenced objects (for example, the `manager` attribute would list `User` as the referenced object).</span></span>|
|<span data-ttu-id="ef38b-147">tipo</span><span class="sxs-lookup"><span data-stu-id="ef38b-147">type</span></span>           |<span data-ttu-id="ef38b-148">String</span><span class="sxs-lookup"><span data-stu-id="ef38b-148">String</span></span>     |<span data-ttu-id="ef38b-149">Tipo de valor de atributo.</span><span class="sxs-lookup"><span data-stu-id="ef38b-149">Attribute value type.</span></span> <span data-ttu-id="ef38b-150">Os valores possíveis são: `String`, `Integer`, `Reference`, `Binary`, `Boolean`.</span><span class="sxs-lookup"><span data-stu-id="ef38b-150">Possible values are: `String`, `Integer`, `Reference`, `Binary`, `Boolean`.</span></span> <span data-ttu-id="ef38b-151">O padrão é `String`.</span><span class="sxs-lookup"><span data-stu-id="ef38b-151">Default is `String`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ef38b-152">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ef38b-152">JSON representation</span></span>

<span data-ttu-id="ef38b-153">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ef38b-153">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attributeDefinition"
}-->

```json
{
  "anchor": true,
  "caseExact": true,
  "defaultValue": "String",
  "metadata": [{"@odata.type": "microsoft.graph.metadataEntry"}],
  "multivalued": true,
  "mutability": "String",
  "name": "String",
  "referencedObjects": [{"@odata.type": "microsoft.graph.referencedObject"}],
  "required": true,
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "attributeDefinition resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
