---
title: tipo de recurso de attributeDefinition
description: Descreve um atributo de um objeto.
localization_priority: Normal
ms.openlocfilehash: 63b7f67808ab6695b30f5464d72aed2814e46c5a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27829677"
---
# <a name="attributedefinition-resource-type"></a><span data-ttu-id="386b7-103">tipo de recurso de attributeDefinition</span><span class="sxs-lookup"><span data-stu-id="386b7-103">attributeDefinition resource type</span></span>

> <span data-ttu-id="386b7-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="386b7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="386b7-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="386b7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="386b7-106">Descreve um atributo de um objeto.</span><span class="sxs-lookup"><span data-stu-id="386b7-106">Describes an attribute of an object.</span></span>

## <a name="properties"></a><span data-ttu-id="386b7-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="386b7-107">Properties</span></span>

| <span data-ttu-id="386b7-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="386b7-108">Property</span></span>      | <span data-ttu-id="386b7-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="386b7-109">Type</span></span>      | <span data-ttu-id="386b7-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="386b7-110">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="386b7-111">âncora</span><span class="sxs-lookup"><span data-stu-id="386b7-111">anchor</span></span>         |<span data-ttu-id="386b7-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="386b7-112">Boolean</span></span>    | <span data-ttu-id="386b7-113">`true`Se o atributo deve ser usado como a âncora do objeto.</span><span class="sxs-lookup"><span data-stu-id="386b7-113">`true` if the attribute should be used as the anchor for the object.</span></span> <span data-ttu-id="386b7-114">Atributos de âncora devem ter um valor exclusivo que identifica um objeto e devem ser imutáveis.</span><span class="sxs-lookup"><span data-stu-id="386b7-114">Anchor attributes must have a unique value identifying an object, and must be immutable.</span></span> <span data-ttu-id="386b7-115">O padrão é `false`.</span><span class="sxs-lookup"><span data-stu-id="386b7-115">Default is `false`.</span></span> <span data-ttu-id="386b7-116">Um e somente um dos atributos do objeto devem ser designado como a âncora para oferecer suporte à sincronização.</span><span class="sxs-lookup"><span data-stu-id="386b7-116">One, and only one, of the object's attributes must be designated as the anchor to support synchronization.</span></span> |
|<span data-ttu-id="386b7-117">caseExact</span><span class="sxs-lookup"><span data-stu-id="386b7-117">caseExact</span></span>      |<span data-ttu-id="386b7-118">Booliano</span><span class="sxs-lookup"><span data-stu-id="386b7-118">Boolean</span></span>    |<span data-ttu-id="386b7-119">`true`Se o valor desse atributo deve ser tratado como diferencia maiusculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="386b7-119">`true` if value of this attribute should be treated as case-sensitive.</span></span> <span data-ttu-id="386b7-120">Essa configuração afeta como o mecanismo de sincronização detecta alterações para o atributo.</span><span class="sxs-lookup"><span data-stu-id="386b7-120">This setting affects how the synchronization engine detects changes for the attribute.</span></span>|
|<span data-ttu-id="386b7-121">metadados</span><span class="sxs-lookup"><span data-stu-id="386b7-121">metadata</span></span>       |[<span data-ttu-id="386b7-122">metadataEntry</span><span class="sxs-lookup"><span data-stu-id="386b7-122">metadataEntry</span></span>](../resources/synchronization-metadataentry.md)    |<span data-ttu-id="386b7-123">Propriedades adicionais de extensão.</span><span class="sxs-lookup"><span data-stu-id="386b7-123">Additional extension properties.</span></span> <span data-ttu-id="386b7-124">A menos que mencionado explicitamente, valores de metadados não devem ser alterados.</span><span class="sxs-lookup"><span data-stu-id="386b7-124">Unless mentioned explicitly, metadata values should not be changed.</span></span>|
|<span data-ttu-id="386b7-125">vários valores</span><span class="sxs-lookup"><span data-stu-id="386b7-125">multivalued</span></span>    |<span data-ttu-id="386b7-126">Booliano</span><span class="sxs-lookup"><span data-stu-id="386b7-126">Boolean</span></span>    |<span data-ttu-id="386b7-127">`true`Se um atributo pode ter vários valores.</span><span class="sxs-lookup"><span data-stu-id="386b7-127">`true` if an attribute can have multiple values.</span></span> <span data-ttu-id="386b7-128">O padrão é `false`.</span><span class="sxs-lookup"><span data-stu-id="386b7-128">Default is `false`.</span></span>|
|<span data-ttu-id="386b7-129">Mutabilidade</span><span class="sxs-lookup"><span data-stu-id="386b7-129">mutability</span></span>     |<span data-ttu-id="386b7-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="386b7-130">String</span></span>     |<span data-ttu-id="386b7-131">Mutabilidade de um atributo.</span><span class="sxs-lookup"><span data-stu-id="386b7-131">An attribute's mutability.</span></span> <span data-ttu-id="386b7-132">Os valores possíveis são: `ReadWrite`, `ReadOnly`, `Immutable`, `WriteOnly`.</span><span class="sxs-lookup"><span data-stu-id="386b7-132">Possible values are:  `ReadWrite`, `ReadOnly`, `Immutable`, `WriteOnly`.</span></span> <span data-ttu-id="386b7-133">O padrão é `ReadWrite`.</span><span class="sxs-lookup"><span data-stu-id="386b7-133">Default is `ReadWrite`.</span></span>|
|<span data-ttu-id="386b7-134">name</span><span class="sxs-lookup"><span data-stu-id="386b7-134">name</span></span>           |<span data-ttu-id="386b7-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="386b7-135">String</span></span>     |<span data-ttu-id="386b7-136">Nome do atributo.</span><span class="sxs-lookup"><span data-stu-id="386b7-136">Name of the attribute.</span></span> <span data-ttu-id="386b7-137">Deve ser exclusivo dentro da definição do objeto.</span><span class="sxs-lookup"><span data-stu-id="386b7-137">Must be unique within the object definition.</span></span> <span data-ttu-id="386b7-138">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="386b7-138">Not nullable.</span></span>|
|<span data-ttu-id="386b7-139">obrigatório</span><span class="sxs-lookup"><span data-stu-id="386b7-139">required</span></span>       |<span data-ttu-id="386b7-140">Booliano</span><span class="sxs-lookup"><span data-stu-id="386b7-140">Boolean</span></span>    |<span data-ttu-id="386b7-141">`true`Se o atributo é necessário.</span><span class="sxs-lookup"><span data-stu-id="386b7-141">`true` if attribute is required.</span></span> <span data-ttu-id="386b7-142">Objeto não pode ser criado se qualquer um dos atributos necessários estão ausentes.</span><span class="sxs-lookup"><span data-stu-id="386b7-142">Object can not be created if any of the required attributes are missing.</span></span> <span data-ttu-id="386b7-143">Se durante a sincronização, o atributo required não tiver nenhum valor, o valor padrão será usado.</span><span class="sxs-lookup"><span data-stu-id="386b7-143">If during synchronization, the required attribute has no value, the default value will be used.</span></span> <span data-ttu-id="386b7-144">Se o valor do padrão não foi definido, a sincronização irá registrar um erro.</span><span class="sxs-lookup"><span data-stu-id="386b7-144">If default the value was not set, synchronization will record an error.</span></span>|
|<span data-ttu-id="386b7-145">referencedObjects</span><span class="sxs-lookup"><span data-stu-id="386b7-145">referencedObjects</span></span>|[<span data-ttu-id="386b7-146">referencedObject</span><span class="sxs-lookup"><span data-stu-id="386b7-146">referencedObject</span></span>](../resources/synchronization-referencedobject.md) |<span data-ttu-id="386b7-147">Para atributos com `reference` digitar, listas de objetos referenciados (por exemplo, o `manager` atributo seria listar `User` como o objeto referenciado).</span><span class="sxs-lookup"><span data-stu-id="386b7-147">For attributes with `reference` type, lists referenced objects (for example, the `manager` attribute would list `User` as the referenced object).</span></span>|
|<span data-ttu-id="386b7-148">type</span><span class="sxs-lookup"><span data-stu-id="386b7-148">type</span></span>           |<span data-ttu-id="386b7-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="386b7-149">String</span></span>     |<span data-ttu-id="386b7-150">Tipo de valor do atributo.</span><span class="sxs-lookup"><span data-stu-id="386b7-150">Attribute value type.</span></span> <span data-ttu-id="386b7-151">Os valores possíveis são: `String`, `Integer`, `Reference`, `Binary`, `Boolean`.</span><span class="sxs-lookup"><span data-stu-id="386b7-151">Possible values are: `String`, `Integer`, `Reference`, `Binary`, `Boolean`.</span></span> <span data-ttu-id="386b7-152">O padrão é `String`.</span><span class="sxs-lookup"><span data-stu-id="386b7-152">Default is `String`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="386b7-153">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="386b7-153">JSON representation</span></span>

<span data-ttu-id="386b7-154">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="386b7-154">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "attributeDefinition resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
