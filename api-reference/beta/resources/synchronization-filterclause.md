---
title: tipo de recurso filterClause
description: Representa uma declaração única que um objeto candidato deve satisfazer.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 6688f26353bed9e92f60a93b688b1679e70bd75f
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/10/2020
ms.locfileid: "43218426"
---
# <a name="filterclause-resource-type"></a>tipo de recurso filterClause

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma declaração única que um objeto candidato deve satisfazer e é avaliada como `true` (objeto satisfaz a asserção) ou `false` (o objeto não satisfaz a asserção).

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|OperatorName|Cadeia de Caracteres|Nome do operador a ser aplicado aos operandos de origem e de destino. Deve ser um dos operadores com suporte. Os operadores com suporte podem ser descobertos.|
|sourceOperandName|Cadeia de Caracteres|Nome do operando de origem (o operando que está sendo testado). O nome do operando de origem deve corresponder a um dos nomes de atributo no objeto de origem.|
|targetOperand|[filterOperand](synchronization-filteroperand.md)|Valores em relação ao qual o operando de origem será testado.|

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
