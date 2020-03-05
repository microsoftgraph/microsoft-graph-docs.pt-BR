---
title: tipo de recurso filterOperatorSchema
description: Descreve um operador que pode ser usado em um filtro.
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 868ecf1e57deb624ab8b276d3f10cd39176efa5b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520167"
---
# <a name="filteroperatorschema-resource-type"></a>tipo de recurso filterOperatorSchema

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Descreve um operador que pode ser usado em um [filtro](synchronization-filter.md).

## <a name="properties"></a>Propriedades

| Propriedade                   | Tipo                      | Descrição    |
|:---------------------------|:--------------------------|:---------------|
|arity                       |String          |Arity do operador. Os valores possíveis são: `Binary` e `Unary`. O padrão é `Binary`.|
|multivaluedComparisonType   |scopeOperatorMultiValuedComparisonType          |Os valores possíveis são: `All` e `Any`. Aplica-se somente a atributos com vários valores. `All`significa que todos os valores devem atender à condição. `Any`significa que pelo menos um valor deve satisfazer a condição. O padrão é `All`.|
|nome                        |String                     |Nome do operador. |
|supportedAttributeTypes     |String collection         |Tipos de atributo suportados pelo operador. Os valores possíveis são: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.|

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
<!--
{
  "type": "#page.annotation",
  "description": "filterOperatorSchema resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
