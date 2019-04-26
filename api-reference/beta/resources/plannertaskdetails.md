---
title: tipo de recurso plannerTaskDetails
description: O recurso **plannerTaskDetails** representa as informações adicionais sobre uma tarefa. Cada objeto Task tem um objeto details.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 579ecdbf43275de90468883d158af725eb1d1734
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563597"
---
# <a name="plannertaskdetails-resource-type"></a>tipo de recurso plannerTaskDetails

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O recurso **plannerTaskDetails** representa as informações adicionais sobre uma tarefa. Cada objeto [Task](plannertask.md) tem um objeto details.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter plannerTaskDetails](../api/plannertaskdetails-get.md) | [plannerTaskDetails](plannertaskdetails.md) |Leia as propriedades e os relacionamentos do objeto **plannerTaskDetails** .|
|[Update](../api/plannertaskdetails-update.md) | [plannerTaskDetails](plannertaskdetails.md)    |Atualize o objeto **plannerTaskDetails** . |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|verificação|[plannerChecklistItems](plannerchecklistitems.md)|A coleção de itens de lista de verificação na tarefa.|
|description|String|Descrição da tarefa|
|id|String| Somente leitura. ID dos detalhes da tarefa. Tem 28 caracteres e diferencia maiúsculas de minúsculas. [Formatar validação](tasks-identifiers-disclaimer.md) é feito no serviço.|
|previewType|string|Isso define o tipo de visualização que aparece na tarefa. Os valores possíveis são: `automatic`, `noPreview`, `checklist`, `description`, `reference`. Quando definido para `automatic` a visualização exibida é escolhido pelo aplicativo que está exibindo a tarefa.|
|Referencie|[plannerExternalReferences](plannerexternalreferences.md)|A coleção de referências na tarefa.|

## <a name="relationships"></a>Relações
Nenhum


## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
<!--
{
  "type": "#page.annotation",
  "description": "plannerTaskDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
