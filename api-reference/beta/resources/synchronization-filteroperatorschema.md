---
title: tipo de recurso filterOperatorSchema
description: Descreve um operador que pode ser usado em um filtro.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 2e80b80a7f37af8b86dfd3925fe268dba89cea17
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/10/2020
ms.locfileid: "43217809"
---
# <a name="filteroperatorschema-resource-type"></a><span data-ttu-id="4845f-103">tipo de recurso filterOperatorSchema</span><span class="sxs-lookup"><span data-stu-id="4845f-103">filterOperatorSchema resource type</span></span>

<span data-ttu-id="4845f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4845f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4845f-105">Descreve um operador que pode ser usado em um [filtro](synchronization-filter.md).</span><span class="sxs-lookup"><span data-stu-id="4845f-105">Describes an operator that can be used in a [filter](synchronization-filter.md).</span></span>

## <a name="properties"></a><span data-ttu-id="4845f-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4845f-106">Properties</span></span>

| <span data-ttu-id="4845f-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4845f-107">Property</span></span>                   | <span data-ttu-id="4845f-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="4845f-108">Type</span></span>                      | <span data-ttu-id="4845f-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="4845f-109">Description</span></span>    |
|:---------------------------|:--------------------------|:---------------|
|<span data-ttu-id="4845f-110">arity</span><span class="sxs-lookup"><span data-stu-id="4845f-110">arity</span></span>                       |<span data-ttu-id="4845f-111">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="4845f-111">String</span></span>          |<span data-ttu-id="4845f-112">Arity do operador.</span><span class="sxs-lookup"><span data-stu-id="4845f-112">Arity of the operator.</span></span> <span data-ttu-id="4845f-113">Os valores possíveis são: `Binary` e `Unary`.</span><span class="sxs-lookup"><span data-stu-id="4845f-113">Possible values are: `Binary`, `Unary`.</span></span> <span data-ttu-id="4845f-114">O padrão é `Binary`.</span><span class="sxs-lookup"><span data-stu-id="4845f-114">The default is `Binary`.</span></span>|
|<span data-ttu-id="4845f-115">multivaluedComparisonType</span><span class="sxs-lookup"><span data-stu-id="4845f-115">multivaluedComparisonType</span></span>   |<span data-ttu-id="4845f-116">scopeOperatorMultiValuedComparisonType</span><span class="sxs-lookup"><span data-stu-id="4845f-116">scopeOperatorMultiValuedComparisonType</span></span>          |<span data-ttu-id="4845f-117">Os valores possíveis são: `All` e `Any`.</span><span class="sxs-lookup"><span data-stu-id="4845f-117">Possible values are: `All`, `Any`.</span></span> <span data-ttu-id="4845f-118">Aplica-se somente a atributos com vários valores.</span><span class="sxs-lookup"><span data-stu-id="4845f-118">Applies only to multivalued attributes.</span></span> <span data-ttu-id="4845f-119">`All`significa que todos os valores devem atender à condição.</span><span class="sxs-lookup"><span data-stu-id="4845f-119">`All` means that all values must satisfy the condition.</span></span> <span data-ttu-id="4845f-120">`Any`significa que pelo menos um valor deve satisfazer a condição.</span><span class="sxs-lookup"><span data-stu-id="4845f-120">`Any` means that at least one value has to satisfy the condition.</span></span> <span data-ttu-id="4845f-121">O padrão é `All`.</span><span class="sxs-lookup"><span data-stu-id="4845f-121">The default is `All`.</span></span>|
|<span data-ttu-id="4845f-122">nome</span><span class="sxs-lookup"><span data-stu-id="4845f-122">name</span></span>                        |<span data-ttu-id="4845f-123">String</span><span class="sxs-lookup"><span data-stu-id="4845f-123">String</span></span>                     |<span data-ttu-id="4845f-124">Nome do operador.</span><span class="sxs-lookup"><span data-stu-id="4845f-124">Operator name.</span></span> |
|<span data-ttu-id="4845f-125">supportedAttributeTypes</span><span class="sxs-lookup"><span data-stu-id="4845f-125">supportedAttributeTypes</span></span>     |<span data-ttu-id="4845f-126">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="4845f-126">String collection</span></span>         |<span data-ttu-id="4845f-127">Tipos de atributo suportados pelo operador.</span><span class="sxs-lookup"><span data-stu-id="4845f-127">Attribute types supported by the operator.</span></span> <span data-ttu-id="4845f-128">Os valores possíveis são: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.</span><span class="sxs-lookup"><span data-stu-id="4845f-128">Possible values are: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4845f-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4845f-129">JSON representation</span></span>

<span data-ttu-id="4845f-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4845f-130">The following is a JSON representation of the resource.</span></span>

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
