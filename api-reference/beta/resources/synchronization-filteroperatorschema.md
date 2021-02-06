---
title: Tipo de recurso filterOperatorSchema
description: Descreve um operador que pode ser usado em um filtro.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 1128b12ffcadd36f2fdd2f34d27f95d973cdfd9d
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131884"
---
# <a name="filteroperatorschema-resource-type"></a><span data-ttu-id="612ca-103">Tipo de recurso filterOperatorSchema</span><span class="sxs-lookup"><span data-stu-id="612ca-103">filterOperatorSchema resource type</span></span>

<span data-ttu-id="612ca-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="612ca-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="612ca-105">Descreve um operador que pode ser usado em um [filtro.](synchronization-filter.md)</span><span class="sxs-lookup"><span data-stu-id="612ca-105">Describes an operator that can be used in a [filter](synchronization-filter.md).</span></span>

## <a name="properties"></a><span data-ttu-id="612ca-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="612ca-106">Properties</span></span>

| <span data-ttu-id="612ca-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="612ca-107">Property</span></span>                   | <span data-ttu-id="612ca-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="612ca-108">Type</span></span>                      | <span data-ttu-id="612ca-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="612ca-109">Description</span></span>    |
|:---------------------------|:--------------------------|:---------------|
|<span data-ttu-id="612ca-110">arity</span><span class="sxs-lookup"><span data-stu-id="612ca-110">arity</span></span>                       |<span data-ttu-id="612ca-111">String</span><span class="sxs-lookup"><span data-stu-id="612ca-111">String</span></span>          |<span data-ttu-id="612ca-112">A personalidade do operador.</span><span class="sxs-lookup"><span data-stu-id="612ca-112">Arity of the operator.</span></span> <span data-ttu-id="612ca-113">Os valores possíveis são: `Binary` e `Unary`.</span><span class="sxs-lookup"><span data-stu-id="612ca-113">Possible values are: `Binary`, `Unary`.</span></span> <span data-ttu-id="612ca-114">O padrão é `Binary` .</span><span class="sxs-lookup"><span data-stu-id="612ca-114">The default is `Binary`.</span></span>|
|<span data-ttu-id="612ca-115">multivaluedComparisonType</span><span class="sxs-lookup"><span data-stu-id="612ca-115">multivaluedComparisonType</span></span>   |<span data-ttu-id="612ca-116">scopeOperatorMultiValuedComparisonType</span><span class="sxs-lookup"><span data-stu-id="612ca-116">scopeOperatorMultiValuedComparisonType</span></span>          |<span data-ttu-id="612ca-117">Os valores possíveis são: `All` e `Any`.</span><span class="sxs-lookup"><span data-stu-id="612ca-117">Possible values are: `All`, `Any`.</span></span> <span data-ttu-id="612ca-118">Aplica-se somente a atributos de múltiplos valores.</span><span class="sxs-lookup"><span data-stu-id="612ca-118">Applies only to multivalued attributes.</span></span> <span data-ttu-id="612ca-119">`All` significa que todos os valores devem satisfazer a condição.</span><span class="sxs-lookup"><span data-stu-id="612ca-119">`All` means that all values must satisfy the condition.</span></span> <span data-ttu-id="612ca-120">`Any` significa que pelo menos um valor deve satisfazer a condição.</span><span class="sxs-lookup"><span data-stu-id="612ca-120">`Any` means that at least one value has to satisfy the condition.</span></span> <span data-ttu-id="612ca-121">O padrão é `All` .</span><span class="sxs-lookup"><span data-stu-id="612ca-121">The default is `All`.</span></span>|
|<span data-ttu-id="612ca-122">nome</span><span class="sxs-lookup"><span data-stu-id="612ca-122">name</span></span>                        |<span data-ttu-id="612ca-123">String</span><span class="sxs-lookup"><span data-stu-id="612ca-123">String</span></span>                     |<span data-ttu-id="612ca-124">Nome do operador.</span><span class="sxs-lookup"><span data-stu-id="612ca-124">Operator name.</span></span> |
|<span data-ttu-id="612ca-125">supportedAttributeTypes</span><span class="sxs-lookup"><span data-stu-id="612ca-125">supportedAttributeTypes</span></span>     |<span data-ttu-id="612ca-126">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="612ca-126">String collection</span></span>         |<span data-ttu-id="612ca-127">Tipos de atributo suportados pelo operador.</span><span class="sxs-lookup"><span data-stu-id="612ca-127">Attribute types supported by the operator.</span></span> <span data-ttu-id="612ca-128">Os valores possíveis são: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.</span><span class="sxs-lookup"><span data-stu-id="612ca-128">Possible values are: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="612ca-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="612ca-129">JSON representation</span></span>

<span data-ttu-id="612ca-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="612ca-130">The following is a JSON representation of the resource.</span></span>

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


