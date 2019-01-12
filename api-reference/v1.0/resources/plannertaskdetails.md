---
title: Tipo de recurso plannerTaskDetails
description: O recurso **plannerTaskDetails** representa as informações adicionais sobre uma tarefa. Cada objeto task tem um objeto de detalhes.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 75e17200dc52fff385c7be8fb0269a3da20464b8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27956007"
---
# <a name="plannertaskdetails-resource-type"></a>Tipo de recurso plannerTaskDetails

O recurso **plannerTaskDetails** representa as informações adicionais sobre uma tarefa. Cada objeto [task](plannertask.md) tem um objeto de detalhes.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Get plannerTaskDetails](../api/plannertaskdetails-get.md) | [plannerTaskDetails](plannertaskdetails.md) |Leia as propriedades e as relações do objeto **plannerTaskDetails**.|
|[Atualizar](../api/plannertaskdetails-update.md) | [plannerTaskDetails](plannertaskdetails.md)    |Atualize o objeto **plannerTaskDetails**. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|lista de verificação|[plannerChecklistItems](plannerchecklistitems.md)|A coleção de itens da lista de verificação na tarefa.|
|description|String|Descrição da tarefa|
|id|String| Somente leitura. ID dos detalhes da tarefa. É 28 caracteres longos e diferencia maiusculas de minúsculas. [Validação de formato](planner-identifiers-disclaimer.md) é feita no serviço.|
|previewType|string|Isto define o tipo de visualização que aparecerá na tarefa. Os valores possíveis são: `automatic`, `noPreview`, `checklist`, `description`, `reference`. Quando definido como `automatic` a visualização exibida for escolhida pelo app exibindo a tarefa.|
|referências|[plannerExternalReferences](plannerexternalreferences.md)|A coleção de referências na tarefa.|

## <a name="relationships"></a>Relações
Nenhum


## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.plannerTaskDetails"
}-->

```json
{
  "checklist": {"@odata.type": "microsoft.graph.plannerChecklistItems"},
  "description": "String",
  "id": "String (identifier)",
  "previewType": "string",
  "references": {"@odata.type": "microsoft.graph.plannerExternalReferences"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerTaskDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
