---
title: tipo de recurso Planner
description: O recurso **Planner** é o ponto de entrada para o modelo de objeto do Planner. Ele retorna um recurso **planejador** singleton.  Ele não contém propriedades utilizáveis.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: a7387b95e933378cb089834a1af29e0c7ca45266
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42534040"
---
# <a name="planner-resource-type"></a>tipo de recurso Planner

Namespace: microsoft.graph

O recurso **Planner** é o ponto de entrada para o modelo de objeto do Planner. Ele retorna um recurso **planejador** singleton.  Ele não contém propriedades utilizáveis.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Criar plannerBucket](../api/planner-post-buckets.md) |[plannerBucket](plannerbucket.md)| Crie um novo **plannerBucket** postando na coleção buckets.|
|[Criar plannerPlan](../api/planner-post-plans.md) |[plannerPlan](plannerplan.md)| Crie um novo **plannerPlan** postando na coleção Plans.|
|[Criar plannerTask](../api/planner-post-tasks.md) |[plannerTask](plannertask.md)| Crie um novo **plannerTask** postando na coleção Tasks.|

## <a name="relationships"></a>Relacionamento
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|buckets|Coleção [plannerBucket](plannerbucket.md)| Somente leitura. Anulável. Retorna uma coleção dos buckets especificados|
|Planeje|Coleção [plannerPlan](plannerplan.md)| Somente leitura. Anulável. Retorna uma coleção de planos especificados|
|tarefas|Coleção [plannerTask](plannertask.md)| Somente leitura. Anulável. Retorna uma coleção das tarefas especificadas|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.planner"
}-->

```json
{
}
```

## <a name="example"></a>Exemplo

O recurso **Planner** está disponível na raiz do gráfico.

<!--{
  "blockType": "request"
}-->
```http
GET https://graph.microsoft.com/v1.0/planner
```

<!--{
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.planner"
}-->
```json
HTTP/1.1 200 OK
Content-type: application/json

{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "planner resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
