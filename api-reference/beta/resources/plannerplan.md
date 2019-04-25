---
title: tipo de recurso plannerPlan
description: O recurso **plannerPlan** representa um plano no Office 365. Um plano pode pertencer a um grupo e contém uma coleção de plannerTasks. Também pode ter uma coleção de plannerBuckets. Cada objeto Plan tem um objeto Details que pode conter mais informações sobre o plano. Para obter mais informações sobre as relações entre grupos, planos e tarefas, consulte Planner.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: f37f6ea08f2951256e2d7f94cf9abad7e8ac60b2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32578864"
---
# <a name="plannerplan-resource-type"></a>tipo de recurso plannerPlan

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O recurso **plannerPlan** representa um plano no Office 365. Um plano pode pertencer a um [grupo](group.md) e contém uma coleção de [plannerTasks](plannertask.md). Também pode ter uma coleção de [plannerBuckets](plannerbucket.md). Cada objeto Plan tem um objeto [Details](plannerplandetails.md) que pode conter mais informações sobre o plano. Para obter mais informações sobre as relações entre grupos, planos e tarefas, consulte [Planner](planner-overview.md).



## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter plannerPlan](../api/plannerplan-get.md) | [plannerPlan](plannerplan.md) |Leia as propriedades e os relacionamentos do objeto **plannerPlan** .|
|[Listar buckets](../api/plannerplan-list-buckets.md) |coleção [plannerBucket](plannerbucket.md)| Obtenha uma coleção de objetos **plannerBucket** .|
|[Listar tarefas](../api/plannerplan-list-tasks.md) |Coleção [plannerTask](plannertask.md)| Obtenha uma coleção de objetos **plannerTask** .|
|[Update](../api/plannerplan-update.md) | [plannerPlan](plannerplan.md) |Atualize o objeto **plannerPlan** . |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|createdDateTime|DateTimeOffset|Somente leitura. Data e hora em que o plano foi criado. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|id|String| Somente leitura. ID do plano. Tem 28 caracteres e diferencia maiúsculas de minúsculas. [Formatar validação](tasks-identifiers-disclaimer.md) é feito no serviço.|
|owner|String|ID do [grupo](group.md) que possui o plano. Um grupo válido deve existir antes que este campo possa ser definido. Após a definição, esta propriedade não pode ser atualizada.|
|title|String|Obrigatório. Título do plano.|
|createdBy|[identitySet](identityset.md)|Somente leitura. O usuário que criou o plano.|
|contextos|[plannerPlanContextCollection](plannerplancontextcollection.md)| Somente leitura. Experiências de usuário adicionais nas quais esse plano é usado, representado como entradas [plannerPlanContext](plannerplancontext.md) .|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|buckets|coleção [plannerBucket](plannerbucket.md)| Somente leitura. Anulável. Conjunto de buckets no plano.|
|detalhes|[plannerPlanDetails](plannerplandetails.md)| Somente leitura. Anulável. Detalhes adicionais sobre o plano.|
|tarefas|Coleção [plannerTask](plannertask.md)| Somente leitura. Anulável. Conjunto de tarefas no plano.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerplan.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
