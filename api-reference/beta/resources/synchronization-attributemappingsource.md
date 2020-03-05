---
title: tipo de recurso attributeMappingSource
description: 'Define como um valor deve ser extraído (ou transformado) a partir do objeto Source. Por exemplo, pode ser um valor simples de um determinado atributo no objeto Source ou pode ser uma expressão mais complexa de concatenação/extração/substituição de cadeia de caracteres com base em vários atributos de origem. '
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 969f262f76f976c13f5c0a26ae53d67751b8820b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520230"
---
# <a name="attributemappingsource-resource-type"></a><span data-ttu-id="40e3f-104">tipo de recurso attributeMappingSource</span><span class="sxs-lookup"><span data-stu-id="40e3f-104">attributeMappingSource resource type</span></span>

<span data-ttu-id="40e3f-105">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="40e3f-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="40e3f-106">Define como um valor deve ser extraído (ou transformado) a partir do objeto Source.</span><span class="sxs-lookup"><span data-stu-id="40e3f-106">Defines how a value should be extracted (or transformed) from the source object.</span></span> <span data-ttu-id="40e3f-107">Por exemplo, pode ser um valor simples de um determinado atributo no objeto Source ou pode ser uma expressão mais complexa de concatenação/extração/substituição de cadeia de caracteres com base em vários atributos de origem.</span><span class="sxs-lookup"><span data-stu-id="40e3f-107">For example, it can be a simple value taken from a given attribute on the source object, or it can be a more complex expression of string concatenation/extraction/replacement based on several source attributes.</span></span> 

## <a name="properties"></a><span data-ttu-id="40e3f-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="40e3f-108">Properties</span></span>

| <span data-ttu-id="40e3f-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="40e3f-109">Property</span></span>              | <span data-ttu-id="40e3f-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="40e3f-110">Type</span></span>                      | <span data-ttu-id="40e3f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="40e3f-111">Description</span></span>               |
|:----------------------|:--------------------------|:--------------------------|
|<span data-ttu-id="40e3f-112">expressão</span><span class="sxs-lookup"><span data-stu-id="40e3f-112">expression</span></span>             |<span data-ttu-id="40e3f-113">String</span><span class="sxs-lookup"><span data-stu-id="40e3f-113">String</span></span>                     |<span data-ttu-id="40e3f-114">Representação de expressão equivalente deste objeto **attributeMappingSource** .</span><span class="sxs-lookup"><span data-stu-id="40e3f-114">Equivalent expression representation of this **attributeMappingSource** object.</span></span>|
|<span data-ttu-id="40e3f-115">nome</span><span class="sxs-lookup"><span data-stu-id="40e3f-115">name</span></span>                   |<span data-ttu-id="40e3f-116">String</span><span class="sxs-lookup"><span data-stu-id="40e3f-116">String</span></span>                     |<span data-ttu-id="40e3f-117">Parâmetro Name da origem do mapeamento.</span><span class="sxs-lookup"><span data-stu-id="40e3f-117">Name parameter of the mapping source.</span></span> <span data-ttu-id="40e3f-118">Dependendo do valor da propriedade **Type** , isso pode ser o nome da função, o nome do atributo de origem ou um valor constante a ser usado.</span><span class="sxs-lookup"><span data-stu-id="40e3f-118">Depending on the **type** property value, this can be the name of the function, the name of the source attribute, or a constant value to be used.</span></span> |
|<span data-ttu-id="40e3f-119">parameters</span><span class="sxs-lookup"><span data-stu-id="40e3f-119">parameters</span></span>             |<span data-ttu-id="40e3f-120">coleção [stringKeyAttributeMappingSourceValuePair](synchronization-stringkeyattributemappingsourcevaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="40e3f-120">[stringKeyAttributeMappingSourceValuePair](synchronization-stringkeyattributemappingsourcevaluepair.md) collection</span></span> | <span data-ttu-id="40e3f-121">Se este objeto representar uma função, lista os parâmetros da função.</span><span class="sxs-lookup"><span data-stu-id="40e3f-121">If this object represents a function, lists function parameters.</span></span> <span data-ttu-id="40e3f-122">Os parâmetros consistem nos objetos **attributeMappingSource** , permitindo expressões complexas.</span><span class="sxs-lookup"><span data-stu-id="40e3f-122">Parameters consist of **attributeMappingSource** objects themselves, allowing for complex expressions.</span></span> <span data-ttu-id="40e3f-123">Se **Type** não `Function`for, esta propriedade será NULL/matriz vazia.</span><span class="sxs-lookup"><span data-stu-id="40e3f-123">If **type** is not `Function`, this property will be null/empty array.</span></span> |
|<span data-ttu-id="40e3f-124">type</span><span class="sxs-lookup"><span data-stu-id="40e3f-124">type</span></span>                   | <span data-ttu-id="40e3f-125">String</span><span class="sxs-lookup"><span data-stu-id="40e3f-125">String</span></span>                    |<span data-ttu-id="40e3f-126">O tipo desta fonte de mapeamento de atributos.</span><span class="sxs-lookup"><span data-stu-id="40e3f-126">The type of this attribute mapping source.</span></span> <span data-ttu-id="40e3f-127">Os valores possíveis são: `Attribute`, `Constant`, `Function`.</span><span class="sxs-lookup"><span data-stu-id="40e3f-127">Possible values are: `Attribute`, `Constant`, `Function`.</span></span> <span data-ttu-id="40e3f-128">O padrão é `Attribute`.</span><span class="sxs-lookup"><span data-stu-id="40e3f-128">Default is `Attribute`.</span></span>| 

## <a name="json-representation"></a><span data-ttu-id="40e3f-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="40e3f-129">JSON representation</span></span>

<span data-ttu-id="40e3f-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="40e3f-130">The following is a JSON representation of the resource.</span></span>

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

## <a name="json-examples"></a><span data-ttu-id="40e3f-131">Exemplos de JSON</span><span class="sxs-lookup"><span data-stu-id="40e3f-131">JSON Examples</span></span>

<span data-ttu-id="40e3f-132">Atributo simples para mapeamento de atributos</span><span class="sxs-lookup"><span data-stu-id="40e3f-132">Simple attribute to attribute mapping</span></span>

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

<span data-ttu-id="40e3f-133">Expressão que extrai primeiro 8 caracteres do atributo Source</span><span class="sxs-lookup"><span data-stu-id="40e3f-133">Expression extracting first 8 characters from the source attribute</span></span>

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
