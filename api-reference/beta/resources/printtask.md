---
title: tipo de recurso de multitarefa
description: Representa uma tarefa que está em execução ou foi executada como resultado de um evento de impressão universal.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: fb41bc68112aa04e1eea825d45982f2f3f0db48c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47973789"
---
# <a name="printtask-resource-type"></a>tipo de recurso de multitarefa

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma tarefa que está em execução ou foi executada como resultado de um evento de impressão universal.

Para obter detalhes sobre como usar esse recurso para adicionar suporte à impressão pull à impressão universal, consulte [estender a impressão universal para dar suporte à impressão pull](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).

## <a name="methods"></a>Methods

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Lista (de printTaskDefintion)](../api/printtaskdefinition-list-tasks.md) | [printTask](printtask.md) | Obter uma lista de tarefas que foram criadas com base em um determinado printTaskDefinition. A lista inclui tarefas em execução no momento e tarefas concluídas recentemente. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|String|O identificador da tarefa. Somente leitura.|
|status|[printTaskStatus](printtaskstatus.md)|O status de execução atual desta multitarefa. **O aplicativo de chamada é responsável por atualizar esse status quando o processamento for concluído, a menos que o printJob relacionado tenha sido Redirecionado para outra impressora.** A falha na conclusão do relatório fará com que o trabalho de impressão relacionado seja bloqueado da impressão e, eventualmente, excluído. |
|parentUrl|String|A URL da entidade de impressão que disparou essa tarefa. Por exemplo, `https://graph.microsoft.com/beta/print/printers/{printerId}/jobs/{jobId}`. Somente leitura.|

## <a name="relationships"></a>Relações
| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|dispara|[printTaskTrigger](printtasktrigger.md)|O printTaskTrigger que disparou a execução da tarefa. Somente leitura.|
|definir|[printTaskDefinition](printtaskdefinition.md)|O printTaskDefinition que foi usado para criar essa tarefa. Somente leitura.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printTask",
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity"
}-->

```json
{
  "id": "String (identifier)",
  "status": {"@odata.type": "microsoft.graph.printTaskStatus"},
  "parentUrl": "String",
  "trigger": {"@odata.type": "microsoft.graph.printTaskTrigger"},
  "definition": {"@odata.type": "microsoft.graph.printTaskDefinition"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printTask resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


