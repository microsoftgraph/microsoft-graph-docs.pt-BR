---
title: Tipo de recurso printTask
description: Representa uma tarefa que está executando ou foi executada como resultado de um evento Impressão Universal.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: c684ff64aa4c3667214b61b70a422690381525b3
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2021
ms.locfileid: "51766298"
---
# <a name="printtask-resource-type"></a>Tipo de recurso printTask

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma tarefa que está executando ou foi executada como resultado de um evento Impressão Universal.

Para obter detalhes sobre como usar esse recurso para adicionar suporte à impressão pull à Impressão Universal, consulte [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Lista (de printTaskDefintion)](../api/printtaskdefinition-list-tasks.md) | [printTask](printtask.md) | Obter uma lista de tarefas que foram criadas com base em uma determinada printTaskDefinition. A lista inclui tarefas executadas no momento e tarefas concluídas recentemente. |
| [Get](../api/printtask-get.md) | [printTask](printtask.md) | Obter detalhes sobre uma tarefa de impressão. |
| [Atualizar](../api/printtaskdefinition-update-task.md) | [printTask](printtask.md) | Atualiza uma tarefa de impressão. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|String|O identificador printTask. Somente leitura.|
|status|[printTaskStatus](printtaskstatus.md)|O status de execução atual deste printTask. **O aplicativo de chamada é responsável por atualizar esse status ao terminar o processamento, a menos que a impressão relacionadaJob tenha sido redirecionada para outra impressora.** A falha na conclusão do relatório resultará no bloqueio do trabalho de impressão relacionado à impressão e, eventualmente, excluído. |
|parentUrl|String|A URL da entidade de impressão que disparou essa tarefa. Por exemplo, `https://graph.microsoft.com/beta/print/printers/{printerId}/jobs/{jobId}`. Somente leitura.|

## <a name="relationships"></a>Relações
| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|trigger|[printTaskTrigger](printtasktrigger.md)|O printTaskTrigger que disparou a execução dessa tarefa. Somente leitura.|
|definition|[printTaskDefinition](printtaskdefinition.md)|A printTaskDefinition usada para criar essa tarefa. Somente leitura.|

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


