---
title: Tipo de recurso plannerBucket
description: ) para tarefas em um plano em Microsoft 365. Ele está contido em um plannerPlan e pode ter uma coleção de plannerTasks.
author: TarkanSevilmis
ms.localizationpriority: medium
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 46360d413f676e6420f28b94b5ba91ec9237e681
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59129842"
---
# <a name="plannerbucket-resource-type"></a>Tipo de recurso plannerBucket

Namespace: microsoft.graph

O **recurso plannerBucket** representa um bucket (ou "coluna personalizada") para tarefas em um plano em Microsoft 365. Ele está contido em um [plannerPlan](plannerplan.md) e pode ter uma coleção de [plannerTasks](plannertask.md).



## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter plannerBucket](../api/plannerbucket-get.md) | [plannerBucket](plannerbucket.md) |Ler propriedades e relações do **objeto plannerBucket.**|
|[Listar plannerTasks](../api/plannerbucket-list-tasks.md) |Coleção [plannerTask](plannertask.md)| Obter uma coleção de objetos **plannerTask**.|
|[Criar](../api/planner-post-buckets.md) | [plannerBucket](plannerbucket.md)   | Crie um novo **objeto plannerBucket.** |
|[Atualizar](../api/plannerbucket-update.md) | [plannerBucket](plannerbucket.md)   |Atualizar **o objeto plannerBucket.** |
|[Delete](../api/plannerbucket-delete.md) | Nenhum(a) |Excluir **objeto plannerBucket.** |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|String| Somente leitura. ID do bucket. Tem 28 caracteres e diferencia maiúsculas de minúsculas. [Formatar validação](planner-identifiers-disclaimer.md) é feito no serviço.|
|nome|String|Nome do bucket.|
|orderHint|String|Dica usada para ordenar itens deste tipo em um modo de exibição de lista. O formato é definido como descrito [aqui](planner-order-hint-format.md).|
|planId|String|Planejar a ID à qual o bucket pertence.|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|tarefas|Coleção [plannerTask](plannertask.md)| Somente leitura. Anulável. A coleção de tarefas no bucket.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerBucket"
}-->

```json
{
  "id": "String (identifier)",
  "name": "String",
  "orderHint": "String",
  "planId": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerBucket resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

