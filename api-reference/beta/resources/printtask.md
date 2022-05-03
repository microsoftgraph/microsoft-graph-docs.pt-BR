---
title: Tipo de recurso printTask
description: Representa uma tarefa que está em execução ou foi executada como resultado de um evento de Impressão Universal.
author: braedenp-msft
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 4348a07af0849359c72c6b28fa5ef665420a2842
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176747"
---
# <a name="printtask-resource-type"></a>Tipo de recurso printTask

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma tarefa que está em execução ou foi executada como resultado de um evento de Impressão Universal.

Para obter detalhes sobre como usar esse recurso para adicionar suporte de impressão pull à Impressão Universal, consulte Estendendo Impressão Universal para dar suporte [à impressão pull](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Lista (de printTaskDefintion)](../api/printtaskdefinition-list-tasks.md) | [printTask](printtask.md) | Obtenha uma lista de tarefas que foram criadas com base em uma determinada printTaskDefinition. A lista inclui tarefas em execução no momento e tarefas concluídas recentemente. |
| [Get](../api/printtask-get.md) | [printTask](printtask.md) | Obter detalhes sobre uma tarefa de impressão. |
| [Atualizar](../api/printtaskdefinition-update-task.md) | [printTask](printtask.md) | Atualiza uma tarefa de impressão. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|Cadeia de caracteres|O identificador de printTask. Somente leitura.|
|status|[printTaskStatus](printtaskstatus.md)|O status de execução atual dessa printTask. **O aplicativo de chamada é responsável por atualizar esse status quando o processamento for concluído, a menos que o printJob relacionado tenha sido redirecionado para outra impressora.** A falha ao relatar a conclusão fará com que o trabalho de impressão relacionado seja impedido de imprimir e, eventualmente, excluído. |
|parentUrl|Cadeia de Caracteres|A URL da entidade de impressão que disparou essa tarefa. Por exemplo, `https://graph.microsoft.com/beta/print/printers/{printerId}/jobs/{jobId}`. Somente leitura.|

## <a name="relationships"></a>Relações
| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|Gatilho|[printTaskTrigger](printtasktrigger.md)|O printTaskTrigger que disparou a execução dessa tarefa. Somente leitura.|
|Definição|[printTaskDefinition](printtaskdefinition.md)|A printTaskDefinition que foi usada para criar essa tarefa. Somente leitura.|

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


