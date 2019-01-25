---
title: tipo de recurso de filterClause
description: Representa um único assertion que um objeto de candidato deve satisfazer e é avaliado para uma `true` (objeto atenda a afirmação) ou `false` (o objeto não atender a afirmação).
localization_priority: Normal
ms.openlocfilehash: 62623cee5b2991acbe162561940adb1afd3574a1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523866"
---
# <a name="filterclause-resource-type"></a>tipo de recurso de filterClause

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um único assertion que um objeto de candidato deve satisfazer e é avaliado para uma `true` (objeto atenda a afirmação) ou `false` (o objeto não atender a afirmação).

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|operatorName|String|Nome do operador a ser aplicada à operandos de origem e destino. Deve ser um dos operadores com suporte. Os operadores com suporte que podem ser descobertos.|
|sourceOperandName|String|Nome do operando de origem (o operando que está sendo testado). O nome da fonte operando deve corresponder a um dos nomes de atributo no objeto de origem.|
|targetOperand|[filterOperand](synchronization-filteroperand.md)|Valores que o operando de origem será testado em relação.|

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
