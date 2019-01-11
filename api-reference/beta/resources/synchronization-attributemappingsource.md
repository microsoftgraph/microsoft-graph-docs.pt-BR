---
title: tipo de recurso de attributeMappingSource
description: 'Define como um valor deve ser extraída (ou transformados) do objeto de origem. Por exemplo, pode ser um valor simple tirado de um determinado atributo no objeto de origem, ou pode ser uma expressão mais complexa de cadeia de caracteres concatenação/extração/substituição com base em vários atributos de fonte. '
localization_priority: Normal
ms.openlocfilehash: a7c1493f27f34230d4305fe95b2d2f03a5ad25e2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27825008"
---
# <a name="attributemappingsource-resource-type"></a><span data-ttu-id="ec68e-104">tipo de recurso de attributeMappingSource</span><span class="sxs-lookup"><span data-stu-id="ec68e-104">attributeMappingSource resource type</span></span>

> <span data-ttu-id="ec68e-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ec68e-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ec68e-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ec68e-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ec68e-107">Define como um valor deve ser extraída (ou transformados) do objeto de origem.</span><span class="sxs-lookup"><span data-stu-id="ec68e-107">Defines how a value should be extracted (or transformed) from the source object.</span></span> <span data-ttu-id="ec68e-108">Por exemplo, pode ser um valor simple tirado de um determinado atributo no objeto de origem, ou pode ser uma expressão mais complexa de cadeia de caracteres concatenação/extração/substituição com base em vários atributos de fonte.</span><span class="sxs-lookup"><span data-stu-id="ec68e-108">For example, it can be a simple value taken from a given attribute on the source object, or it can be a more complex expression of string concatenation/extraction/replacement based on several source attributes.</span></span> 

## <a name="properties"></a><span data-ttu-id="ec68e-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ec68e-109">Properties</span></span>

| <span data-ttu-id="ec68e-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ec68e-110">Property</span></span>              | <span data-ttu-id="ec68e-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="ec68e-111">Type</span></span>                      | <span data-ttu-id="ec68e-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="ec68e-112">Description</span></span>               |
|:----------------------|:--------------------------|:--------------------------|
|<span data-ttu-id="ec68e-113">expressão</span><span class="sxs-lookup"><span data-stu-id="ec68e-113">expression</span></span>             |<span data-ttu-id="ec68e-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ec68e-114">String</span></span>                     |<span data-ttu-id="ec68e-115">Representação de expressão equivalente deste objeto **attributeMappingSource** .</span><span class="sxs-lookup"><span data-stu-id="ec68e-115">Equivalent expression representation of this **attributeMappingSource** object.</span></span>|
|<span data-ttu-id="ec68e-116">name</span><span class="sxs-lookup"><span data-stu-id="ec68e-116">name</span></span>                   |<span data-ttu-id="ec68e-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ec68e-117">String</span></span>                     |<span data-ttu-id="ec68e-118">Parâmetro nome da fonte de mapeamento.</span><span class="sxs-lookup"><span data-stu-id="ec68e-118">Name parameter of the mapping source.</span></span> <span data-ttu-id="ec68e-119">Dependendo do valor da propriedade **type** , isso pode ser o nome da função, o nome do atributo de origem, ou um valor de constante a ser usado.</span><span class="sxs-lookup"><span data-stu-id="ec68e-119">Depending on the **type** property value, this can be the name of the function, the name of the source attribute, or a constant value to be used.</span></span> |
|<span data-ttu-id="ec68e-120">parâmetros</span><span class="sxs-lookup"><span data-stu-id="ec68e-120">parameters</span></span>             |<span data-ttu-id="ec68e-121">coleção [stringKeyAttributeMappingSourceValuePair](synchronization-stringkeyattributemappingsourcevaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="ec68e-121">[stringKeyAttributeMappingSourceValuePair](synchronization-stringkeyattributemappingsourcevaluepair.md) collection</span></span> | <span data-ttu-id="ec68e-122">Se esse objeto representa uma função, lista os parâmetros da função.</span><span class="sxs-lookup"><span data-stu-id="ec68e-122">If this object represents a function, lists function parameters.</span></span> <span data-ttu-id="ec68e-123">Parâmetros consistem em objetos **attributeMappingSource** sozinhos, permitindo expressões complexas.</span><span class="sxs-lookup"><span data-stu-id="ec68e-123">Parameters consist of **attributeMappingSource** objects themselves, allowing for complex expressions.</span></span> <span data-ttu-id="ec68e-124">Se **tipo** não for `Function`, essa propriedade será null/vazio matriz.</span><span class="sxs-lookup"><span data-stu-id="ec68e-124">If **type** is not `Function`, this property will be null/empty array.</span></span> |
|<span data-ttu-id="ec68e-125">type</span><span class="sxs-lookup"><span data-stu-id="ec68e-125">type</span></span>                   | <span data-ttu-id="ec68e-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ec68e-126">String</span></span>                    |<span data-ttu-id="ec68e-127">O tipo de fonte de mapeamento este atributo.</span><span class="sxs-lookup"><span data-stu-id="ec68e-127">The type of this attribute mapping source.</span></span> <span data-ttu-id="ec68e-128">Os valores possíveis são: `Attribute`, `Constant`, `Function`.</span><span class="sxs-lookup"><span data-stu-id="ec68e-128">Possible values are: `Attribute`, `Constant`, `Function`.</span></span> <span data-ttu-id="ec68e-129">O padrão é `Attribute`.</span><span class="sxs-lookup"><span data-stu-id="ec68e-129">Default is `Attribute`.</span></span>| 

## <a name="json-representation"></a><span data-ttu-id="ec68e-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ec68e-130">JSON representation</span></span>

<span data-ttu-id="ec68e-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ec68e-131">The following is a JSON representation of the resource.</span></span>

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

## <a name="json-examples"></a><span data-ttu-id="ec68e-132">Exemplos JSON</span><span class="sxs-lookup"><span data-stu-id="ec68e-132">JSON Examples</span></span>

<span data-ttu-id="ec68e-133">Mapeamento de atributo para o atributo simples</span><span class="sxs-lookup"><span data-stu-id="ec68e-133">Simple attribute to attribute mapping</span></span>

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

<span data-ttu-id="ec68e-134">Expressão extraindo 8 primeiros caracteres do atributo de origem</span><span class="sxs-lookup"><span data-stu-id="ec68e-134">Expression extracting first 8 characters from the source attribute</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "attributeMappingSource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
