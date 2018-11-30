---
title: Tipo de recurso planner
description: O recurso **planner** é o ponto de entrada do modelo de objeto do Planner. Ele retorna um único recurso **planner**.  Ele não contém quaisquer propriedades utilizáveis.
ms.openlocfilehash: e5980f6f4037b57e977b12ef223e8a5a2cf7c77c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006747"
---
# <a name="planner-resource-type"></a>Tipo de recurso planner

O recurso **planner** é o ponto de entrada do modelo de objeto do Planner. Ele retorna um único recurso **planner**.  Ele não contém quaisquer propriedades utilizáveis.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Criar plannerBucket](../api/planner-post-buckets.md) |[plannerBucket](plannerbucket.md)| Crie um novo **plannerBucket** ao postar na coleção de buckets.|
|[Criar plannerPlan](../api/planner-post-plans.md) |[plannerPlan](plannerplan.md)| Crie um novo **plannerPlan** ao postar na coleção de planos.|
|[Criar plannerTask](../api/planner-post-tasks.md) |[plannerTask](plannertask.md)| Crie um novo **plannerTask** ao postar na coleção de tarefas.|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|buckets|Coleção [plannerBucket](plannerbucket.md)| Somente leitura. Anulável. Retorna uma coleção dos buckets especificados|
|plans|Coleção [plannerPlan](plannerplan.md)| Somente leitura. Anulável. Retorna uma coleção dos planos especificados|
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

O recurso de **Planejador** estará disponível na raiz do gráfico.

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