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
# <a name="filteroperatorschema-resource-type"></a>tipo de recurso de filterOperatorSchema

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Descreve um operador que pode ser usado em um [filtro](synchronization-filter.md).

## <a name="properties"></a>Propriedades

| Propriedade                   | Tipo                      | Descrição    |
|:---------------------------|:--------------------------|:---------------|
|aridade                       |Cadeia de caracteres          |Aridade do operador. Os valores possíveis são: `Binary` e `Unary`. O padrão é `Binary`.|
|multivaluedComparisonType   |scopeOperatorMultiValuedComparisonType          |Os valores possíveis são: `All` e `Any`. Só se aplica aos atributos de valores múltiplos. `All`significa que todos os valores devem satisfazer a condição. `Any`significa que pelo menos um valor tem que satisfazer a condição. O padrão é `All`.|
|name                        |Cadeia de caracteres                     |Nome do operador. |
|supportedAttributeTypes     |String collection         |Tipos suportados pela operadora de atributo. Os valores possíveis são: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

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
