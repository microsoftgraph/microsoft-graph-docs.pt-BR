---
title: tipo de recurso de filterOperatorSchema
description: Descreve um operador que pode ser usado em um filtro.
localization_priority: Normal
ms.openlocfilehash: 0d26fb58b77369b70ab185fa8ad5214d6b6c1e71
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27848276"
---
# <a name="filteroperatorschema-resource-type"></a><span data-ttu-id="a72f1-103">tipo de recurso de filterOperatorSchema</span><span class="sxs-lookup"><span data-stu-id="a72f1-103">filterOperatorSchema resource type</span></span>

> <span data-ttu-id="a72f1-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a72f1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a72f1-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a72f1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a72f1-106">Descreve um operador que pode ser usado em um [filtro](synchronization-filter.md).</span><span class="sxs-lookup"><span data-stu-id="a72f1-106">Describes an operator that can be used in a [filter](synchronization-filter.md).</span></span>

## <a name="properties"></a><span data-ttu-id="a72f1-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a72f1-107">Properties</span></span>

| <span data-ttu-id="a72f1-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a72f1-108">Property</span></span>                   | <span data-ttu-id="a72f1-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="a72f1-109">Type</span></span>                      | <span data-ttu-id="a72f1-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a72f1-110">Description</span></span>    |
|:---------------------------|:--------------------------|:---------------|
|<span data-ttu-id="a72f1-111">aridade</span><span class="sxs-lookup"><span data-stu-id="a72f1-111">arity</span></span>                       |<span data-ttu-id="a72f1-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a72f1-112">String</span></span>          |<span data-ttu-id="a72f1-113">Aridade do operador.</span><span class="sxs-lookup"><span data-stu-id="a72f1-113">Arity of the operator.</span></span> <span data-ttu-id="a72f1-114">Os valores possíveis são: `Binary` e `Unary`.</span><span class="sxs-lookup"><span data-stu-id="a72f1-114">Possible values are: `Binary`, `Unary`.</span></span> <span data-ttu-id="a72f1-115">O padrão é `Binary`.</span><span class="sxs-lookup"><span data-stu-id="a72f1-115">The default is `Binary`.</span></span>|
|<span data-ttu-id="a72f1-116">multivaluedComparisonType</span><span class="sxs-lookup"><span data-stu-id="a72f1-116">multivaluedComparisonType</span></span>   |<span data-ttu-id="a72f1-117">scopeOperatorMultiValuedComparisonType</span><span class="sxs-lookup"><span data-stu-id="a72f1-117">scopeOperatorMultiValuedComparisonType</span></span>          |<span data-ttu-id="a72f1-118">Os valores possíveis são: `All` e `Any`.</span><span class="sxs-lookup"><span data-stu-id="a72f1-118">Possible values are: `All`, `Any`.</span></span> <span data-ttu-id="a72f1-119">Só se aplica aos atributos de valores múltiplos.</span><span class="sxs-lookup"><span data-stu-id="a72f1-119">Applies only to multivalued attributes.</span></span> <span data-ttu-id="a72f1-120">`All`significa que todos os valores devem satisfazer a condição.</span><span class="sxs-lookup"><span data-stu-id="a72f1-120">`All` means that all values must satisfy the condition.</span></span> <span data-ttu-id="a72f1-121">`Any`significa que pelo menos um valor tem que satisfazer a condição.</span><span class="sxs-lookup"><span data-stu-id="a72f1-121">`Any` means that at least one value has to satisfy the condition.</span></span> <span data-ttu-id="a72f1-122">O padrão é `All`.</span><span class="sxs-lookup"><span data-stu-id="a72f1-122">The default is `All`.</span></span>|
|<span data-ttu-id="a72f1-123">name</span><span class="sxs-lookup"><span data-stu-id="a72f1-123">name</span></span>                        |<span data-ttu-id="a72f1-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a72f1-124">String</span></span>                     |<span data-ttu-id="a72f1-125">Nome do operador.</span><span class="sxs-lookup"><span data-stu-id="a72f1-125">Operator name.</span></span> |
|<span data-ttu-id="a72f1-126">supportedAttributeTypes</span><span class="sxs-lookup"><span data-stu-id="a72f1-126">supportedAttributeTypes</span></span>     |<span data-ttu-id="a72f1-127">String collection</span><span class="sxs-lookup"><span data-stu-id="a72f1-127">String collection</span></span>         |<span data-ttu-id="a72f1-128">Tipos suportados pela operadora de atributo.</span><span class="sxs-lookup"><span data-stu-id="a72f1-128">Attribute types supported by the operator.</span></span> <span data-ttu-id="a72f1-129">Os valores possíveis são: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.</span><span class="sxs-lookup"><span data-stu-id="a72f1-129">Possible values are: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a72f1-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a72f1-130">JSON representation</span></span>

<span data-ttu-id="a72f1-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a72f1-131">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "filterOperatorSchema resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
