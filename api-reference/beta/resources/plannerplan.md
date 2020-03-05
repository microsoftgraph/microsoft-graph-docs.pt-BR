---
title: Tipo de recurso plannerPlan
description: O recurso **plannerPlan** representa um plano no Office 365. Um plano pode pertencer a um grupo e conter um conjunto de plannerTasks. Ele também pode ter uma coleção de plannerBuckets. Cada objeto Plan tem um objeto Details que pode conter mais informações sobre o plano. Para saber mais sobre as relações entre grupos, planos e tarefas, confira o Planner.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 973d6dfd9bed1bfef2c607276b9aaa0512f0fe9a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521710"
---
# <a name="plannerplan-resource-type"></a>Tipo de recurso plannerPlan

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O recurso **plannerPlan** representa um plano no Office 365. Um plano pode pertencer a um [grupo](group.md) e conter uma coleção de [plannerTasks](plannertask.md). Ele também pode ter uma coleção de [plannerBuckets](plannerbucket.md). Cada objeto Plan tem um objeto [Details](plannerplandetails.md) que pode conter mais informações sobre o plano. Para saber mais sobre as relações entre grupos, planos e tarefas, confira o [Planner](planner-overview.md).



## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Get plannerPlan](../api/plannerplan-get.md) | [plannerPlan](plannerplan.md) |Leia as propriedades e as relações do objeto **plannerPlan**.|
|[Listar buckets](../api/plannerplan-list-buckets.md) |Coleção [plannerBucket](plannerbucket.md)| Obter uma coleção de objetos **plannerBucket**.|
|[Listar tarefas](../api/plannerplan-list-tasks.md) |Coleção [plannerTask](plannertask.md)| Obter uma coleção de objetos **plannerTask**.|
|[Atualizar](../api/plannerplan-update.md) | [plannerPlan](plannerplan.md) |Atualize o objeto **plannerPlan**. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|createdDateTime|DateTimeOffset|Somente leitura. A data e a hora que o plano foi criado. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|id|String| Somente leitura. A ID do plano. Tem 28 caracteres e diferencia maiúsculas de minúsculas. [Formatar validação](tasks-identifiers-disclaimer.md) é feito no serviço.|
|owner|Cadeia de caracteres|A ID do [Grupo](group.md) que possui o plano. Deve haver um grupo válido para que esse campo possa ser definido. Depois de definida, essa propriedade não pode ser atualizada.|
|title|String|Obrigatório. Título do plano.|
|createdBy|[identitySet](identityset.md)|Somente leitura. O usuário que criou o plano.|
|contextos|[plannerPlanContextCollection](plannerplancontextcollection.md)| Somente leitura. Experiências de usuário adicionais nas quais esse plano é usado, representado como entradas [plannerPlanContext](plannerplancontext.md) .|

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
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",  
  "@odata.type": "microsoft.graph.plannerPlan"
}-->

```json
{
  "contexts": {
    "48#19%3Ad128c63941b24733951ea7defd81e550%40thread%2Eskype19%3Ad128c63941b24733951ea7defd81e550%40thread%2Eskype": {
        "@odata.type": "#microsoft.graph.plannerPlanContext",
        "associationType": "Board",
        "createdDateTime": "2015-10-14T00:57:28.4698344Z",
        "displayNameSegments": [
            "Finance Team",
            "Budget Plans"
        ],
        "ownerAppId": "5e3ce6c0-2b1f-4285-8d4b-75ee78787346"
    }
  },
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "owner": "String",
  "title": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerPlan resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
