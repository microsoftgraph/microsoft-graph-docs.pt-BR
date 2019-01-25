---
title: Tipo de recurso planner
description: O recurso **planner** é o ponto de entrada do modelo de objeto do Planner. Ele retorna um único recurso **planner**.  Ele não contém quaisquer propriedades utilizáveis.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 50ceb8b76b398bd5898e48f31df9a6443569781e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523397"
---
# <a name="planner-resource-type"></a>Tipo de recurso planner

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O recurso **planner** é o ponto de entrada do modelo de objeto do Planner. Ele retorna um único recurso **planner**.  Ele não contém quaisquer propriedades utilizáveis.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Criar plannerBucket](../api/planner-post-buckets.md) |[plannerBucket](plannerbucket.md)| Crie um novo **plannerBucket** ao postar na coleção de buckets.|
|[Criar plannerPlan](../api/planner-post-plans.md) |[plannerPlan](plannerplan.md)| Crie um novo **plannerPlan** ao postar na coleção de planos.|
|[Criar plannerTask](../api/planner-post-tasks.md) |[plannerTask](plannertask.md)| Crie um novo **plannerTask** ao postar na coleção de tarefas.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|String| Somente leitura. O identificador do recurso **planner**|

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
  "optionalProperties": [

  ],
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
  "suppressions": [
    "Error: /api-reference/beta/resources/planner.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
