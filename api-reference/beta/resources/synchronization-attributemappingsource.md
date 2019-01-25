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
# <a name="attributemappingsource-resource-type"></a>tipo de recurso de attributeMappingSource

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Define como um valor deve ser extraída (ou transformados) do objeto de origem. Por exemplo, pode ser um valor simple tirado de um determinado atributo no objeto de origem, ou pode ser uma expressão mais complexa de cadeia de caracteres concatenação/extração/substituição com base em vários atributos de fonte. 

## <a name="properties"></a>Propriedades

| Propriedade              | Tipo                      | Descrição               |
|:----------------------|:--------------------------|:--------------------------|
|expressão             |String                     |Representação de expressão equivalente deste objeto **attributeMappingSource** .|
|name                   |Cadeia de caracteres                     |Parâmetro nome da fonte de mapeamento. Dependendo do valor da propriedade **type** , isso pode ser o nome da função, o nome do atributo de origem, ou um valor de constante a ser usado. |
|parâmetros             |coleção [stringKeyAttributeMappingSourceValuePair](synchronization-stringkeyattributemappingsourcevaluepair.md) | Se esse objeto representa uma função, lista os parâmetros da função. Parâmetros consistem em objetos **attributeMappingSource** sozinhos, permitindo expressões complexas. Se **tipo** não for `Function`, essa propriedade será null/vazio matriz. |
|type                   | String                    |O tipo de fonte de mapeamento este atributo. Os valores possíveis são: `Attribute`, `Constant`, `Function`. O padrão é `Attribute`.| 

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

Mapeamento de atributo para o atributo simples

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

Expressão extraindo 8 primeiros caracteres do atributo de origem

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
