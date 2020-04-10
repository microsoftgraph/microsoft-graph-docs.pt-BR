---
title: tipo de recurso de filtro
description: Define um conjunto de cláusulas que um objeto deve satisfazer para ser considerado em escopo.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 6e7933bf2fef6240dd0dc53d7da975074225aa30
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/10/2020
ms.locfileid: "43217887"
---
# <a name="filtergroup-resource-type"></a>tipo de recurso de filtro

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Define um conjunto de cláusulas que um objeto deve satisfazer para ser considerado em escopo. Um objeto é considerado no escopo do grupo (o grupo é avaliado como `true`) somente se todas as cláusulas do grupo são avaliadas. `true`

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|cláusulas|coleção [filterClause](synchronization-filterclause.md)|Cláusulas de filtro (condições) desse grupo. Todas as cláusulas em um grupo devem ser atendidas para que o grupo de filtros seja `true`avaliado.|
|nome|String|Nome legível do grupo de filtros.|

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
  "suppressions": []
}
-->
