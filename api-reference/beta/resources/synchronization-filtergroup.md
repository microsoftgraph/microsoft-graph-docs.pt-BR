---
title: tipo de recurso de filterGroup
description: Define um conjunto de cláusulas que um objeto deve satisfazer para ser considerados no escopo. Um objeto é considerado no escopo do grupo (o grupo é avaliado para `true`) somente se todas as cláusulas do grupo são avaliadas para `true`.
localization_priority: Normal
ms.openlocfilehash: b71bdf16d6639b5ecc8512565ccf56d592a0da58
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514184"
---
# <a name="filtergroup-resource-type"></a>tipo de recurso de filterGroup

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Define um conjunto de cláusulas que um objeto deve satisfazer para ser considerados no escopo. Um objeto é considerado no escopo do grupo (o grupo é avaliado para `true`) somente se todas as cláusulas do grupo são avaliadas para `true`.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|Cláusulas|coleção [filterClause](synchronization-filterclause.md)|Filtre cláusulas (condições) desse grupo. Todas as cláusulas em um grupo devem ser atendidas para o grupo de filtro a ser avaliada como `true`.|
|name|String|Legíveis nome do grupo de filtro.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.filterGroup"
}-->

```json
{
  "clauses": [{"@odata.type": "microsoft.graph.filterClause"}],
  "name": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "filterGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-filtergroup.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
