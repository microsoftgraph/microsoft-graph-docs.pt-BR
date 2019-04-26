---
title: tipo de recurso plannerUser
description: 'O recurso **plannerUser** fornece acesso aos recursos do Planner para um usuário. '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 1f10810f6debf2346ed12484bac8e1f4bfd2f372
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563639"
---
# <a name="planneruser-resource-type"></a>tipo de recurso plannerUser

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O recurso **plannerUser** fornece acesso aos recursos do Planner para um [usuário](user.md). 


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Listar tarefas](../api/planneruser-list-tasks.md) |Coleção [plannerTask](plannertask.md)| Obtenha o [plannerTasks](plannertask.md) atribuído ao usuário.|
|[Listar favoritePlans](../api/planneruser-list-favoriteplans.md) |Coleção [plannerPlan](plannerplan.md)| Obter o [plannerPlans](plannerplan.md) marcado como favorito pelo usuário.|
|[Listar recentPlans](../api/planneruser-list-recentplans.md) |Coleção [plannerPlan](plannerplan.md)| Obtenha o [plannerPlans](plannerplan.md) exibido recentemente pelo usuário.|
|[Update](../api/planneruser-update.md) | [plannerUser](planneruser.md)| Atualizar um objeto **plannerUser** . |


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|String| Somente leitura. Identificador do plannerUser|
|favoritePlanReferences|[plannerFavoritePlanReferenceCollection](plannerfavoriteplanreferencecollection.md)| Uma coleção que contém as referências aos planos que o usuário marcou como favoritos.|
|recentPlanReferences|[plannerRecentPlanReferenceCollection](plannerrecentplanreferencecollection.md)| Uma coleção que contém referências aos planos que foram exibidos recentemente pelo usuário em aplicativos que dão suporte a planos recentes.|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|tarefas|Coleção [plannerTask](plannertask.md)| Somente leitura. Anulável. Retorna o [plannerTasks](plannertask.md) atribuído ao usuário.|
|favoritePlans|Coleção [plannerPlan](plannerplan.md)| Somente leitura. Anulável. Retorna o [plannerPlans](plannerplan.md) que o usuário marcou como favoritos.|
|recentPlans|Coleção [plannerPlan](plannerplan.md)| Somente leitura. Anulável. Retorna o [plannerPlans](plannerplan.md) que foi exibido recentemente pelo usuário em aplicativos que dão suporte a planos recentes. |

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",  
  "@odata.type": "microsoft.graph.plannerUser"
}-->

```json
{
  "favoritePlanReferences": {"@odata.type": "microsoft.graph.plannerFavoritePlanReferenceCollection"},
  "id": "String (identifier)",
  "recentPlanReferences": {"@odata.type": "microsoft.graph.plannerRecentPlanReferenceCollection"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
