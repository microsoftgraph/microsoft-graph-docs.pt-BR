---
title: tipo de recurso filterClause
description: Representa uma declaração única que um objeto candidato deve satisfazer e é avaliada como `true` (objeto satisfaz a asserção) ou `false` (o objeto não satisfaz a asserção).
localization_priority: Normal
ms.openlocfilehash: 62623cee5b2991acbe162561940adb1afd3574a1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32582035"
---
# <a name="filterclause-resource-type"></a>tipo de recurso filterClause

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
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-filterclause.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
