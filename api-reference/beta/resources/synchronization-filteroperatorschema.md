---
title: tipo de recurso filterOperatorSchema
description: Descreve um operador que pode ser usado em um filtro.
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 868ecf1e57deb624ab8b276d3f10cd39176efa5b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520167"
---
# <a name="filteroperatorschema-resource-type"></a><span data-ttu-id="9940d-103">tipo de recurso filterOperatorSchema</span><span class="sxs-lookup"><span data-stu-id="9940d-103">filterOperatorSchema resource type</span></span>

<span data-ttu-id="9940d-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="9940d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9940d-105">Descreve um operador que pode ser usado em um [filtro](synchronization-filter.md).</span><span class="sxs-lookup"><span data-stu-id="9940d-105">Describes an operator that can be used in a [filter](synchronization-filter.md).</span></span>

## <a name="properties"></a><span data-ttu-id="9940d-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9940d-106">Properties</span></span>

| <span data-ttu-id="9940d-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9940d-107">Property</span></span>                   | <span data-ttu-id="9940d-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="9940d-108">Type</span></span>                      | <span data-ttu-id="9940d-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="9940d-109">Description</span></span>    |
|:---------------------------|:--------------------------|:---------------|
|<span data-ttu-id="9940d-110">arity</span><span class="sxs-lookup"><span data-stu-id="9940d-110">arity</span></span>                       |<span data-ttu-id="9940d-111">String</span><span class="sxs-lookup"><span data-stu-id="9940d-111">String</span></span>          |<span data-ttu-id="9940d-112">Arity do operador.</span><span class="sxs-lookup"><span data-stu-id="9940d-112">Arity of the operator.</span></span> <span data-ttu-id="9940d-113">Os valores possíveis são: `Binary` e `Unary`.</span><span class="sxs-lookup"><span data-stu-id="9940d-113">Possible values are: `Binary`, `Unary`.</span></span> <span data-ttu-id="9940d-114">O padrão é `Binary`.</span><span class="sxs-lookup"><span data-stu-id="9940d-114">The default is `Binary`.</span></span>|
|<span data-ttu-id="9940d-115">multivaluedComparisonType</span><span class="sxs-lookup"><span data-stu-id="9940d-115">multivaluedComparisonType</span></span>   |<span data-ttu-id="9940d-116">scopeOperatorMultiValuedComparisonType</span><span class="sxs-lookup"><span data-stu-id="9940d-116">scopeOperatorMultiValuedComparisonType</span></span>          |<span data-ttu-id="9940d-117">Os valores possíveis são: `All` e `Any`.</span><span class="sxs-lookup"><span data-stu-id="9940d-117">Possible values are: `All`, `Any`.</span></span> <span data-ttu-id="9940d-118">Aplica-se somente a atributos com vários valores.</span><span class="sxs-lookup"><span data-stu-id="9940d-118">Applies only to multivalued attributes.</span></span> <span data-ttu-id="9940d-119">`All`significa que todos os valores devem atender à condição.</span><span class="sxs-lookup"><span data-stu-id="9940d-119">`All` means that all values must satisfy the condition.</span></span> <span data-ttu-id="9940d-120">`Any`significa que pelo menos um valor deve satisfazer a condição.</span><span class="sxs-lookup"><span data-stu-id="9940d-120">`Any` means that at least one value has to satisfy the condition.</span></span> <span data-ttu-id="9940d-121">O padrão é `All`.</span><span class="sxs-lookup"><span data-stu-id="9940d-121">The default is `All`.</span></span>|
|<span data-ttu-id="9940d-122">nome</span><span class="sxs-lookup"><span data-stu-id="9940d-122">name</span></span>                        |<span data-ttu-id="9940d-123">String</span><span class="sxs-lookup"><span data-stu-id="9940d-123">String</span></span>                     |<span data-ttu-id="9940d-124">Nome do operador.</span><span class="sxs-lookup"><span data-stu-id="9940d-124">Operator name.</span></span> |
|<span data-ttu-id="9940d-125">supportedAttributeTypes</span><span class="sxs-lookup"><span data-stu-id="9940d-125">supportedAttributeTypes</span></span>     |<span data-ttu-id="9940d-126">String collection</span><span class="sxs-lookup"><span data-stu-id="9940d-126">String collection</span></span>         |<span data-ttu-id="9940d-127">Tipos de atributo suportados pelo operador.</span><span class="sxs-lookup"><span data-stu-id="9940d-127">Attribute types supported by the operator.</span></span> <span data-ttu-id="9940d-128">Os valores possíveis são: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.</span><span class="sxs-lookup"><span data-stu-id="9940d-128">Possible values are: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9940d-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9940d-129">JSON representation</span></span>

<span data-ttu-id="9940d-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9940d-130">The following is a JSON representation of the resource.</span></span>

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
