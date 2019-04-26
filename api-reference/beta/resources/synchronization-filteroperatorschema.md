---
title: tipo de recurso filterOperatorSchema
description: Descreve um operador que pode ser usado em um filtro.
localization_priority: Normal
ms.openlocfilehash: 0f0ada4aaa02efa2484ffa75d88b2c8256f15fe8
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342851"
---
# <a name="filteroperatorschema-resource-type"></a><span data-ttu-id="52663-103">tipo de recurso filterOperatorSchema</span><span class="sxs-lookup"><span data-stu-id="52663-103">filterOperatorSchema resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="52663-104">Descreve um operador que pode ser usado em um [filtro](synchronization-filter.md).</span><span class="sxs-lookup"><span data-stu-id="52663-104">Describes an operator that can be used in a [filter](synchronization-filter.md).</span></span>

## <a name="properties"></a><span data-ttu-id="52663-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="52663-105">Properties</span></span>

| <span data-ttu-id="52663-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="52663-106">Property</span></span>                   | <span data-ttu-id="52663-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="52663-107">Type</span></span>                      | <span data-ttu-id="52663-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="52663-108">Description</span></span>    |
|:---------------------------|:--------------------------|:---------------|
|<span data-ttu-id="52663-109">arity</span><span class="sxs-lookup"><span data-stu-id="52663-109">arity</span></span>                       |<span data-ttu-id="52663-110">String</span><span class="sxs-lookup"><span data-stu-id="52663-110">String</span></span>          |<span data-ttu-id="52663-111">Arity do operador.</span><span class="sxs-lookup"><span data-stu-id="52663-111">Arity of the operator.</span></span> <span data-ttu-id="52663-112">Os valores possíveis são: `Binary` e `Unary`.</span><span class="sxs-lookup"><span data-stu-id="52663-112">Possible values are: `Binary`, `Unary`.</span></span> <span data-ttu-id="52663-113">O padrão é `Binary`.</span><span class="sxs-lookup"><span data-stu-id="52663-113">The default is `Binary`.</span></span>|
|<span data-ttu-id="52663-114">multivaluedComparisonType</span><span class="sxs-lookup"><span data-stu-id="52663-114">multivaluedComparisonType</span></span>   |<span data-ttu-id="52663-115">scopeOperatorMultiValuedComparisonType</span><span class="sxs-lookup"><span data-stu-id="52663-115">scopeOperatorMultiValuedComparisonType</span></span>          |<span data-ttu-id="52663-116">Os valores possíveis são: `All` e `Any`.</span><span class="sxs-lookup"><span data-stu-id="52663-116">Possible values are: `All`, `Any`.</span></span> <span data-ttu-id="52663-117">Aplica-se somente a atributos com vários valores.</span><span class="sxs-lookup"><span data-stu-id="52663-117">Applies only to multivalued attributes.</span></span> <span data-ttu-id="52663-118">`All`significa que todos os valores devem atender à condição.</span><span class="sxs-lookup"><span data-stu-id="52663-118">`All` means that all values must satisfy the condition.</span></span> <span data-ttu-id="52663-119">`Any`significa que pelo menos um valor deve satisfazer a condição.</span><span class="sxs-lookup"><span data-stu-id="52663-119">`Any` means that at least one value has to satisfy the condition.</span></span> <span data-ttu-id="52663-120">O padrão é `All`.</span><span class="sxs-lookup"><span data-stu-id="52663-120">The default is `All`.</span></span>|
|<span data-ttu-id="52663-121">name</span><span class="sxs-lookup"><span data-stu-id="52663-121">name</span></span>                        |<span data-ttu-id="52663-122">String</span><span class="sxs-lookup"><span data-stu-id="52663-122">String</span></span>                     |<span data-ttu-id="52663-123">Nome do operador.</span><span class="sxs-lookup"><span data-stu-id="52663-123">Operator name.</span></span> |
|<span data-ttu-id="52663-124">supportedAttributeTypes</span><span class="sxs-lookup"><span data-stu-id="52663-124">supportedAttributeTypes</span></span>     |<span data-ttu-id="52663-125">Coleção String</span><span class="sxs-lookup"><span data-stu-id="52663-125">String collection</span></span>         |<span data-ttu-id="52663-126">Tipos de atributo suportados pelo operador.</span><span class="sxs-lookup"><span data-stu-id="52663-126">Attribute types supported by the operator.</span></span> <span data-ttu-id="52663-127">Os valores possíveis são: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.</span><span class="sxs-lookup"><span data-stu-id="52663-127">Possible values are: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="52663-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="52663-128">JSON representation</span></span>

<span data-ttu-id="52663-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="52663-129">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.filterOperatorSchema"
}-->

```json
{
  "arity": "String",
  "multivaluedComparisonType": "String",
  "name": "String",
  "supportedAttributeTypes": ["String"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "filterOperatorSchema resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
