---
title: Tipo de recurso plannerUser
description: 'O recurso de **plannerUser** fornece acesso aos recursos do Planejador de um usuário. '
localization_priority: Normal
ms.openlocfilehash: 709b259c88d8fe0f02defaa57e77727a7b967cfd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27820801"
---
# <a name="planneruser-resource-type"></a>Tipo de recurso plannerUser

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

O recurso de **plannerUser** fornece acesso aos recursos do Planejador de um [usuário](user.md). 


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Listar tarefas](../api/planneruser-list-tasks.md) |Coleção [plannerTask](plannertask.md)| Obtenha o [plannerTasks](plannertask.md) atribuída ao usuário.|
|[Lista favoritePlans](../api/planneruser-list-favoriteplans.md) |Coleção [plannerPlan](plannerplan.md)| Obtenha o [plannerPlans](plannerplan.md) marcado como favorito pelo usuário.|
|[Lista recentPlans](../api/planneruser-list-recentplans.md) |Coleção [plannerPlan](plannerplan.md)| Obtenha o [plannerPlans](plannerplan.md) visualizados recentemente pelo usuário.|
|[Update](../api/planneruser-update.md) | [plannerUser](planneruser.md)| Atualize um objeto **plannerUser** . |


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|Cadeia de caracteres| Somente leitura. Identificador do plannerUser|
|favoritePlanReferences|[plannerFavoritePlanReferenceCollection](plannerfavoriteplanreferencecollection.md)| Uma coleção que contém as referências para os planos de que o usuário tenha marcado como Favoritos.|
|recentPlanReferences|[plannerRecentPlanReferenceCollection](plannerrecentplanreferencecollection.md)| Uma coleção que contém referências para os planos que foram visualizados recentemente pelo usuário em aplicativos que suportam planos recentes.|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|tarefas|Coleção [plannerTask](plannertask.md)| Somente leitura. Anulável. Returna o [plannerTasks](plannertask.md) atribuídos ao usuário.|
|favoritePlans|Coleção [plannerPlan](plannerplan.md)| Somente leitura. Anulável. Retorna o [plannerPlans](plannerplan.md) que o usuário marcado como Favoritos.|
|recentPlans|Coleção [plannerPlan](plannerplan.md)| Somente leitura. Anulável. Retorna o [plannerPlans](plannerplan.md) exibidos recentemente pelo usuário em aplicativos que suportam planos recentes. |

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
<!-- {
  "type": "#page.annotation",
  "description": "plannerUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
