---
title: Tipo de recurso plannerPlanDetails
description: O **recurso plannerPlanDetails** representa as informações adicionais sobre um plano. Cada objeto de plano tem um objeto de detalhes.
ms.localizationpriority: medium
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 41daa24c42805b76702a9ed77942c9ce1edbcbf7
ms.sourcegitcommit: ca1b33aaecb320b33423aeec7438ce306bffab14
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/14/2022
ms.locfileid: "65420548"
---
# <a name="plannerplandetails-resource-type"></a>Tipo de recurso plannerPlanDetails

Namespace: microsoft.graph


O **recurso plannerPlanDetails** representa as informações adicionais sobre um plano. Cada [objeto de](plannerplan.md) plano tem um objeto de detalhes.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter plannerPlanDetails](../api/plannerplandetails-get.md) | [plannerPlanDetails](plannerplandetails.md) |Ler propriedades e relações do **objeto plannerPlanDetails** .|
|[Atualizar](../api/plannerplandetails-update.md) | [plannerPlanDetails](plannerplandetails.md)    |**Atualize o objeto plannerPlanDetails**. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|categoryDescriptions|[plannerCategoryDescriptions](plannercategorydescriptions.md)|Um objeto que especifica as descrições das 25 categorias que podem ser associadas a tarefas no plano.|
|id|String| Somente leitura. ID dos detalhes do plano. Tem 28 caracteres e diferencia maiúsculas de minúsculas. [Formatar validação](planner-identifiers-disclaimer.md) é feito no serviço.|
|sharedWith|[plannerUserIds](planneruserids.md)|Conjunto de IDs de usuário com as qual esse plano é compartilhado. Se você estiver aproveitando os Microsoft 365, use a API de Grupos para gerenciar a associação de grupo para compartilhar o [plano do](group.md) grupo. Você também pode adicionar membros existentes do grupo a essa coleção, embora não seja necessário que eles acessem o plano pertencente ao grupo. |

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

