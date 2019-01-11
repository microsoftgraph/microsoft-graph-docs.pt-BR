---
title: Tipo de recurso plannerOrderHintsByAssignee
description: O **plannerOrderHintsByAssignee** é um recurso que contém as dicas de ordenação para os destinatários em um recurso de plannerTask, para indicar a ordem da tarefa no modo do conselho tarefa atribuída a.
localization_priority: Normal
ms.openlocfilehash: cdc254eab43972d321e01e646880b3087f3af6f5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27863942"
---
# <a name="plannerorderhintsbyassignee-resource-type"></a>Tipo de recurso plannerOrderHintsByAssignee

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

O **plannerOrderHintsByAssignee** é um recurso que contém [dicas de ordenação](planner-order-hint-format.md) para os destinatários em um recurso [plannerTask](plannertask.md) para indicar a ordem da Tarefa no modo de exibição AssignedTo do Quadro de Tarefas. Este é um Tipo Aberto. As propriedades são as identificações dos usuários atribuídos à tarefa, e os valores são as dicas de ordem.

## <a name="properties"></a>Propriedades
As propriedades de um Tipo Aberto podem ser definidas pelo cliente. Nesse caso, o cliente deve fornecer as identificações dos usuários atribuídos à tarefa, como nomes de propriedades e uma [dica de ordem](planner-order-hint-format.md) válida como o valor. As propriedades não podem ser removidas deste tipo. O serviço automaticamente removerá os valores à medida que as atribuições existentes no objeto [plannerTask](plannertask.md) forem atualizadas.

Exemplo:

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
