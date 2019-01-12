---
title: Tipo de recurso plannerGroup
description: O recurso de **plannerGroup** fornece acesso aos recursos de Planejador para um grupo. Não contém todas as propriedades utilizáveis.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 6e60db0a3f33bc47d0ea63b7a773b7bb691cd5be
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27981417"
---
# <a name="plannergroup-resource-type"></a>Tipo de recurso plannerGroup

O recurso **plannerGroup** oferece acesso aos recursos do Planner para um [grupo](group.md). Ele não contém quaisquer propriedades utilizáveis.

## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Listar planos](../api/plannergroup-list-plans.md) |Coleção [plannerPlan](plannerplan.md)| Obtenha uma coleção de objetos **plannerPlan**.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|String| Somente leitura. O identificador do **plannerGroup**|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|plans|Coleção [plannerPlan](plannerplan.md)| Somente leitura. Anulável. Retorna o [plannerPlans](plannerplan.md) que pertence ao grupo.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerGroup"
}-->

```json
{
  "id": "String (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
