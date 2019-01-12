---
title: Tipo de recurso plannerPlan
description: O recurso de **plannerPlan** representa um plano no Office 365. Um plano pode pertencer a um grupo e contém uma coleção de plannerTasks. Ele também pode ter uma coleção de plannerBuckets. Cada objeto de plano tem um objeto de detalhes que pode conter mais informações sobre o plano. Para obter mais informações sobre os relacionamentos entre grupos, planos e tarefas, consulte planejador.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: b5d95b1bfab7404007c3139833e54f155c10d9aa
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27950519"
---
# <a name="plannerplan-resource-type"></a>Tipo de recurso plannerPlan

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

O recurso de **plannerPlan** representa um plano no Office 365. Um plano pode pertencer a um [grupo](group.md) e contém uma coleção de [plannerTasks](plannertask.md). Ele também pode ter uma coleção de [plannerBuckets](plannerbucket.md). Cada objeto de plano tem um objeto de [detalhes](plannerplandetails.md) que pode conter mais informações sobre o plano. Para obter mais informações sobre os relacionamentos entre grupos, planos e tarefas, consulte [Planejador](planner-overview.md).



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
|createdDateTime|DateTimeOffset|Somente leitura. A data e a hora que o plano foi criado. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|id|String| Somente leitura. ID do plano. É 28 caracteres longos e diferencia maiusculas de minúsculas. [Validação de formato](tasks-identifiers-disclaimer.md) é feita no serviço.|
|owner|String|ID do [grupo](group.md) que possui o plano. Um grupo válido deve existir antes que esse campo pode ser definido. Depois que ele for definido, essa propriedade não pode ser atualizada.|
|title|String|Obrigatório. Título do plano.|
|createdBy|[identitySet](identityset.md)|Somente leitura. O usuário que criou o plano.|
|contextos|[plannerPlanContextCollection](plannerplancontextcollection.md)| Somente leitura. Experiências de usuário adicional no qual este plano for usado, representado como entradas de [plannerPlanContext](plannerplancontext.md) .|

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
<!-- {
  "type": "#page.annotation",
  "description": "plannerPlan resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
