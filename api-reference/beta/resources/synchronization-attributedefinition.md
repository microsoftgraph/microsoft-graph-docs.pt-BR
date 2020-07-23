---
title: tipo de recurso attributeDefinition
description: Descreve um atributo de um objeto.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a82fb5dcfd14f8c8fb09713a3a60c0f8c1e1f917
ms.sourcegitcommit: fec7d5002dbeb8d58587c89f1b678d4a54645422
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/23/2020
ms.locfileid: "45384385"
---
# <a name="attributedefinition-resource-type"></a><span data-ttu-id="90048-103">tipo de recurso attributeDefinition</span><span class="sxs-lookup"><span data-stu-id="90048-103">attributeDefinition resource type</span></span>

<span data-ttu-id="90048-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="90048-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="90048-105">Descreve um atributo de um objeto.</span><span class="sxs-lookup"><span data-stu-id="90048-105">Describes an attribute of an object.</span></span>

## <a name="properties"></a><span data-ttu-id="90048-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="90048-106">Properties</span></span>

| <span data-ttu-id="90048-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="90048-107">Property</span></span>      | <span data-ttu-id="90048-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="90048-108">Type</span></span>      | <span data-ttu-id="90048-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="90048-109">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="90048-110">Core</span><span class="sxs-lookup"><span data-stu-id="90048-110">anchor</span></span>         |<span data-ttu-id="90048-111">Booliano</span><span class="sxs-lookup"><span data-stu-id="90048-111">Boolean</span></span>    | <span data-ttu-id="90048-112">`true`Se o atributo deve ser usado como a âncora do objeto.</span><span class="sxs-lookup"><span data-stu-id="90048-112">`true` if the attribute should be used as the anchor for the object.</span></span> <span data-ttu-id="90048-113">Atributos de âncora devem ter um valor exclusivo que identifica um objeto e deve ser imutável.</span><span class="sxs-lookup"><span data-stu-id="90048-113">Anchor attributes must have a unique value identifying an object, and must be immutable.</span></span> <span data-ttu-id="90048-114">O padrão é `false`.</span><span class="sxs-lookup"><span data-stu-id="90048-114">Default is `false`.</span></span> <span data-ttu-id="90048-115">Um, e apenas um, dos atributos do objeto deve ser designado como a âncora para dar suporte à sincronização.</span><span class="sxs-lookup"><span data-stu-id="90048-115">One, and only one, of the object's attributes must be designated as the anchor to support synchronization.</span></span> |
|<span data-ttu-id="90048-116">caseExact</span><span class="sxs-lookup"><span data-stu-id="90048-116">caseExact</span></span>      |<span data-ttu-id="90048-117">Booliano</span><span class="sxs-lookup"><span data-stu-id="90048-117">Boolean</span></span>    |<span data-ttu-id="90048-118">`true`Se o valor desse atributo deve ser tratado como diferencia maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="90048-118">`true` if value of this attribute should be treated as case-sensitive.</span></span> <span data-ttu-id="90048-119">Essa configuração afeta como o mecanismo de sincronização detecta alterações para o atributo.</span><span class="sxs-lookup"><span data-stu-id="90048-119">This setting affects how the synchronization engine detects changes for the attribute.</span></span>|
|<span data-ttu-id="90048-120">flowNullValues</span><span class="sxs-lookup"><span data-stu-id="90048-120">flowNullValues</span></span> |<span data-ttu-id="90048-121">Booliano</span><span class="sxs-lookup"><span data-stu-id="90048-121">Boolean</span></span>    |<span data-ttu-id="90048-122">' true ' para permitir valores nulos de atributos.</span><span class="sxs-lookup"><span data-stu-id="90048-122">'true' to allow null values for attributes.</span></span>|
|<span data-ttu-id="90048-123">los</span><span class="sxs-lookup"><span data-stu-id="90048-123">metadata</span></span>       |<span data-ttu-id="90048-124">coleção [metadataEntry](../resources/synchronization-metadataentry.md)</span><span class="sxs-lookup"><span data-stu-id="90048-124">[metadataEntry](../resources/synchronization-metadataentry.md) collection</span></span>   |<span data-ttu-id="90048-125">Propriedades de extensão adicionais.</span><span class="sxs-lookup"><span data-stu-id="90048-125">Additional extension properties.</span></span> <span data-ttu-id="90048-126">A menos que seja mencionado explicitamente, os valores de metadados não devem ser alterados.</span><span class="sxs-lookup"><span data-stu-id="90048-126">Unless mentioned explicitly, metadata values should not be changed.</span></span>|
|<span data-ttu-id="90048-127">múltiplos valores</span><span class="sxs-lookup"><span data-stu-id="90048-127">multivalued</span></span>    |<span data-ttu-id="90048-128">Booliano</span><span class="sxs-lookup"><span data-stu-id="90048-128">Boolean</span></span>    |<span data-ttu-id="90048-129">`true`se um atributo puder ter vários valores.</span><span class="sxs-lookup"><span data-stu-id="90048-129">`true` if an attribute can have multiple values.</span></span> <span data-ttu-id="90048-130">O padrão é `false`.</span><span class="sxs-lookup"><span data-stu-id="90048-130">Default is `false`.</span></span>|
|<span data-ttu-id="90048-131">Imutabilidade</span><span class="sxs-lookup"><span data-stu-id="90048-131">mutability</span></span>     |<span data-ttu-id="90048-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="90048-132">String</span></span>     |<span data-ttu-id="90048-133">Uma imutabilidade de atributo.</span><span class="sxs-lookup"><span data-stu-id="90048-133">An attribute's mutability.</span></span> <span data-ttu-id="90048-134">Os valores possíveis são: `ReadWrite` , `ReadOnly` , `Immutable` , `WriteOnly` .</span><span class="sxs-lookup"><span data-stu-id="90048-134">Possible values are:  `ReadWrite`, `ReadOnly`, `Immutable`, `WriteOnly`.</span></span> <span data-ttu-id="90048-135">O padrão é `ReadWrite`.</span><span class="sxs-lookup"><span data-stu-id="90048-135">Default is `ReadWrite`.</span></span>|
|<span data-ttu-id="90048-136">nome</span><span class="sxs-lookup"><span data-stu-id="90048-136">name</span></span>           |<span data-ttu-id="90048-137">String</span><span class="sxs-lookup"><span data-stu-id="90048-137">String</span></span>     |<span data-ttu-id="90048-138">Nome do atributo.</span><span class="sxs-lookup"><span data-stu-id="90048-138">Name of the attribute.</span></span> <span data-ttu-id="90048-139">Deve ser exclusivo dentro da definição do objeto.</span><span class="sxs-lookup"><span data-stu-id="90048-139">Must be unique within the object definition.</span></span> <span data-ttu-id="90048-140">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="90048-140">Not nullable.</span></span>|
|<span data-ttu-id="90048-141">obrigatório</span><span class="sxs-lookup"><span data-stu-id="90048-141">required</span></span>       |<span data-ttu-id="90048-142">Booliano</span><span class="sxs-lookup"><span data-stu-id="90048-142">Boolean</span></span>    |<span data-ttu-id="90048-143">`true`Se o atributo for necessário.</span><span class="sxs-lookup"><span data-stu-id="90048-143">`true` if attribute is required.</span></span> <span data-ttu-id="90048-144">Objeto não pode ser criado se qualquer um dos atributos necessários estiver ausente.</span><span class="sxs-lookup"><span data-stu-id="90048-144">Object can not be created if any of the required attributes are missing.</span></span> <span data-ttu-id="90048-145">Se durante a sincronização, o atributo Required não tem valor, o valor padrão será usado.</span><span class="sxs-lookup"><span data-stu-id="90048-145">If during synchronization, the required attribute has no value, the default value will be used.</span></span> <span data-ttu-id="90048-146">Se o valor padrão não foi definido, a sincronização registrará um erro.</span><span class="sxs-lookup"><span data-stu-id="90048-146">If default the value was not set, synchronization will record an error.</span></span>|
|<span data-ttu-id="90048-147">referencedObjects</span><span class="sxs-lookup"><span data-stu-id="90048-147">referencedObjects</span></span>|<span data-ttu-id="90048-148">coleção [referenciable](../resources/synchronization-referencedobject.md)</span><span class="sxs-lookup"><span data-stu-id="90048-148">[referencedObject](../resources/synchronization-referencedobject.md) collection</span></span> |<span data-ttu-id="90048-149">Para atributos com `reference` tipo, lista objetos referenciados (por exemplo, o `manager` atributo seria List `User` como o objeto referenciado).</span><span class="sxs-lookup"><span data-stu-id="90048-149">For attributes with `reference` type, lists referenced objects (for example, the `manager` attribute would list `User` as the referenced object).</span></span>|
|<span data-ttu-id="90048-150">tipo</span><span class="sxs-lookup"><span data-stu-id="90048-150">type</span></span>           |<span data-ttu-id="90048-151">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="90048-151">String</span></span>     |<span data-ttu-id="90048-152">Tipo de valor de atributo.</span><span class="sxs-lookup"><span data-stu-id="90048-152">Attribute value type.</span></span> <span data-ttu-id="90048-153">Os valores possíveis são: `String`, `Integer`, `Reference`, `Binary`, `Boolean`.</span><span class="sxs-lookup"><span data-stu-id="90048-153">Possible values are: `String`, `Integer`, `Reference`, `Binary`, `Boolean`.</span></span> <span data-ttu-id="90048-154">O padrão é `String`.</span><span class="sxs-lookup"><span data-stu-id="90048-154">Default is `String`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="90048-155">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="90048-155">JSON representation</span></span>

<span data-ttu-id="90048-156">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="90048-156">The following is a JSON representation of the resource.</span></span>

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
  "flowNullValues": true,
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
