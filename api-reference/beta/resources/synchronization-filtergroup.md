---
title: tipo de recurso de filtro
description: Define um conjunto de cláusulas que um objeto deve satisfazer para ser considerado em escopo. Um objeto é considerado no escopo do grupo (o grupo é avaliado como `true`) somente se todas as cláusulas do grupo são avaliadas. `true`
localization_priority: Normal
ms.openlocfilehash: b71bdf16d6639b5ecc8512565ccf56d592a0da58
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32582028"
---
# <a name="filtergroup-resource-type"></a>tipo de recurso de filtro

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Define um conjunto de cláusulas que um objeto deve satisfazer para ser considerado em escopo. Um objeto é considerado no escopo do grupo (o grupo é avaliado como `true`) somente se todas as cláusulas do grupo são avaliadas. `true`

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|cláusulas|coleção [filterClause](synchronization-filterclause.md)|Cláusulas de filtro (condições) desse grupo. Todas as cláusulas em um grupo devem ser atendidas para que o grupo de filtros seja `true`avaliado.|
|name|String|Nome legível do grupo de filtros.|

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
