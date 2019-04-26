---
title: tipo de recurso attributeMappingSource
description: 'Define como um valor deve ser extraído (ou transformado) a partir do objeto Source. Por exemplo, pode ser um valor simples de um determinado atributo no objeto Source ou pode ser uma expressão mais complexa de concatenação/extração/substituição de cadeia de caracteres com base em vários atributos de origem. '
localization_priority: Normal
ms.openlocfilehash: 8b00cec8f49b914d37d252e5dc464720228bb825
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345614"
---
# <a name="attributemappingsource-resource-type"></a><span data-ttu-id="9777d-104">tipo de recurso attributeMappingSource</span><span class="sxs-lookup"><span data-stu-id="9777d-104">attributeMappingSource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9777d-105">Define como um valor deve ser extraído (ou transformado) a partir do objeto Source.</span><span class="sxs-lookup"><span data-stu-id="9777d-105">Defines how a value should be extracted (or transformed) from the source object.</span></span> <span data-ttu-id="9777d-106">Por exemplo, pode ser um valor simples de um determinado atributo no objeto Source ou pode ser uma expressão mais complexa de concatenação/extração/substituição de cadeia de caracteres com base em vários atributos de origem.</span><span class="sxs-lookup"><span data-stu-id="9777d-106">For example, it can be a simple value taken from a given attribute on the source object, or it can be a more complex expression of string concatenation/extraction/replacement based on several source attributes.</span></span> 

## <a name="properties"></a><span data-ttu-id="9777d-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9777d-107">Properties</span></span>

| <span data-ttu-id="9777d-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9777d-108">Property</span></span>              | <span data-ttu-id="9777d-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="9777d-109">Type</span></span>                      | <span data-ttu-id="9777d-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="9777d-110">Description</span></span>               |
|:----------------------|:--------------------------|:--------------------------|
|<span data-ttu-id="9777d-111">expressão</span><span class="sxs-lookup"><span data-stu-id="9777d-111">expression</span></span>             |<span data-ttu-id="9777d-112">String</span><span class="sxs-lookup"><span data-stu-id="9777d-112">String</span></span>                     |<span data-ttu-id="9777d-113">Representação de expressão equivalente deste objeto **attributeMappingSource** .</span><span class="sxs-lookup"><span data-stu-id="9777d-113">Equivalent expression representation of this **attributeMappingSource** object.</span></span>|
|<span data-ttu-id="9777d-114">name</span><span class="sxs-lookup"><span data-stu-id="9777d-114">name</span></span>                   |<span data-ttu-id="9777d-115">String</span><span class="sxs-lookup"><span data-stu-id="9777d-115">String</span></span>                     |<span data-ttu-id="9777d-116">Parâmetro Name da origem do mapeamento.</span><span class="sxs-lookup"><span data-stu-id="9777d-116">Name parameter of the mapping source.</span></span> <span data-ttu-id="9777d-117">Dependendo do valor da propriedade **Type** , isso pode ser o nome da função, o nome do atributo de origem ou um valor constante a ser usado.</span><span class="sxs-lookup"><span data-stu-id="9777d-117">Depending on the **type** property value, this can be the name of the function, the name of the source attribute, or a constant value to be used.</span></span> |
|<span data-ttu-id="9777d-118">parameters</span><span class="sxs-lookup"><span data-stu-id="9777d-118">parameters</span></span>             |<span data-ttu-id="9777d-119">coleção [stringKeyAttributeMappingSourceValuePair](synchronization-stringkeyattributemappingsourcevaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="9777d-119">[stringKeyAttributeMappingSourceValuePair](synchronization-stringkeyattributemappingsourcevaluepair.md) collection</span></span> | <span data-ttu-id="9777d-120">Se este objeto representar uma função, lista os parâmetros da função.</span><span class="sxs-lookup"><span data-stu-id="9777d-120">If this object represents a function, lists function parameters.</span></span> <span data-ttu-id="9777d-121">Os parâmetros consistem nos objetos **attributeMappingSource** , permitindo expressões complexas.</span><span class="sxs-lookup"><span data-stu-id="9777d-121">Parameters consist of **attributeMappingSource** objects themselves, allowing for complex expressions.</span></span> <span data-ttu-id="9777d-122">Se **Type** não `Function`for, esta propriedade será NULL/matriz vazia.</span><span class="sxs-lookup"><span data-stu-id="9777d-122">If **type** is not `Function`, this property will be null/empty array.</span></span> |
|<span data-ttu-id="9777d-123">tipo</span><span class="sxs-lookup"><span data-stu-id="9777d-123">type</span></span>                   | <span data-ttu-id="9777d-124">String</span><span class="sxs-lookup"><span data-stu-id="9777d-124">String</span></span>                    |<span data-ttu-id="9777d-125">O tipo desta fonte de mapeamento de atributos.</span><span class="sxs-lookup"><span data-stu-id="9777d-125">The type of this attribute mapping source.</span></span> <span data-ttu-id="9777d-126">Os valores possíveis são: `Attribute`, `Constant`, `Function`.</span><span class="sxs-lookup"><span data-stu-id="9777d-126">Possible values are: `Attribute`, `Constant`, `Function`.</span></span> <span data-ttu-id="9777d-127">O padrão é `Attribute`.</span><span class="sxs-lookup"><span data-stu-id="9777d-127">Default is `Attribute`.</span></span>| 

## <a name="json-representation"></a><span data-ttu-id="9777d-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9777d-128">JSON representation</span></span>

<span data-ttu-id="9777d-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9777d-129">The following is a JSON representation of the resource.</span></span>

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

## <a name="json-examples"></a><span data-ttu-id="9777d-130">Exemplos de JSON</span><span class="sxs-lookup"><span data-stu-id="9777d-130">JSON Examples</span></span>

<span data-ttu-id="9777d-131">Atributo simples para mapeamento de atributos</span><span class="sxs-lookup"><span data-stu-id="9777d-131">Simple attribute to attribute mapping</span></span>

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

<span data-ttu-id="9777d-132">Expressão que extrai primeiro 8 caracteres do atributo Source</span><span class="sxs-lookup"><span data-stu-id="9777d-132">Expression extracting first 8 characters from the source attribute</span></span>

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
