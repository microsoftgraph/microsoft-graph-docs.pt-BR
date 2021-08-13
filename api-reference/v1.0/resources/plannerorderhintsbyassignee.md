---
title: Tipo de recurso plannerOrderHintsByAssignee
description: O **plannerOrderHintsByAssignee** é um recurso que contém dicas de ordenação para os atribuídos em um recurso plannerTask, para indicar a ordem da tarefa em Atribuído a modo de exibição do Quadro de Tarefas.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 9ddfe9f30387d66e6a55da680eb176d5d20f8e33e44f6f827e84efe687d29e92
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54146325"
---
# <a name="plannerorderhintsbyassignee-resource-type"></a>Tipo de recurso plannerOrderHintsByAssignee

Namespace: microsoft.graph

O **plannerOrderHintsByAssignee** é um recurso que contém dicas de ordenação para os [atribuídos](planner-order-hint-format.md) em um [recurso plannerTask,](plannertask.md) para indicar a ordem da tarefa em Atribuído a modo de exibição do Quadro de Tarefas.
Esse tipo é um tipo aberto. As propriedades são as ids dos usuários atribuídos à tarefa e os valores são dicas de ordem.

## <a name="properties"></a>Propriedades
As propriedades de um Tipo Aberto podem ser definidas pelo cliente. Nesse caso, o cliente deve fornecer ids de usuários atribuídos à tarefa como nomes de propriedade e uma dica de ordem [válida](planner-order-hint-format.md) como o valor.
As propriedades não podem ser removidas desse tipo. O serviço removerá automaticamente os valores à medida que as atribuições no [plannerTask](plannertask.md) que contêm são atualizadas.

Exemplo:

<!-- {
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [ "ca2a1df2-e36b-4987-9f6b-0ea462f4eb47", "4e98f8f1-bb03-4015-b8e0-19bb370949d8" ],
  "@odata.type": "microsoft.graph.plannerOrderHintsByAssignee"
}-->

```json
{
  "ca2a1df2-e36b-4987-9f6b-0ea462f4eb47": "String",
  "4e98f8f1-bb03-4015-b8e0-19bb370949d8": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerOrderHintsByAssignee resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

