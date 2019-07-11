---
title: tipo de recurso filterOperatorSchema
description: Descreve um operador que pode ser usado em um filtro.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c55838e6e7d12789d1bd84d63dff95b4d9b72efa
ms.sourcegitcommit: 121c0fad692fb3c5c01dc051481b5249e4491b48
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/11/2019
ms.locfileid: "35621365"
---
# <a name="filteroperatorschema-resource-type"></a><span data-ttu-id="5faf1-103">tipo de recurso filterOperatorSchema</span><span class="sxs-lookup"><span data-stu-id="5faf1-103">filterOperatorSchema resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5faf1-104">Descreve um operador que pode ser usado em um [filtro](synchronization-filter.md).</span><span class="sxs-lookup"><span data-stu-id="5faf1-104">Describes an operator that can be used in a [filter](synchronization-filter.md).</span></span>

## <a name="properties"></a><span data-ttu-id="5faf1-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5faf1-105">Properties</span></span>

| <span data-ttu-id="5faf1-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5faf1-106">Property</span></span>                   | <span data-ttu-id="5faf1-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="5faf1-107">Type</span></span>                      | <span data-ttu-id="5faf1-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="5faf1-108">Description</span></span>    |
|:---------------------------|:--------------------------|:---------------|
|<span data-ttu-id="5faf1-109">arity</span><span class="sxs-lookup"><span data-stu-id="5faf1-109">arity</span></span>                       |<span data-ttu-id="5faf1-110">String</span><span class="sxs-lookup"><span data-stu-id="5faf1-110">String</span></span>          |<span data-ttu-id="5faf1-111">Arity do operador.</span><span class="sxs-lookup"><span data-stu-id="5faf1-111">Arity of the operator.</span></span> <span data-ttu-id="5faf1-112">Os valores possíveis são: `Binary` e `Unary`.</span><span class="sxs-lookup"><span data-stu-id="5faf1-112">Possible values are: `Binary`, `Unary`.</span></span> <span data-ttu-id="5faf1-113">O padrão é `Binary`.</span><span class="sxs-lookup"><span data-stu-id="5faf1-113">The default is `Binary`.</span></span>|
|<span data-ttu-id="5faf1-114">multivaluedComparisonType</span><span class="sxs-lookup"><span data-stu-id="5faf1-114">multivaluedComparisonType</span></span>   |<span data-ttu-id="5faf1-115">scopeOperatorMultiValuedComparisonType</span><span class="sxs-lookup"><span data-stu-id="5faf1-115">scopeOperatorMultiValuedComparisonType</span></span>          |<span data-ttu-id="5faf1-116">Os valores possíveis são: `All` e `Any`.</span><span class="sxs-lookup"><span data-stu-id="5faf1-116">Possible values are: `All`, `Any`.</span></span> <span data-ttu-id="5faf1-117">Aplica-se somente a atributos com vários valores.</span><span class="sxs-lookup"><span data-stu-id="5faf1-117">Applies only to multivalued attributes.</span></span> <span data-ttu-id="5faf1-118">`All`significa que todos os valores devem atender à condição.</span><span class="sxs-lookup"><span data-stu-id="5faf1-118">`All` means that all values must satisfy the condition.</span></span> <span data-ttu-id="5faf1-119">`Any`significa que pelo menos um valor deve satisfazer a condição.</span><span class="sxs-lookup"><span data-stu-id="5faf1-119">`Any` means that at least one value has to satisfy the condition.</span></span> <span data-ttu-id="5faf1-120">O padrão é `All`.</span><span class="sxs-lookup"><span data-stu-id="5faf1-120">The default is `All`.</span></span>|
|<span data-ttu-id="5faf1-121">name</span><span class="sxs-lookup"><span data-stu-id="5faf1-121">name</span></span>                        |<span data-ttu-id="5faf1-122">String</span><span class="sxs-lookup"><span data-stu-id="5faf1-122">String</span></span>                     |<span data-ttu-id="5faf1-123">Nome do operador.</span><span class="sxs-lookup"><span data-stu-id="5faf1-123">Operator name.</span></span> |
|<span data-ttu-id="5faf1-124">supportedAttributeTypes</span><span class="sxs-lookup"><span data-stu-id="5faf1-124">supportedAttributeTypes</span></span>     |<span data-ttu-id="5faf1-125">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="5faf1-125">String collection</span></span>         |<span data-ttu-id="5faf1-126">Tipos de atributo suportados pelo operador.</span><span class="sxs-lookup"><span data-stu-id="5faf1-126">Attribute types supported by the operator.</span></span> <span data-ttu-id="5faf1-127">Os valores possíveis são: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.</span><span class="sxs-lookup"><span data-stu-id="5faf1-127">Possible values are: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5faf1-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5faf1-128">JSON representation</span></span>

<span data-ttu-id="5faf1-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5faf1-129">The following is a JSON representation of the resource.</span></span>

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
