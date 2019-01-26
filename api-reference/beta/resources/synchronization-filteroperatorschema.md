---
title: tipo de recurso de filterOperatorSchema
description: Descreve um operador que pode ser usado em um filtro.
localization_priority: Normal
ms.openlocfilehash: 366e00b5d21efeaf67e3e799c5b1c2412a68e268
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573674"
---
# <a name="filteroperatorschema-resource-type"></a><span data-ttu-id="00529-103">tipo de recurso de filterOperatorSchema</span><span class="sxs-lookup"><span data-stu-id="00529-103">filterOperatorSchema resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="00529-104">Descreve um operador que pode ser usado em um [filtro](synchronization-filter.md).</span><span class="sxs-lookup"><span data-stu-id="00529-104">Describes an operator that can be used in a [filter](synchronization-filter.md).</span></span>

## <a name="properties"></a><span data-ttu-id="00529-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="00529-105">Properties</span></span>

| <span data-ttu-id="00529-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="00529-106">Property</span></span>                   | <span data-ttu-id="00529-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="00529-107">Type</span></span>                      | <span data-ttu-id="00529-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="00529-108">Description</span></span>    |
|:---------------------------|:--------------------------|:---------------|
|<span data-ttu-id="00529-109">aridade</span><span class="sxs-lookup"><span data-stu-id="00529-109">arity</span></span>                       | <span data-ttu-id="00529-110">microsoft.graph.scopeOperatorType</span><span class="sxs-lookup"><span data-stu-id="00529-110">microsoft.graph.scopeOperatorType</span></span>         |<span data-ttu-id="00529-111">Aridade do operador.</span><span class="sxs-lookup"><span data-stu-id="00529-111">Arity of the operator.</span></span> <span data-ttu-id="00529-112">Os valores possíveis são: `Binary` e `Unary`.</span><span class="sxs-lookup"><span data-stu-id="00529-112">Possible values are: `Binary`, `Unary`.</span></span> <span data-ttu-id="00529-113">O padrão é `Binary`.</span><span class="sxs-lookup"><span data-stu-id="00529-113">The default is `Binary`.</span></span>|
|<span data-ttu-id="00529-114">multivaluedComparisonType</span><span class="sxs-lookup"><span data-stu-id="00529-114">multivaluedComparisonType</span></span>   | <span data-ttu-id="00529-115">microsoft.graph.scopeOperatorMultiValuedComparisonType</span><span class="sxs-lookup"><span data-stu-id="00529-115">microsoft.graph.scopeOperatorMultiValuedComparisonType</span></span>          |<span data-ttu-id="00529-116">Os valores possíveis são: `All` e `Any`.</span><span class="sxs-lookup"><span data-stu-id="00529-116">Possible values are: `All`, `Any`.</span></span> <span data-ttu-id="00529-117">Só se aplica aos atributos de valores múltiplos.</span><span class="sxs-lookup"><span data-stu-id="00529-117">Applies only to multivalued attributes.</span></span> <span data-ttu-id="00529-118">`All`significa que todos os valores devem satisfazer a condição.</span><span class="sxs-lookup"><span data-stu-id="00529-118">`All` means that all values must satisfy the condition.</span></span> <span data-ttu-id="00529-119">`Any`significa que pelo menos um valor tem que satisfazer a condição.</span><span class="sxs-lookup"><span data-stu-id="00529-119">`Any` means that at least one value has to satisfy the condition.</span></span> <span data-ttu-id="00529-120">O padrão é `All`.</span><span class="sxs-lookup"><span data-stu-id="00529-120">The default is `All`.</span></span>|
|<span data-ttu-id="00529-121">supportedAttributeTypes</span><span class="sxs-lookup"><span data-stu-id="00529-121">supportedAttributeTypes</span></span>     | <span data-ttu-id="00529-122">coleção attributeType</span><span class="sxs-lookup"><span data-stu-id="00529-122">attributeType collection</span></span>         |<span data-ttu-id="00529-123">Tipos suportados pela operadora de atributo.</span><span class="sxs-lookup"><span data-stu-id="00529-123">Attribute types supported by the operator.</span></span> <span data-ttu-id="00529-124">Os valores possíveis são: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.</span><span class="sxs-lookup"><span data-stu-id="00529-124">Possible values are: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="00529-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="00529-125">JSON representation</span></span>

<span data-ttu-id="00529-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="00529-126">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.filterOperatorSchema"
}-->

```json
{
  "arity": "microsoft.graph.scopeOperatorType",
  "multivaluedComparisonType": "microsoft.graph.scopeOperatorMultiValuedComparisonType",  
  "supportedAttributeTypes": ["attributeType"]
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
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-filteroperatorschema.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
