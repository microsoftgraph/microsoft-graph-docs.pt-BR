---
title: Tipo de recurso filterOperatorSchema
description: Descreve um operador que pode ser usado em um filtro.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 1128b12ffcadd36f2fdd2f34d27f95d973cdfd9d
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131884"
---
# <a name="filteroperatorschema-resource-type"></a>Tipo de recurso filterOperatorSchema

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Descreve um operador que pode ser usado em um [filtro.](synchronization-filter.md)

## <a name="properties"></a>Propriedades

| Propriedade                   | Tipo                      | Descrição    |
|:---------------------------|:--------------------------|:---------------|
|arity                       |String          |A personalidade do operador. Os valores possíveis são: `Binary` e `Unary`. O padrão é `Binary` .|
|multivaluedComparisonType   |scopeOperatorMultiValuedComparisonType          |Os valores possíveis são: `All` e `Any`. Aplica-se somente a atributos de múltiplos valores. `All` significa que todos os valores devem satisfazer a condição. `Any` significa que pelo menos um valor deve satisfazer a condição. O padrão é `All` .|
|nome                        |String                     |Nome do operador. |
|supportedAttributeTypes     |Coleção de cadeias de caracteres         |Tipos de atributo suportados pelo operador. Os valores possíveis são: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.|

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


