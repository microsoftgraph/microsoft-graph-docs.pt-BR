---
title: tipo de recurso de attributeDefinition
description: Descreve um atributo de um objeto.
localization_priority: Normal
ms.openlocfilehash: f9268bf61fec397c53744c9999635ba159b047f4
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643913"
---
# <a name="attributedefinition-resource-type"></a><span data-ttu-id="0fb82-103">tipo de recurso de attributeDefinition</span><span class="sxs-lookup"><span data-stu-id="0fb82-103">attributeDefinition resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0fb82-104">Descreve um atributo de um objeto.</span><span class="sxs-lookup"><span data-stu-id="0fb82-104">Describes an attribute of an object.</span></span>

## <a name="properties"></a><span data-ttu-id="0fb82-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0fb82-105">Properties</span></span>

| <span data-ttu-id="0fb82-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0fb82-106">Property</span></span>      | <span data-ttu-id="0fb82-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="0fb82-107">Type</span></span>      | <span data-ttu-id="0fb82-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="0fb82-108">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="0fb82-109">âncora</span><span class="sxs-lookup"><span data-stu-id="0fb82-109">anchor</span></span>         |<span data-ttu-id="0fb82-110">Booliano</span><span class="sxs-lookup"><span data-stu-id="0fb82-110">Boolean</span></span>    | <span data-ttu-id="0fb82-111">`true`Se o atributo deve ser usado como a âncora do objeto.</span><span class="sxs-lookup"><span data-stu-id="0fb82-111">`true` if the attribute should be used as the anchor for the object.</span></span> <span data-ttu-id="0fb82-112">Atributos de âncora devem ter um valor exclusivo que identifica um objeto e devem ser imutáveis.</span><span class="sxs-lookup"><span data-stu-id="0fb82-112">Anchor attributes must have a unique value identifying an object, and must be immutable.</span></span> <span data-ttu-id="0fb82-113">O padrão é `false`.</span><span class="sxs-lookup"><span data-stu-id="0fb82-113">Default is `false`.</span></span> <span data-ttu-id="0fb82-114">Um e somente um dos atributos do objeto devem ser designado como a âncora para oferecer suporte à sincronização.</span><span class="sxs-lookup"><span data-stu-id="0fb82-114">One, and only one, of the object's attributes must be designated as the anchor to support synchronization.</span></span> |
|<span data-ttu-id="0fb82-115">caseExact</span><span class="sxs-lookup"><span data-stu-id="0fb82-115">caseExact</span></span>      |<span data-ttu-id="0fb82-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="0fb82-116">Boolean</span></span>    |<span data-ttu-id="0fb82-117">`true`Se o valor desse atributo deve ser tratado como diferencia maiusculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="0fb82-117">`true` if value of this attribute should be treated as case-sensitive.</span></span> <span data-ttu-id="0fb82-118">Essa configuração afeta como o mecanismo de sincronização detecta alterações para o atributo.</span><span class="sxs-lookup"><span data-stu-id="0fb82-118">This setting affects how the synchronization engine detects changes for the attribute.</span></span>|
|<span data-ttu-id="0fb82-119">metadados</span><span class="sxs-lookup"><span data-stu-id="0fb82-119">metadata</span></span>       |[<span data-ttu-id="0fb82-120">metadataEntry</span><span class="sxs-lookup"><span data-stu-id="0fb82-120">metadataEntry</span></span>](../resources/synchronization-metadataentry.md)    |<span data-ttu-id="0fb82-121">Propriedades adicionais de extensão.</span><span class="sxs-lookup"><span data-stu-id="0fb82-121">Additional extension properties.</span></span> <span data-ttu-id="0fb82-122">A menos que mencionado explicitamente, valores de metadados não devem ser alterados.</span><span class="sxs-lookup"><span data-stu-id="0fb82-122">Unless mentioned explicitly, metadata values should not be changed.</span></span>|
|<span data-ttu-id="0fb82-123">vários valores</span><span class="sxs-lookup"><span data-stu-id="0fb82-123">multivalued</span></span>    |<span data-ttu-id="0fb82-124">Booliano</span><span class="sxs-lookup"><span data-stu-id="0fb82-124">Boolean</span></span>    |<span data-ttu-id="0fb82-125">`true`Se um atributo pode ter vários valores.</span><span class="sxs-lookup"><span data-stu-id="0fb82-125">`true` if an attribute can have multiple values.</span></span> <span data-ttu-id="0fb82-126">O padrão é `false`.</span><span class="sxs-lookup"><span data-stu-id="0fb82-126">Default is `false`.</span></span>|
|<span data-ttu-id="0fb82-127">Mutabilidade</span><span class="sxs-lookup"><span data-stu-id="0fb82-127">mutability</span></span>     |<span data-ttu-id="0fb82-128">String</span><span class="sxs-lookup"><span data-stu-id="0fb82-128">String</span></span>     |<span data-ttu-id="0fb82-129">Mutabilidade de um atributo.</span><span class="sxs-lookup"><span data-stu-id="0fb82-129">An attribute's mutability.</span></span> <span data-ttu-id="0fb82-130">Os valores possíveis são: `ReadWrite`, `ReadOnly`, `Immutable`, `WriteOnly`.</span><span class="sxs-lookup"><span data-stu-id="0fb82-130">Possible values are:  `ReadWrite`, `ReadOnly`, `Immutable`, `WriteOnly`.</span></span> <span data-ttu-id="0fb82-131">O padrão é `ReadWrite`.</span><span class="sxs-lookup"><span data-stu-id="0fb82-131">Default is `ReadWrite`.</span></span>|
|<span data-ttu-id="0fb82-132">name</span><span class="sxs-lookup"><span data-stu-id="0fb82-132">name</span></span>           |<span data-ttu-id="0fb82-133">String</span><span class="sxs-lookup"><span data-stu-id="0fb82-133">String</span></span>     |<span data-ttu-id="0fb82-134">Nome do atributo.</span><span class="sxs-lookup"><span data-stu-id="0fb82-134">Name of the attribute.</span></span> <span data-ttu-id="0fb82-135">Deve ser exclusivo dentro da definição do objeto.</span><span class="sxs-lookup"><span data-stu-id="0fb82-135">Must be unique within the object definition.</span></span> <span data-ttu-id="0fb82-136">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="0fb82-136">Not nullable.</span></span>|
|<span data-ttu-id="0fb82-137">obrigatório</span><span class="sxs-lookup"><span data-stu-id="0fb82-137">required</span></span>       |<span data-ttu-id="0fb82-138">Booliano</span><span class="sxs-lookup"><span data-stu-id="0fb82-138">Boolean</span></span>    |<span data-ttu-id="0fb82-139">`true`Se o atributo é necessário.</span><span class="sxs-lookup"><span data-stu-id="0fb82-139">`true` if attribute is required.</span></span> <span data-ttu-id="0fb82-140">Objeto não pode ser criado se qualquer um dos atributos necessários estão ausentes.</span><span class="sxs-lookup"><span data-stu-id="0fb82-140">Object can not be created if any of the required attributes are missing.</span></span> <span data-ttu-id="0fb82-141">Se durante a sincronização, o atributo required não tiver nenhum valor, o valor padrão será usado.</span><span class="sxs-lookup"><span data-stu-id="0fb82-141">If during synchronization, the required attribute has no value, the default value will be used.</span></span> <span data-ttu-id="0fb82-142">Se o valor do padrão não foi definido, a sincronização irá registrar um erro.</span><span class="sxs-lookup"><span data-stu-id="0fb82-142">If default the value was not set, synchronization will record an error.</span></span>|
|<span data-ttu-id="0fb82-143">referencedObjects</span><span class="sxs-lookup"><span data-stu-id="0fb82-143">referencedObjects</span></span>|[<span data-ttu-id="0fb82-144">referencedObject</span><span class="sxs-lookup"><span data-stu-id="0fb82-144">referencedObject</span></span>](../resources/synchronization-referencedobject.md) |<span data-ttu-id="0fb82-145">Para atributos com `reference` digitar, listas de objetos referenciados (por exemplo, o `manager` atributo seria listar `User` como o objeto referenciado).</span><span class="sxs-lookup"><span data-stu-id="0fb82-145">For attributes with `reference` type, lists referenced objects (for example, the `manager` attribute would list `User` as the referenced object).</span></span>|
|<span data-ttu-id="0fb82-146">type</span><span class="sxs-lookup"><span data-stu-id="0fb82-146">type</span></span>           |<span data-ttu-id="0fb82-147">String</span><span class="sxs-lookup"><span data-stu-id="0fb82-147">String</span></span>     |<span data-ttu-id="0fb82-148">Tipo de valor do atributo.</span><span class="sxs-lookup"><span data-stu-id="0fb82-148">Attribute value type.</span></span> <span data-ttu-id="0fb82-149">Os valores possíveis são: `String`, `Integer`, `Reference`, `Binary`, `Boolean`.</span><span class="sxs-lookup"><span data-stu-id="0fb82-149">Possible values are: `String`, `Integer`, `Reference`, `Binary`, `Boolean`.</span></span> <span data-ttu-id="0fb82-150">O padrão é `String`.</span><span class="sxs-lookup"><span data-stu-id="0fb82-150">Default is `String`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0fb82-151">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0fb82-151">JSON representation</span></span>

<span data-ttu-id="0fb82-152">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0fb82-152">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-attributedefinition.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
