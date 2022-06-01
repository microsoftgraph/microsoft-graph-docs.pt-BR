---
title: Tipo de recurso plannerPlan
description: O recurso **plannerPlan** representa um plano no Microsoft 365. Um plano pode pertencer a um grupo e conter um conjunto de plannerTasks. Ele também pode ter uma coleção de plannerBuckets. Cada objeto de plano tem um objeto de detalhes que pode conter mais informações sobre o plano. Para saber mais sobre as relações entre grupos, planos e tarefas, confira o Planner.
ms.localizationpriority: high
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: d25c85d8cf63ff018a521b86822d8d2380d65ebb
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/01/2022
ms.locfileid: "65819710"
---
# <a name="plannerplan-resource-type"></a>Tipo de recurso plannerPlan

Namespace: microsoft.graph

O recurso **plannerPlan** representa um plano no Microsoft 365. Um plano pode pertencer a um [grupo](group.md) e conter uma coleção de [plannerTasks](plannertask.md). Ele também pode ter uma coleção de [plannerBuckets](plannerbucket.md). Cada objeto de plano tem um objeto de [detalhes](plannerplandetails.md) que pode conter mais informações sobre o plano. Para saber mais sobre as relações entre grupos, planos e tarefas, confira o [Planner](planner-overview.md).

## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Get plannerPlan](../api/plannerplan-get.md) | [plannerPlan](plannerplan.md) |Leia as propriedades e as relações do objeto **plannerPlan**.|
|[Listar buckets](../api/plannerplan-list-buckets.md) |Coleção [plannerBucket](plannerbucket.md)| Obter uma coleção de objetos **plannerBucket**.|
|[Listar tarefas](../api/plannerplan-list-tasks.md) |Coleção [plannerTask](plannertask.md)| Obter uma coleção de objetos **plannerTask**.|
|[Atualizar](../api/plannerplan-update.md) | [plannerPlan](plannerplan.md) |Atualize o objeto **plannerPlan**. |
|[Delete](../api/plannerplan-delete.md) | Nenhum | Exclua o objeto **plannerPlan**. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|contêiner|[plannerPlanContainer](../resources/plannerplancontainer.md)|Identifica o contêiner do plano. Depois de definida, essa propriedade não pode ser atualizada. Obrigatório.|
|createdBy|[identitySet](identityset.md)|Somente leitura. O usuário que criou o plano.|
|createdDateTime|DateTimeOffset|Somente leitura. Data e hora em que o plano é criado. O tipo de carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1º de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|id|String| Somente leitura. A ID do plano. Tem 28 caracteres e diferencia maiúsculas de minúsculas. [Formatar validação](planner-identifiers-disclaimer.md) é feito no serviço.|
|title|String|Obrigatório. Título do plano.|
|proprietário (obsoleto) |String| Use antes a propriedade **contêiner**. A ID do [grupo](group.md) que possui o plano. Depois de definida, essa propriedade não pode ser atualizada. Esta propriedade não devolverá uma ID de grupo válida se o contêiner do plano não for um grupo.|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|buckets|Coleção [plannerBucket](plannerbucket.md)| Somente leitura. Anulável. A coleção de buckets no plano.|
|detalhes|[plannerPlanDetails](plannerplandetails.md)| Somente leitura. Anulável. Outros detalhes sobre o plano.|
|tarefas|Coleção [plannerTask](plannertask.md)| Somente leitura. Anulável. A coleção de tarefas no plano.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerPlan"
}-->

```json
{
  "container": {
    "@odata.type": "microsoft.graph.plannerPlanContainer",
    "containerId": "String",
    "type": "String",
    "url": "String"
  },
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "title": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerPlan resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

