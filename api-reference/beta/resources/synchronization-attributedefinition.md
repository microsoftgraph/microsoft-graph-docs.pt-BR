---
title: tipo de recurso attributeDefinition
description: Descreve um atributo de um objeto.
localization_priority: Normal
ms.openlocfilehash: 04ee5ffb6cda3cc48f89a722caab3a4e46500379
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345619"
---
# <a name="attributedefinition-resource-type"></a><span data-ttu-id="037d8-103">tipo de recurso attributeDefinition</span><span class="sxs-lookup"><span data-stu-id="037d8-103">attributeDefinition resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="037d8-104">Descreve um atributo de um objeto.</span><span class="sxs-lookup"><span data-stu-id="037d8-104">Describes an attribute of an object.</span></span>

## <a name="properties"></a><span data-ttu-id="037d8-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="037d8-105">Properties</span></span>

| <span data-ttu-id="037d8-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="037d8-106">Property</span></span>      | <span data-ttu-id="037d8-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="037d8-107">Type</span></span>      | <span data-ttu-id="037d8-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="037d8-108">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="037d8-109">Core</span><span class="sxs-lookup"><span data-stu-id="037d8-109">anchor</span></span>         |<span data-ttu-id="037d8-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="037d8-110">Boolean</span></span>    | <span data-ttu-id="037d8-111">`true`Se o atributo deve ser usado como a âncora do objeto.</span><span class="sxs-lookup"><span data-stu-id="037d8-111">`true` if the attribute should be used as the anchor for the object.</span></span> <span data-ttu-id="037d8-112">Atributos de âncora devem ter um valor exclusivo que identifica um objeto e deve ser imutável.</span><span class="sxs-lookup"><span data-stu-id="037d8-112">Anchor attributes must have a unique value identifying an object, and must be immutable.</span></span> <span data-ttu-id="037d8-113">O padrão é `false`.</span><span class="sxs-lookup"><span data-stu-id="037d8-113">Default is `false`.</span></span> <span data-ttu-id="037d8-114">Um, e apenas um, dos atributos do objeto deve ser designado como a âncora para dar suporte à sincronização.</span><span class="sxs-lookup"><span data-stu-id="037d8-114">One, and only one, of the object's attributes must be designated as the anchor to support synchronization.</span></span> |
|<span data-ttu-id="037d8-115">caseExact</span><span class="sxs-lookup"><span data-stu-id="037d8-115">caseExact</span></span>      |<span data-ttu-id="037d8-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="037d8-116">Boolean</span></span>    |<span data-ttu-id="037d8-117">`true`Se o valor desse atributo deve ser tratado como diferencia maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="037d8-117">`true` if value of this attribute should be treated as case-sensitive.</span></span> <span data-ttu-id="037d8-118">Essa configuração afeta como o mecanismo de sincronização detecta alterações para o atributo.</span><span class="sxs-lookup"><span data-stu-id="037d8-118">This setting affects how the synchronization engine detects changes for the attribute.</span></span>|
|<span data-ttu-id="037d8-119">los</span><span class="sxs-lookup"><span data-stu-id="037d8-119">metadata</span></span>       |<span data-ttu-id="037d8-120">coleção [metadataEntry](../resources/synchronization-metadataentry.md)</span><span class="sxs-lookup"><span data-stu-id="037d8-120">[metadataEntry](../resources/synchronization-metadataentry.md) collection</span></span>   |<span data-ttu-id="037d8-121">Propriedades de extensão adicionais.</span><span class="sxs-lookup"><span data-stu-id="037d8-121">Additional extension properties.</span></span> <span data-ttu-id="037d8-122">A menos que seja mencionado explicitamente, os valores de metadados não devem ser alterados.</span><span class="sxs-lookup"><span data-stu-id="037d8-122">Unless mentioned explicitly, metadata values should not be changed.</span></span>|
|<span data-ttu-id="037d8-123">múltiplos valores</span><span class="sxs-lookup"><span data-stu-id="037d8-123">multivalued</span></span>    |<span data-ttu-id="037d8-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="037d8-124">Boolean</span></span>    |<span data-ttu-id="037d8-125">`true`se um atributo puder ter vários valores.</span><span class="sxs-lookup"><span data-stu-id="037d8-125">`true` if an attribute can have multiple values.</span></span> <span data-ttu-id="037d8-126">O padrão é `false`.</span><span class="sxs-lookup"><span data-stu-id="037d8-126">Default is `false`.</span></span>|
|<span data-ttu-id="037d8-127">Imutabilidade</span><span class="sxs-lookup"><span data-stu-id="037d8-127">mutability</span></span>     |<span data-ttu-id="037d8-128">String</span><span class="sxs-lookup"><span data-stu-id="037d8-128">String</span></span>     |<span data-ttu-id="037d8-129">Uma imutabilidade de atributo.</span><span class="sxs-lookup"><span data-stu-id="037d8-129">An attribute's mutability.</span></span> <span data-ttu-id="037d8-130">Os valores possíveis são `ReadWrite`: `ReadOnly`, `Immutable`, `WriteOnly`,.</span><span class="sxs-lookup"><span data-stu-id="037d8-130">Possible values are:  `ReadWrite`, `ReadOnly`, `Immutable`, `WriteOnly`.</span></span> <span data-ttu-id="037d8-131">O padrão é `ReadWrite`.</span><span class="sxs-lookup"><span data-stu-id="037d8-131">Default is `ReadWrite`.</span></span>|
|<span data-ttu-id="037d8-132">name</span><span class="sxs-lookup"><span data-stu-id="037d8-132">name</span></span>           |<span data-ttu-id="037d8-133">String</span><span class="sxs-lookup"><span data-stu-id="037d8-133">String</span></span>     |<span data-ttu-id="037d8-134">Nome do atributo.</span><span class="sxs-lookup"><span data-stu-id="037d8-134">Name of the attribute.</span></span> <span data-ttu-id="037d8-135">Deve ser exclusivo dentro da definição do objeto.</span><span class="sxs-lookup"><span data-stu-id="037d8-135">Must be unique within the object definition.</span></span> <span data-ttu-id="037d8-136">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="037d8-136">Not nullable.</span></span>|
|<span data-ttu-id="037d8-137">obrigatório</span><span class="sxs-lookup"><span data-stu-id="037d8-137">required</span></span>       |<span data-ttu-id="037d8-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="037d8-138">Boolean</span></span>    |<span data-ttu-id="037d8-139">`true`Se o atributo for necessário.</span><span class="sxs-lookup"><span data-stu-id="037d8-139">`true` if attribute is required.</span></span> <span data-ttu-id="037d8-140">Objeto não pode ser criado se qualquer um dos atributos necessários estiver ausente.</span><span class="sxs-lookup"><span data-stu-id="037d8-140">Object can not be created if any of the required attributes are missing.</span></span> <span data-ttu-id="037d8-141">Se durante a sincronização, o atributo Required não tem valor, o valor padrão será usado.</span><span class="sxs-lookup"><span data-stu-id="037d8-141">If during synchronization, the required attribute has no value, the default value will be used.</span></span> <span data-ttu-id="037d8-142">Se o valor padrão não foi definido, a sincronização registrará um erro.</span><span class="sxs-lookup"><span data-stu-id="037d8-142">If default the value was not set, synchronization will record an error.</span></span>|
|<span data-ttu-id="037d8-143">referencedObjects</span><span class="sxs-lookup"><span data-stu-id="037d8-143">referencedObjects</span></span>|<span data-ttu-id="037d8-144">[](../resources/synchronization-referencedobject.md) coleção referenciable</span><span class="sxs-lookup"><span data-stu-id="037d8-144">[referencedObject](../resources/synchronization-referencedobject.md) collection</span></span> |<span data-ttu-id="037d8-145">Para atributos com `reference` tipo, lista objetos referenciados (por exemplo, `manager` o atributo seria `User` List como o objeto referenciado).</span><span class="sxs-lookup"><span data-stu-id="037d8-145">For attributes with `reference` type, lists referenced objects (for example, the `manager` attribute would list `User` as the referenced object).</span></span>|
|<span data-ttu-id="037d8-146">tipo</span><span class="sxs-lookup"><span data-stu-id="037d8-146">type</span></span>           |<span data-ttu-id="037d8-147">String</span><span class="sxs-lookup"><span data-stu-id="037d8-147">String</span></span>     |<span data-ttu-id="037d8-148">Tipo de valor de atributo.</span><span class="sxs-lookup"><span data-stu-id="037d8-148">Attribute value type.</span></span> <span data-ttu-id="037d8-149">Os valores possíveis são: `String`, `Integer`, `Reference`, `Binary`, `Boolean`.</span><span class="sxs-lookup"><span data-stu-id="037d8-149">Possible values are: `String`, `Integer`, `Reference`, `Binary`, `Boolean`.</span></span> <span data-ttu-id="037d8-150">O padrão é `String`.</span><span class="sxs-lookup"><span data-stu-id="037d8-150">Default is `String`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="037d8-151">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="037d8-151">JSON representation</span></span>

<span data-ttu-id="037d8-152">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="037d8-152">The following is a JSON representation of the resource.</span></span>

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
