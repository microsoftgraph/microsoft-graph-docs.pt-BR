---
title: tipo de recurso de attributeMappingSource
description: 'Define como um valor deve ser extraída (ou transformados) do objeto de origem. Por exemplo, pode ser um valor simple tirado de um determinado atributo no objeto de origem, ou pode ser uma expressão mais complexa de cadeia de caracteres concatenação/extração/substituição com base em vários atributos de fonte. '
localization_priority: Normal
ms.openlocfilehash: 1d15cd82c0a58ac8bdd3ac5805abc166322f27fe
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510404"
---
# <a name="attributemappingsource-resource-type"></a><span data-ttu-id="4a138-104">tipo de recurso de attributeMappingSource</span><span class="sxs-lookup"><span data-stu-id="4a138-104">attributeMappingSource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4a138-105">Define como um valor deve ser extraída (ou transformados) do objeto de origem.</span><span class="sxs-lookup"><span data-stu-id="4a138-105">Defines how a value should be extracted (or transformed) from the source object.</span></span> <span data-ttu-id="4a138-106">Por exemplo, pode ser um valor simple tirado de um determinado atributo no objeto de origem, ou pode ser uma expressão mais complexa de cadeia de caracteres concatenação/extração/substituição com base em vários atributos de fonte.</span><span class="sxs-lookup"><span data-stu-id="4a138-106">For example, it can be a simple value taken from a given attribute on the source object, or it can be a more complex expression of string concatenation/extraction/replacement based on several source attributes.</span></span> 

## <a name="properties"></a><span data-ttu-id="4a138-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4a138-107">Properties</span></span>

| <span data-ttu-id="4a138-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4a138-108">Property</span></span>              | <span data-ttu-id="4a138-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="4a138-109">Type</span></span>                      | <span data-ttu-id="4a138-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="4a138-110">Description</span></span>               |
|:----------------------|:--------------------------|:--------------------------|
|<span data-ttu-id="4a138-111">expressão</span><span class="sxs-lookup"><span data-stu-id="4a138-111">expression</span></span>             |<span data-ttu-id="4a138-112">String</span><span class="sxs-lookup"><span data-stu-id="4a138-112">String</span></span>                     |<span data-ttu-id="4a138-113">Representação de expressão equivalente deste objeto **attributeMappingSource** .</span><span class="sxs-lookup"><span data-stu-id="4a138-113">Equivalent expression representation of this **attributeMappingSource** object.</span></span>|
|<span data-ttu-id="4a138-114">name</span><span class="sxs-lookup"><span data-stu-id="4a138-114">name</span></span>                   |<span data-ttu-id="4a138-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4a138-115">String</span></span>                     |<span data-ttu-id="4a138-116">Parâmetro nome da fonte de mapeamento.</span><span class="sxs-lookup"><span data-stu-id="4a138-116">Name parameter of the mapping source.</span></span> <span data-ttu-id="4a138-117">Dependendo do valor da propriedade **type** , isso pode ser o nome da função, o nome do atributo de origem, ou um valor de constante a ser usado.</span><span class="sxs-lookup"><span data-stu-id="4a138-117">Depending on the **type** property value, this can be the name of the function, the name of the source attribute, or a constant value to be used.</span></span> |
|<span data-ttu-id="4a138-118">parâmetros</span><span class="sxs-lookup"><span data-stu-id="4a138-118">parameters</span></span>             |<span data-ttu-id="4a138-119">coleção [stringKeyAttributeMappingSourceValuePair](synchronization-stringkeyattributemappingsourcevaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="4a138-119">[stringKeyAttributeMappingSourceValuePair](synchronization-stringkeyattributemappingsourcevaluepair.md) collection</span></span> | <span data-ttu-id="4a138-120">Se esse objeto representa uma função, lista os parâmetros da função.</span><span class="sxs-lookup"><span data-stu-id="4a138-120">If this object represents a function, lists function parameters.</span></span> <span data-ttu-id="4a138-121">Parâmetros consistem em objetos **attributeMappingSource** sozinhos, permitindo expressões complexas.</span><span class="sxs-lookup"><span data-stu-id="4a138-121">Parameters consist of **attributeMappingSource** objects themselves, allowing for complex expressions.</span></span> <span data-ttu-id="4a138-122">Se **tipo** não for `Function`, essa propriedade será null/vazio matriz.</span><span class="sxs-lookup"><span data-stu-id="4a138-122">If **type** is not `Function`, this property will be null/empty array.</span></span> |
|<span data-ttu-id="4a138-123">type</span><span class="sxs-lookup"><span data-stu-id="4a138-123">type</span></span>                   | <span data-ttu-id="4a138-124">String</span><span class="sxs-lookup"><span data-stu-id="4a138-124">String</span></span>                    |<span data-ttu-id="4a138-125">O tipo de fonte de mapeamento este atributo.</span><span class="sxs-lookup"><span data-stu-id="4a138-125">The type of this attribute mapping source.</span></span> <span data-ttu-id="4a138-126">Os valores possíveis são: `Attribute`, `Constant`, `Function`.</span><span class="sxs-lookup"><span data-stu-id="4a138-126">Possible values are: `Attribute`, `Constant`, `Function`.</span></span> <span data-ttu-id="4a138-127">O padrão é `Attribute`.</span><span class="sxs-lookup"><span data-stu-id="4a138-127">Default is `Attribute`.</span></span>| 

## <a name="json-representation"></a><span data-ttu-id="4a138-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4a138-128">JSON representation</span></span>

<span data-ttu-id="4a138-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4a138-129">The following is a JSON representation of the resource.</span></span>

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

## <a name="json-examples"></a><span data-ttu-id="4a138-130">Exemplos JSON</span><span class="sxs-lookup"><span data-stu-id="4a138-130">JSON Examples</span></span>

<span data-ttu-id="4a138-131">Mapeamento de atributo para o atributo simples</span><span class="sxs-lookup"><span data-stu-id="4a138-131">Simple attribute to attribute mapping</span></span>

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

<span data-ttu-id="4a138-132">Expressão extraindo 8 primeiros caracteres do atributo de origem</span><span class="sxs-lookup"><span data-stu-id="4a138-132">Expression extracting first 8 characters from the source attribute</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-attributemappingsource.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
