---
title: Tipo de recurso filterClause
description: Representa uma única declaração que um objeto candidato deve satisfazer.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: fc633f6e25373713679da30a5b319ab8ae99fb04
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131919"
---
# <a name="filterclause-resource-type"></a>Tipo de recurso filterClause

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma única declaração que um objeto candidato deve satisfazer e é avaliada para (o objeto satisfaz a assarção) ou (o objeto não satisfaz `true` `false` a assarção).

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|operatorName|String|Nome do operador a ser aplicado aos operadores de origem e de destino. Deve ser um dos operadores com suporte. Os operadores com suporte podem ser descobertos.|
|sourceOperandName|String|Nome do operand de origem (o operand que está sendo testado). O nome do operand de origem deve corresponder a um dos nomes de atributo no objeto de origem.|
|targetOperand|[filterOperand](synchronization-filteroperand.md)|Valores que o operand de origem será testado.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.filterClause"
}-->

```json
{
  "operatorName": "String",
  "sourceOperandName": "String",
  "targetOperand": {"@odata.type": "microsoft.graph.filterOperand"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "filterClause resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


