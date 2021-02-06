---
title: Tipo de recurso attributeDefinition
description: Descreve um atributo de um objeto.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 34503f3edf15542db449d56e5211cd33b3d9132e
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50128810"
---
# <a name="attributedefinition-resource-type"></a><span data-ttu-id="9d95d-103">Tipo de recurso attributeDefinition</span><span class="sxs-lookup"><span data-stu-id="9d95d-103">attributeDefinition resource type</span></span>

<span data-ttu-id="9d95d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9d95d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9d95d-105">Descreve um atributo de um objeto.</span><span class="sxs-lookup"><span data-stu-id="9d95d-105">Describes an attribute of an object.</span></span>

## <a name="properties"></a><span data-ttu-id="9d95d-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9d95d-106">Properties</span></span>

| <span data-ttu-id="9d95d-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9d95d-107">Property</span></span>      | <span data-ttu-id="9d95d-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="9d95d-108">Type</span></span>      | <span data-ttu-id="9d95d-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="9d95d-109">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="9d95d-110">âncora</span><span class="sxs-lookup"><span data-stu-id="9d95d-110">anchor</span></span>         |<span data-ttu-id="9d95d-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="9d95d-111">Boolean</span></span>    | <span data-ttu-id="9d95d-112">`true` se o atributo deve ser usado como âncora para o objeto.</span><span class="sxs-lookup"><span data-stu-id="9d95d-112">`true` if the attribute should be used as the anchor for the object.</span></span> <span data-ttu-id="9d95d-113">Os atributos de âncora devem ter um valor exclusivo que identifique um objeto e devem ser imutáveis.</span><span class="sxs-lookup"><span data-stu-id="9d95d-113">Anchor attributes must have a unique value identifying an object, and must be immutable.</span></span> <span data-ttu-id="9d95d-114">O padrão é `false`.</span><span class="sxs-lookup"><span data-stu-id="9d95d-114">Default is `false`.</span></span> <span data-ttu-id="9d95d-115">Um e apenas um dos atributos do objeto devem ser designados como a âncora para suportar a sincronização.</span><span class="sxs-lookup"><span data-stu-id="9d95d-115">One, and only one, of the object's attributes must be designated as the anchor to support synchronization.</span></span> |
|<span data-ttu-id="9d95d-116">caseExact</span><span class="sxs-lookup"><span data-stu-id="9d95d-116">caseExact</span></span>      |<span data-ttu-id="9d95d-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="9d95d-117">Boolean</span></span>    |<span data-ttu-id="9d95d-118">`true` se o valor desse atributo deve ser tratado como sensível a minúsculas.</span><span class="sxs-lookup"><span data-stu-id="9d95d-118">`true` if value of this attribute should be treated as case-sensitive.</span></span> <span data-ttu-id="9d95d-119">Essa configuração afeta como o mecanismo de sincronização detecta alterações para o atributo.</span><span class="sxs-lookup"><span data-stu-id="9d95d-119">This setting affects how the synchronization engine detects changes for the attribute.</span></span>|
|<span data-ttu-id="9d95d-120">flowNullValues</span><span class="sxs-lookup"><span data-stu-id="9d95d-120">flowNullValues</span></span> |<span data-ttu-id="9d95d-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="9d95d-121">Boolean</span></span>    |<span data-ttu-id="9d95d-122">"true" para permitir valores nulos para atributos.</span><span class="sxs-lookup"><span data-stu-id="9d95d-122">'true' to allow null values for attributes.</span></span>|
|<span data-ttu-id="9d95d-123">metadados</span><span class="sxs-lookup"><span data-stu-id="9d95d-123">metadata</span></span>       |<span data-ttu-id="9d95d-124">[Coleção metadataEntry](../resources/synchronization-metadataentry.md)</span><span class="sxs-lookup"><span data-stu-id="9d95d-124">[metadataEntry](../resources/synchronization-metadataentry.md) collection</span></span>   |<span data-ttu-id="9d95d-125">Propriedades de extensão adicionais.</span><span class="sxs-lookup"><span data-stu-id="9d95d-125">Additional extension properties.</span></span> <span data-ttu-id="9d95d-126">A menos que seja mencionado explicitamente, os valores de metadados não devem ser alterados.</span><span class="sxs-lookup"><span data-stu-id="9d95d-126">Unless mentioned explicitly, metadata values should not be changed.</span></span>|
|<span data-ttu-id="9d95d-127">multivalorado</span><span class="sxs-lookup"><span data-stu-id="9d95d-127">multivalued</span></span>    |<span data-ttu-id="9d95d-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="9d95d-128">Boolean</span></span>    |<span data-ttu-id="9d95d-129">`true` se um atributo puder ter vários valores.</span><span class="sxs-lookup"><span data-stu-id="9d95d-129">`true` if an attribute can have multiple values.</span></span> <span data-ttu-id="9d95d-130">O padrão é `false`.</span><span class="sxs-lookup"><span data-stu-id="9d95d-130">Default is `false`.</span></span>|
|<span data-ttu-id="9d95d-131">mutability</span><span class="sxs-lookup"><span data-stu-id="9d95d-131">mutability</span></span>     |<span data-ttu-id="9d95d-132">String</span><span class="sxs-lookup"><span data-stu-id="9d95d-132">String</span></span>     |<span data-ttu-id="9d95d-133">A transformabilidade de um atributo.</span><span class="sxs-lookup"><span data-stu-id="9d95d-133">An attribute's mutability.</span></span> <span data-ttu-id="9d95d-134">Os valores possíveis `ReadWrite` são: `ReadOnly` , , `Immutable` . `WriteOnly`</span><span class="sxs-lookup"><span data-stu-id="9d95d-134">Possible values are:  `ReadWrite`, `ReadOnly`, `Immutable`, `WriteOnly`.</span></span> <span data-ttu-id="9d95d-135">O padrão é `ReadWrite`.</span><span class="sxs-lookup"><span data-stu-id="9d95d-135">Default is `ReadWrite`.</span></span>|
|<span data-ttu-id="9d95d-136">nome</span><span class="sxs-lookup"><span data-stu-id="9d95d-136">name</span></span>           |<span data-ttu-id="9d95d-137">String</span><span class="sxs-lookup"><span data-stu-id="9d95d-137">String</span></span>     |<span data-ttu-id="9d95d-138">Nome do atributo.</span><span class="sxs-lookup"><span data-stu-id="9d95d-138">Name of the attribute.</span></span> <span data-ttu-id="9d95d-139">Deve ser exclusivo na definição do objeto.</span><span class="sxs-lookup"><span data-stu-id="9d95d-139">Must be unique within the object definition.</span></span> <span data-ttu-id="9d95d-140">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="9d95d-140">Not nullable.</span></span>|
|<span data-ttu-id="9d95d-141">obrigatório</span><span class="sxs-lookup"><span data-stu-id="9d95d-141">required</span></span>       |<span data-ttu-id="9d95d-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="9d95d-142">Boolean</span></span>    |<span data-ttu-id="9d95d-143">`true` se o atributo for necessário.</span><span class="sxs-lookup"><span data-stu-id="9d95d-143">`true` if attribute is required.</span></span> <span data-ttu-id="9d95d-144">O objeto não poderá ser criado se nenhum dos atributos necessários estiver faltando.</span><span class="sxs-lookup"><span data-stu-id="9d95d-144">Object can not be created if any of the required attributes are missing.</span></span> <span data-ttu-id="9d95d-145">Se, durante a sincronização, o atributo necessário não tiver valor, o valor padrão será usado.</span><span class="sxs-lookup"><span data-stu-id="9d95d-145">If during synchronization, the required attribute has no value, the default value will be used.</span></span> <span data-ttu-id="9d95d-146">Se o valor padrão não foi definido, a sincronização registrará um erro.</span><span class="sxs-lookup"><span data-stu-id="9d95d-146">If default the value was not set, synchronization will record an error.</span></span>|
|<span data-ttu-id="9d95d-147">referencedObjects</span><span class="sxs-lookup"><span data-stu-id="9d95d-147">referencedObjects</span></span>|<span data-ttu-id="9d95d-148">[Coleção referencedObject](../resources/synchronization-referencedobject.md)</span><span class="sxs-lookup"><span data-stu-id="9d95d-148">[referencedObject](../resources/synchronization-referencedobject.md) collection</span></span> |<span data-ttu-id="9d95d-149">Para atributos com `reference` tipo, listas de objetos referenciados (por exemplo, o `manager` atributo listaria `User` como o objeto referenciado).</span><span class="sxs-lookup"><span data-stu-id="9d95d-149">For attributes with `reference` type, lists referenced objects (for example, the `manager` attribute would list `User` as the referenced object).</span></span>|
|<span data-ttu-id="9d95d-150">type</span><span class="sxs-lookup"><span data-stu-id="9d95d-150">type</span></span>           |<span data-ttu-id="9d95d-151">String</span><span class="sxs-lookup"><span data-stu-id="9d95d-151">String</span></span>     |<span data-ttu-id="9d95d-152">Tipo de valor de atributo.</span><span class="sxs-lookup"><span data-stu-id="9d95d-152">Attribute value type.</span></span> <span data-ttu-id="9d95d-153">Os valores possíveis são: `String`, `Integer`, `Reference`, `Binary`, `Boolean`.</span><span class="sxs-lookup"><span data-stu-id="9d95d-153">Possible values are: `String`, `Integer`, `Reference`, `Binary`, `Boolean`.</span></span> <span data-ttu-id="9d95d-154">O padrão é `String`.</span><span class="sxs-lookup"><span data-stu-id="9d95d-154">Default is `String`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9d95d-155">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9d95d-155">JSON representation</span></span>

<span data-ttu-id="9d95d-156">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9d95d-156">The following is a JSON representation of the resource.</span></span>

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


