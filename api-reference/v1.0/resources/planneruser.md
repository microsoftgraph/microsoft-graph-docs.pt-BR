---
title: tipo de recurso plannerUser
description: O recurso **plannerUser** fornece acesso a recursos do Planner para um usuário. Ele não contém propriedades utilizáveis.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 49b8989bd8526cbe8074a386ae31e76fd195642d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447091"
---
# <a name="planneruser-resource-type"></a>tipo de recurso plannerUser

Namespace: Microsoft. Graph

O recurso **plannerUser** fornece acesso a recursos do Planner para um [usuário](user.md). Ele não contém propriedades utilizáveis.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Listar planos](../api/planneruser-list-plans.md) |Coleção [plannerPlan](plannerplan.md)| Obtenha uma coleção de objetos **plannerPlan** .|
|[Listar tarefas](../api/planneruser-list-tasks.md) |Coleção [plannerTask](plannertask.md)| Obter uma coleção de objetos **plannerTask**.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|String| Somente leitura. Identificador do planenrUser|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|Planeje|Coleção [plannerPlan](plannerplan.md)| Somente leitura. Anulável. Retorna o [plannerTasks](plannertask.md) atribuído ao usuário.|
|tarefas|Coleção [plannerTask](plannertask.md)| Somente leitura. Anulável. Retorna o [plannerPlans](plannerplan.md) compartilhado com o usuário.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerUser"
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
  "description": "plannerUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
