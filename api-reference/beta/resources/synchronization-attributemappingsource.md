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
# <a name="attributemappingsource-resource-type"></a>tipo de recurso de attributeMappingSource

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Define como um valor deve ser extraída (ou transformados) do objeto de origem. Por exemplo, pode ser um valor simple tirado de um determinado atributo no objeto de origem, ou pode ser uma expressão mais complexa de cadeia de caracteres concatenação/extração/substituição com base em vários atributos de fonte. 

## <a name="properties"></a>Propriedades

| Propriedade              | Tipo                      | Descrição               |
|:----------------------|:--------------------------|:--------------------------|
|expressão             |Cadeia de caracteres                     |Representação de expressão equivalente deste objeto **attributeMappingSource** .|
|name                   |Cadeia de caracteres                     |Parâmetro nome da fonte de mapeamento. Dependendo do valor da propriedade **type** , isso pode ser o nome da função, o nome do atributo de origem, ou um valor de constante a ser usado. |
|parâmetros             |coleção [stringKeyAttributeMappingSourceValuePair](synchronization-stringkeyattributemappingsourcevaluepair.md) | Se esse objeto representa uma função, lista os parâmetros da função. Parâmetros consistem em objetos **attributeMappingSource** sozinhos, permitindo expressões complexas. Se **tipo** não for `Function`, essa propriedade será null/vazio matriz. |
|type                   | Cadeia de caracteres                    |O tipo de fonte de mapeamento este atributo. Os valores possíveis são: `Attribute`, `Constant`, `Function`. O padrão é `Attribute`.| 

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
<!-- {
  "type": "#page.annotation",
  "description": "attributeMappingSource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
