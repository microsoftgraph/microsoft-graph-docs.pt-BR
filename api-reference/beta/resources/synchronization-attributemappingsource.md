---
title: Tipo de recurso attributeMappingSource
description: Define como um valor deve ser extraído (ou transformado) do objeto de origem.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 50443eb85ed87bce466e7842f46d0c457f28e216
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133235"
---
# <a name="attributemappingsource-resource-type"></a><span data-ttu-id="557a7-103">Tipo de recurso attributeMappingSource</span><span class="sxs-lookup"><span data-stu-id="557a7-103">attributeMappingSource resource type</span></span>

<span data-ttu-id="557a7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="557a7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="557a7-105">Define como um valor deve ser extraído (ou transformado) do objeto de origem.</span><span class="sxs-lookup"><span data-stu-id="557a7-105">Defines how a value should be extracted (or transformed) from the source object.</span></span> <span data-ttu-id="557a7-106">Por exemplo, pode ser um valor simples extraído de um determinado atributo no objeto de origem ou pode ser uma expressão mais complexa de concatenação/extração/substituição de cadeia de caracteres com base em vários atributos de origem.</span><span class="sxs-lookup"><span data-stu-id="557a7-106">For example, it can be a simple value taken from a given attribute on the source object, or it can be a more complex expression of string concatenation/extraction/replacement based on several source attributes.</span></span>

## <a name="properties"></a><span data-ttu-id="557a7-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="557a7-107">Properties</span></span>

| <span data-ttu-id="557a7-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="557a7-108">Property</span></span>              | <span data-ttu-id="557a7-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="557a7-109">Type</span></span>                      | <span data-ttu-id="557a7-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="557a7-110">Description</span></span>               |
|:----------------------|:--------------------------|:--------------------------|
|<span data-ttu-id="557a7-111">expressão</span><span class="sxs-lookup"><span data-stu-id="557a7-111">expression</span></span>             |<span data-ttu-id="557a7-112">String</span><span class="sxs-lookup"><span data-stu-id="557a7-112">String</span></span>                     |<span data-ttu-id="557a7-113">Representação de expressão equivalente desse **objeto attributeMappingSource.**</span><span class="sxs-lookup"><span data-stu-id="557a7-113">Equivalent expression representation of this **attributeMappingSource** object.</span></span>|
|<span data-ttu-id="557a7-114">nome</span><span class="sxs-lookup"><span data-stu-id="557a7-114">name</span></span>                   |<span data-ttu-id="557a7-115">String</span><span class="sxs-lookup"><span data-stu-id="557a7-115">String</span></span>                     |<span data-ttu-id="557a7-116">Parâmetro de nome da fonte de mapeamento.</span><span class="sxs-lookup"><span data-stu-id="557a7-116">Name parameter of the mapping source.</span></span> <span data-ttu-id="557a7-117">Dependendo do valor **da** propriedade de tipo, pode ser o nome da função, o nome do atributo de origem ou um valor constante a ser usado.</span><span class="sxs-lookup"><span data-stu-id="557a7-117">Depending on the **type** property value, this can be the name of the function, the name of the source attribute, or a constant value to be used.</span></span> |
|<span data-ttu-id="557a7-118">parameters</span><span class="sxs-lookup"><span data-stu-id="557a7-118">parameters</span></span>             |<span data-ttu-id="557a7-119">[Coleção stringKeyAttributeMappingSourceValuePair](synchronization-stringkeyattributemappingsourcevaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="557a7-119">[stringKeyAttributeMappingSourceValuePair](synchronization-stringkeyattributemappingsourcevaluepair.md) collection</span></span> | <span data-ttu-id="557a7-120">Se esse objeto representar uma função, lista os parâmetros da função.</span><span class="sxs-lookup"><span data-stu-id="557a7-120">If this object represents a function, lists function parameters.</span></span> <span data-ttu-id="557a7-121">Os parâmetros **consistem em objetos attributeMappingSource** em si, permitindo expressões complexas.</span><span class="sxs-lookup"><span data-stu-id="557a7-121">Parameters consist of **attributeMappingSource** objects themselves, allowing for complex expressions.</span></span> <span data-ttu-id="557a7-122">Se **o tipo** não `Function` for, essa propriedade será uma matriz nula/vazia.</span><span class="sxs-lookup"><span data-stu-id="557a7-122">If **type** is not `Function`, this property will be null/empty array.</span></span> |
|<span data-ttu-id="557a7-123">type</span><span class="sxs-lookup"><span data-stu-id="557a7-123">type</span></span>                   | <span data-ttu-id="557a7-124">String</span><span class="sxs-lookup"><span data-stu-id="557a7-124">String</span></span>                    |<span data-ttu-id="557a7-125">O tipo dessa fonte de mapeamento de atributos.</span><span class="sxs-lookup"><span data-stu-id="557a7-125">The type of this attribute mapping source.</span></span> <span data-ttu-id="557a7-126">Os valores possíveis são: `Attribute`, `Constant`, `Function`.</span><span class="sxs-lookup"><span data-stu-id="557a7-126">Possible values are: `Attribute`, `Constant`, `Function`.</span></span> <span data-ttu-id="557a7-127">O padrão é `Attribute`.</span><span class="sxs-lookup"><span data-stu-id="557a7-127">Default is `Attribute`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="557a7-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="557a7-128">JSON representation</span></span>

<span data-ttu-id="557a7-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="557a7-129">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attributeMappingSource"
}-->

```json
{
  "expression": "String",
  "name": "String",
  "parameters": [{"@odata.type": "microsoft.graph.stringKeyAttributeMappingSourceValuePair"}],
  "type": "String"
}
```

## <a name="json-examples"></a><span data-ttu-id="557a7-130">Exemplos JSON</span><span class="sxs-lookup"><span data-stu-id="557a7-130">JSON Examples</span></span>

<span data-ttu-id="557a7-131">Atributo simples para mapeamento de atributos</span><span class="sxs-lookup"><span data-stu-id="557a7-131">Simple attribute to attribute mapping</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attributeMappingSource"
}-->

```json
{
    "expression": "[mail]",
    "name": "mail",
    "type": "Attribute"
}
```

<span data-ttu-id="557a7-132">Expression extracting first 8 characters from the source attribute</span><span class="sxs-lookup"><span data-stu-id="557a7-132">Expression extracting first 8 characters from the source attribute</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attributeMappingSource"
}-->

```json
 {
    "expression": "Mid([userPrincipalName], 1, 8)",
    "name": "Mid",
    "parameters": [
        {
            "key": "source",
            "value": {
                "expression": "[userPrincipalName]",
                "name": "userPrincipalName",
                "parameters": [],
                "type": "Attribute"
            }
        },
        {
            "key": "start",
            "value": {
                "expression": "\"1\"",
                "name": "1",
                "parameters": [],
                "type": "Constant"
            }
        },
        {
            "key": "length",
            "value": {
                "expression": "\"8\"",
                "name": "8",
                "parameters": [],
                "type": "Constant"
            }
        }
    ],
    "type": "Function"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "attributeMappingSource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


