---
title: tipo de recurso Planner
description: O recurso **Planner** é o ponto de entrada para o modelo de objeto do Planner. Ele retorna um recurso **planejador** singleton.  Ele não contém propriedades utilizáveis.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 2f1fb3b7058a87dd7b8390408590371cf1b0e9cd
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344611"
---
# <a name="planner-resource-type"></a>tipo de recurso Planner

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O recurso **Planner** é o ponto de entrada para o modelo de objeto do Planner. Ele retorna um recurso **planejador** singleton.  Ele não contém propriedades utilizáveis.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Criar plannerBucket](../api/planner-post-buckets.md) |[plannerBucket](plannerbucket.md)| Crie um novo **plannerBucket** postando na coleção buckets.|
|[Criar plannerPlan](../api/planner-post-plans.md) |[plannerPlan](plannerplan.md)| Crie um novo **plannerPlan** postando na coleção Plans.|
|[Criar plannerTask](../api/planner-post-tasks.md) |[plannerTask](plannertask.md)| Crie um novo **plannerTask** postando na coleção Tasks.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|String| Somente leitura. Identificador do recurso **Planner** .|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|buckets|Coleção [plannerBucket](plannerbucket.md)| Somente leitura. Anulável. Retorna uma coleção dos buckets especificados|
|Planeje|Coleção [plannerPlan](plannerplan.md)| Somente leitura. Anulável. Retorna uma coleção de planos especificados|
|tarefas|Coleção [plannerTask](plannertask.md)| Somente leitura. Anulável. Retorna uma coleção das tarefas especificadas|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",  
  "@odata.type": "microsoft.graph.planner"
}-->

```json
{
  "id": "String (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "planner resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
