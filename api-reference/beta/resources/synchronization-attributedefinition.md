---
title: Tipo de recurso attributeDefinition
description: Descreve um atributo de um objeto.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: a9c50721c1ee19505edc2507313cc346a6adabfd
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50956810"
---
# <a name="attributedefinition-resource-type"></a><span data-ttu-id="7b87a-103">Tipo de recurso attributeDefinition</span><span class="sxs-lookup"><span data-stu-id="7b87a-103">attributeDefinition resource type</span></span>

<span data-ttu-id="7b87a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7b87a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7b87a-105">Descreve um atributo de um objeto.</span><span class="sxs-lookup"><span data-stu-id="7b87a-105">Describes an attribute of an object.</span></span>

## <a name="properties"></a><span data-ttu-id="7b87a-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7b87a-106">Properties</span></span>

| <span data-ttu-id="7b87a-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7b87a-107">Property</span></span>      | <span data-ttu-id="7b87a-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="7b87a-108">Type</span></span>      | <span data-ttu-id="7b87a-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="7b87a-109">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="7b87a-110">anchor</span><span class="sxs-lookup"><span data-stu-id="7b87a-110">anchor</span></span>         |<span data-ttu-id="7b87a-111">Booliano</span><span class="sxs-lookup"><span data-stu-id="7b87a-111">Boolean</span></span>    | <span data-ttu-id="7b87a-112">`true` se o atributo deve ser usado como âncora para o objeto.</span><span class="sxs-lookup"><span data-stu-id="7b87a-112">`true` if the attribute should be used as the anchor for the object.</span></span> <span data-ttu-id="7b87a-113">Os atributos de âncora devem ter um valor exclusivo que identifique um objeto e devem ser imutáveis.</span><span class="sxs-lookup"><span data-stu-id="7b87a-113">Anchor attributes must have a unique value identifying an object, and must be immutable.</span></span> <span data-ttu-id="7b87a-114">O padrão é `false`.</span><span class="sxs-lookup"><span data-stu-id="7b87a-114">Default is `false`.</span></span> <span data-ttu-id="7b87a-115">Um e apenas um dos atributos do objeto devem ser designados como âncora para dar suporte à sincronização.</span><span class="sxs-lookup"><span data-stu-id="7b87a-115">One, and only one, of the object's attributes must be designated as the anchor to support synchronization.</span></span> |
|<span data-ttu-id="7b87a-116">caseExact</span><span class="sxs-lookup"><span data-stu-id="7b87a-116">caseExact</span></span>      |<span data-ttu-id="7b87a-117">Booliano</span><span class="sxs-lookup"><span data-stu-id="7b87a-117">Boolean</span></span>    |<span data-ttu-id="7b87a-118">`true` se o valor desse atributo deve ser tratado como sensível a caso.</span><span class="sxs-lookup"><span data-stu-id="7b87a-118">`true` if value of this attribute should be treated as case-sensitive.</span></span> <span data-ttu-id="7b87a-119">Essa configuração afeta como o mecanismo de sincronização detecta alterações para o atributo.</span><span class="sxs-lookup"><span data-stu-id="7b87a-119">This setting affects how the synchronization engine detects changes for the attribute.</span></span>|
|<span data-ttu-id="7b87a-120">flowNullValues</span><span class="sxs-lookup"><span data-stu-id="7b87a-120">flowNullValues</span></span> |<span data-ttu-id="7b87a-121">Booliano</span><span class="sxs-lookup"><span data-stu-id="7b87a-121">Boolean</span></span>    |<span data-ttu-id="7b87a-122">'true' para permitir valores nulos para atributos.</span><span class="sxs-lookup"><span data-stu-id="7b87a-122">'true' to allow null values for attributes.</span></span>|
|<span data-ttu-id="7b87a-123">metadados</span><span class="sxs-lookup"><span data-stu-id="7b87a-123">metadata</span></span>       |<span data-ttu-id="7b87a-124">[Coleção metadataEntry](../resources/synchronization-metadataentry.md)</span><span class="sxs-lookup"><span data-stu-id="7b87a-124">[metadataEntry](../resources/synchronization-metadataentry.md) collection</span></span>   |<span data-ttu-id="7b87a-125">Propriedades de extensão adicionais.</span><span class="sxs-lookup"><span data-stu-id="7b87a-125">Additional extension properties.</span></span> <span data-ttu-id="7b87a-126">A menos que mencionado explicitamente, os valores de metadados não devem ser alterados.</span><span class="sxs-lookup"><span data-stu-id="7b87a-126">Unless mentioned explicitly, metadata values should not be changed.</span></span>|
|<span data-ttu-id="7b87a-127">multivalued</span><span class="sxs-lookup"><span data-stu-id="7b87a-127">multivalued</span></span>    |<span data-ttu-id="7b87a-128">Booliano</span><span class="sxs-lookup"><span data-stu-id="7b87a-128">Boolean</span></span>    |<span data-ttu-id="7b87a-129">`true` se um atributo pode ter vários valores.</span><span class="sxs-lookup"><span data-stu-id="7b87a-129">`true` if an attribute can have multiple values.</span></span> <span data-ttu-id="7b87a-130">O padrão é `false`.</span><span class="sxs-lookup"><span data-stu-id="7b87a-130">Default is `false`.</span></span>|
|<span data-ttu-id="7b87a-131">mutabilidade</span><span class="sxs-lookup"><span data-stu-id="7b87a-131">mutability</span></span>     |<span data-ttu-id="7b87a-132">mutabilidade</span><span class="sxs-lookup"><span data-stu-id="7b87a-132">mutability</span></span>     |<span data-ttu-id="7b87a-133">Mutabilidade de um atributo.</span><span class="sxs-lookup"><span data-stu-id="7b87a-133">An attribute's mutability.</span></span> <span data-ttu-id="7b87a-134">Os valores possíveis são:  `ReadWrite` `ReadOnly` , , , `Immutable` `WriteOnly` .</span><span class="sxs-lookup"><span data-stu-id="7b87a-134">Possible values are:  `ReadWrite`, `ReadOnly`, `Immutable`, `WriteOnly`.</span></span> <span data-ttu-id="7b87a-135">O padrão é `ReadWrite`.</span><span class="sxs-lookup"><span data-stu-id="7b87a-135">Default is `ReadWrite`.</span></span>|
|<span data-ttu-id="7b87a-136">nome</span><span class="sxs-lookup"><span data-stu-id="7b87a-136">name</span></span>           |<span data-ttu-id="7b87a-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7b87a-137">String</span></span>     |<span data-ttu-id="7b87a-138">Nome do atributo.</span><span class="sxs-lookup"><span data-stu-id="7b87a-138">Name of the attribute.</span></span> <span data-ttu-id="7b87a-139">Deve ser exclusivo na definição do objeto.</span><span class="sxs-lookup"><span data-stu-id="7b87a-139">Must be unique within the object definition.</span></span> <span data-ttu-id="7b87a-140">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="7b87a-140">Not nullable.</span></span>|
|<span data-ttu-id="7b87a-141">obrigatório</span><span class="sxs-lookup"><span data-stu-id="7b87a-141">required</span></span>       |<span data-ttu-id="7b87a-142">Booliano</span><span class="sxs-lookup"><span data-stu-id="7b87a-142">Boolean</span></span>    |<span data-ttu-id="7b87a-143">`true` se o atributo for necessário.</span><span class="sxs-lookup"><span data-stu-id="7b87a-143">`true` if attribute is required.</span></span> <span data-ttu-id="7b87a-144">O objeto não poderá ser criado se nenhum dos atributos necessários estiver ausente.</span><span class="sxs-lookup"><span data-stu-id="7b87a-144">Object can not be created if any of the required attributes are missing.</span></span> <span data-ttu-id="7b87a-145">Se durante a sincronização, o atributo necessário não tiver valor, o valor padrão será usado.</span><span class="sxs-lookup"><span data-stu-id="7b87a-145">If during synchronization, the required attribute has no value, the default value will be used.</span></span> <span data-ttu-id="7b87a-146">Se o valor padrão não foi definido, a sincronização registrará um erro.</span><span class="sxs-lookup"><span data-stu-id="7b87a-146">If default the value was not set, synchronization will record an error.</span></span>|
|<span data-ttu-id="7b87a-147">referencedObjects</span><span class="sxs-lookup"><span data-stu-id="7b87a-147">referencedObjects</span></span>|<span data-ttu-id="7b87a-148">[Coleção referencedObject](../resources/synchronization-referencedobject.md)</span><span class="sxs-lookup"><span data-stu-id="7b87a-148">[referencedObject](../resources/synchronization-referencedobject.md) collection</span></span> |<span data-ttu-id="7b87a-149">Para atributos com `reference` tipo, lista objetos referenciados (por exemplo, o `manager` atributo listaria `User` como o objeto referenciado).</span><span class="sxs-lookup"><span data-stu-id="7b87a-149">For attributes with `reference` type, lists referenced objects (for example, the `manager` attribute would list `User` as the referenced object).</span></span>|
|<span data-ttu-id="7b87a-150">tipo</span><span class="sxs-lookup"><span data-stu-id="7b87a-150">type</span></span>           |<span data-ttu-id="7b87a-151">attributeType</span><span class="sxs-lookup"><span data-stu-id="7b87a-151">attributeType</span></span>     |<span data-ttu-id="7b87a-152">Tipo de valor de atributo.</span><span class="sxs-lookup"><span data-stu-id="7b87a-152">Attribute value type.</span></span> <span data-ttu-id="7b87a-153">Os valores possíveis `String` são: `Integer` , , , , , `Reference` `Binary` `Boolean` `DateTime` .</span><span class="sxs-lookup"><span data-stu-id="7b87a-153">Possible values are: `String`, `Integer`, `Reference`, `Binary`, `Boolean`,`DateTime`.</span></span> <span data-ttu-id="7b87a-154">O padrão é `String`.</span><span class="sxs-lookup"><span data-stu-id="7b87a-154">Default is `String`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7b87a-155">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7b87a-155">JSON representation</span></span>

<span data-ttu-id="7b87a-156">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7b87a-156">The following is a JSON representation of the resource.</span></span>

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


