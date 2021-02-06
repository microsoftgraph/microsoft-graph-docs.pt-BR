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
# <a name="attributemappingsource-resource-type"></a>Tipo de recurso attributeMappingSource

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Define como um valor deve ser extraído (ou transformado) do objeto de origem. Por exemplo, pode ser um valor simples extraído de um determinado atributo no objeto de origem ou pode ser uma expressão mais complexa de concatenação/extração/substituição de cadeia de caracteres com base em vários atributos de origem.

## <a name="properties"></a>Propriedades

| Propriedade              | Tipo                      | Descrição               |
|:----------------------|:--------------------------|:--------------------------|
|expressão             |String                     |Representação de expressão equivalente desse **objeto attributeMappingSource.**|
|nome                   |String                     |Parâmetro de nome da fonte de mapeamento. Dependendo do valor **da** propriedade de tipo, pode ser o nome da função, o nome do atributo de origem ou um valor constante a ser usado. |
|parameters             |[Coleção stringKeyAttributeMappingSourceValuePair](synchronization-stringkeyattributemappingsourcevaluepair.md) | Se esse objeto representar uma função, lista os parâmetros da função. Os parâmetros **consistem em objetos attributeMappingSource** em si, permitindo expressões complexas. Se **o tipo** não `Function` for, essa propriedade será uma matriz nula/vazia. |
|type                   | String                    |O tipo dessa fonte de mapeamento de atributos. Os valores possíveis são: `Attribute`, `Constant`, `Function`. O padrão é `Attribute`.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

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

## <a name="json-examples"></a>Exemplos JSON

Atributo simples para mapeamento de atributos

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

Expression extracting first 8 characters from the source attribute

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


