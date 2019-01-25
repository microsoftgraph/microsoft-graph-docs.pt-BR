---
title: Tipo de recurso plannerPlanDetails
description: O recurso **plannerPlanDetails** representa as informações adicionais sobre um plano. Cada objeto plan tem um objeto de detalhes.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 9d10f5b04bc3b98a5e32eac7b577cbf4c582bab4
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529877"
---
# <a name="plannerplandetails-resource-type"></a>Tipo de recurso plannerPlanDetails

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O recurso **plannerPlanDetails** representa as informações adicionais sobre um plano. Cada objeto [plan](plannerplan.md) tem um objeto de detalhes.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Get plannerPlanDetails](../api/plannerplandetails-get.md) | [plannerPlanDetails](plannerplandetails.md) |Leia as propriedades e relacionamentos de um objeto **plannerPlanDetails** .|
|[Update](../api/plannerplandetails-update.md) | [plannerPlanDetails](plannerplandetails.md)    |Atualize um objeto **plannerPlanDetails** . |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|categoryDescriptions|[plannerCategoryDescriptions](plannercategorydescriptions.md)|Um objeto que especifica as descrições das seis categorias que podem ser associadas a tarefas no plano|
|id|String| Somente leitura. A identificação dos detalhes do plano. É 28 caracteres longos e diferencia maiusculas de minúsculas. [Validação de formato](tasks-identifiers-disclaimer.md) é feita no serviço.|
|sharedWith|[plannerUserIds](planneruserids.md)|O conjunto deste plano compartilhada com IDs de usuário. Se você estiver usando o Office 365 grupos, use os API de grupos para gerenciar a associação de grupo para compartilhar o plano [do grupo](group.md) . Você também pode adicionar membros existentes do grupo para este conjunto, embora não seja obrigatório na ordem para que eles possam acessar o plano pertencente ao grupo. |
|contextDetails|[plannerPlanContextDetailsCollection](plannerplancontextdetailscollection.md)|Somente leitura. Uma coleção de informações adicionais associadas entradas [plannerPlanContext](plannerplancontext.md) definidas para o contêiner de [plannerPlan](plannerplan.md) . |

## <a name="relationships"></a>Relações
Nenhum


## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerPlanDetails"
}-->

```json
{
  "categoryDescriptions": {"@odata.type": "microsoft.graph.plannerCategoryDescriptions"},
  "contextDetails": {"@odata.type": "microsoft.graph.plannerPlanContextDetailsCollection"},
  "id": "String (identifier)",
  "sharedWith": {"@odata.type": "microsoft.graph.plannerUserIds"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerPlanDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerplandetails.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
