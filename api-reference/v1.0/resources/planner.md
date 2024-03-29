---
title: Tipo de recurso do planner
description: O **recurso** planner é o ponto de entrada para o modelo de objeto do Planner. Ele retorna um recurso de **planejador de singleton.**  Ele não contém propriedades usáveis.
ms.localizationpriority: medium
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: cdb0234edce0e28456ab830b259f09d1f874b1c7
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59044381"
---
# <a name="planner-resource-type"></a>Tipo de recurso do planner

Namespace: microsoft.graph

O **recurso** planner é o ponto de entrada para o modelo de objeto do Planner. Ele retorna um recurso de **planejador de singleton.**  Ele não contém propriedades usáveis.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Criar plannerBucket](../api/planner-post-buckets.md) |[plannerBucket](plannerbucket.md)| Crie um novo **plannerBucket** postando na coleção buckets.|
|[Criar plannerPlan](../api/planner-post-plans.md) |[plannerPlan](plannerplan.md)| Crie um novo **plannerPlan** postando na coleção plans.|
|[Criar plannerTask](../api/planner-post-tasks.md) |[plannerTask](plannertask.md)| Crie um novo **plannerTask** postando na coleção de tarefas.|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|buckets|Coleção [plannerBucket](plannerbucket.md)| Somente leitura. Anulável. Retorna uma coleção dos buckets especificados|
|plans|coleção [plannerPlan](plannerplan.md)| Somente leitura. Anulável. Retorna uma coleção dos planos especificados|
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

O **recurso** planner está disponível na raiz do gráfico.

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
```http
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

