---
title: Tipo de recurso plannerUser
description: O **recurso plannerUser** fornece acesso aos recursos do Planner para um usuário. Ele não contém propriedades usáveis.
ms.localizationpriority: medium
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 5a2220ced0459118a6be00ee03a2b9282b6635cb
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59129800"
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

