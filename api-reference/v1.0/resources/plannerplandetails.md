---
title: tipo de recurso plannerPlanDetails
description: O recurso **plannerPlanDetails** representa as informações adicionais sobre um plano. Cada objeto Plan tem um objeto details.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: d75bbf877fcd70203b71159b198f5bad5f1bc3f0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035186"
---
# <a name="plannerplandetails-resource-type"></a>tipo de recurso plannerPlanDetails


O recurso **plannerPlanDetails** representa as informações adicionais sobre um plano. Cada objeto [Plan](plannerplan.md) tem um objeto details.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter plannerPlanDetails](../api/plannerplandetails-get.md) | [plannerPlanDetails](plannerplandetails.md) |Leia as propriedades e os relacionamentos do objeto **plannerPlanDetails** .|
|[Atualização](../api/plannerplandetails-update.md) | [plannerPlanDetails](plannerplandetails.md)    |Atualize o objeto **plannerPlanDetails** . |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|categoryDescriptions|[plannerCategoryDescriptions](plannercategorydescriptions.md)|Um objeto que especifica as descrições das seis categorias que podem ser associadas a tarefas no plano|
|id|String| Somente leitura. ID do plano de detalhes. Tem 28 caracteres e diferencia maiúsculas de minúsculas. [Formatar validação](planner-identifiers-disclaimer.md) é feito no serviço.|
|sharedWith|[plannerUserIds](planneruserids.md)|Conjunto de IDs de usuário com as quais esse plano é compartilhado. Se estiver aproveitando os grupos do Office 365, use a API de grupos para gerenciar a associação de grupo para compartilhar o plano [do grupo](group.md) . Você também pode adicionar membros existentes do grupo a essa coleção, embora não seja necessário que eles acessem o plano de Propriedade do grupo. |

## <a name="relationships"></a>Relações
Nenhum


## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.plannerPlanDetails"
}-->

```json
{
  "categoryDescriptions": {"@odata.type": "microsoft.graph.plannerCategoryDescriptions"},
  "id": "String (identifier)",
  "sharedWith": {"@odata.type": "microsoft.graph.plannerUserIds"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerPlanDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
