---
title: Tipo de recurso filterGroup
description: Define um conjunto de cláusulas que um objeto deve satisfazer para ser considerado no escopo.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 6338ae4b02b79d1512d5e9f695a69155197e2f4a
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131912"
---
# <a name="filtergroup-resource-type"></a>Tipo de recurso filterGroup

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Define um conjunto de cláusulas que um objeto deve satisfazer para ser considerado no escopo. Um objeto é considerado no escopo do grupo (o grupo é avaliado para ) somente se todas as cláusulas do grupo são `true` avaliadas para `true` .

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|clauses|[Coleção filterClause](synchronization-filterclause.md)|Cláusulas de filtro (condições) desse grupo. Todas as cláusulas em um grupo devem ser atendidas para que o grupo de filtros seja avaliada como `true` .|
|nome|String|Nome acessível para humanos do grupo de filtros.|

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


