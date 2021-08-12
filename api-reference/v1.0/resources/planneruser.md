---
title: Tipo de recurso plannerUser
description: O **recurso plannerUser** fornece acesso aos recursos do Planner para um usuário. Ele não contém propriedades usáveis.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: a430efc0ca86043a566fce58481edcb2e212f17961b00647aa32781dbcb3dc5b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54154893"
---
# <a name="planneruser-resource-type"></a>Tipo de recurso plannerUser

Namespace: microsoft.graph

O **recurso plannerUser** fornece acesso aos recursos do Planner para um [usuário](user.md). Ele não contém propriedades usáveis.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Listar planos](../api/planneruser-list-plans.md) |coleção [plannerPlan](plannerplan.md)| Obter uma **coleção de objetos plannerPlan.**|
|[Listar tarefas](../api/planneruser-list-tasks.md) |Coleção [plannerTask](plannertask.md)| Obter uma coleção de objetos **plannerTask**.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|String| Somente leitura. Identificador do planenrUser|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|plans|coleção [plannerPlan](plannerplan.md)| Somente leitura. Anulável. Retorna os [plannerTasks](plannertask.md) atribuídos ao usuário.|
|tarefas|Coleção [plannerTask](plannertask.md)| Somente leitura. Anulável. Retorna os [plannerPlans compartilhados](plannerplan.md) com o usuário.|

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

