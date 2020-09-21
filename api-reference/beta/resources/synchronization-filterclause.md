---
title: tipo de recurso filterClause
description: Representa uma declaração única que um objeto candidato deve satisfazer.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 91cc7f85dc4c42f806be5e365f21adb0d5e972fc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47968363"
---
# <a name="filterclause-resource-type"></a>tipo de recurso filterClause

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma declaração única que um objeto candidato deve satisfazer e é avaliada como `true` (objeto satisfaz a asserção) ou `false` (o objeto não satisfaz a asserção).

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|OperatorName|String|Nome do operador a ser aplicado aos operandos de origem e de destino. Deve ser um dos operadores com suporte. Os operadores com suporte podem ser descobertos.|
|sourceOperandName|String|Nome do operando de origem (o operando que está sendo testado). O nome do operando de origem deve corresponder a um dos nomes de atributo no objeto de origem.|
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


