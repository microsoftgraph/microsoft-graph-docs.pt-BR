---
title: Tipo de recurso printTask
description: Representa uma tarefa que está executando ou foi executada como resultado de um evento Impressão Universal.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 2026706ec46a2408d20231add8203d2f5a622c96
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516860"
---
# <a name="printtask-resource-type"></a>Tipo de recurso printTask

Namespace: microsoft.graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

Representa uma tarefa que está executando ou foi executada como resultado de um evento Impressão Universal.

Para obter detalhes sobre como usar esse recurso para adicionar suporte à impressão pull à Impressão Universal, consulte [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
| [Lista (de printTaskDefintion)](../api/printtaskdefinition-list-tasks.md) | [printTask](printtask.md) | Obter uma lista de tarefas que foram criadas com base em uma determinada printTaskDefinition. A lista inclui tarefas executadas no momento e tarefas concluídas recentemente. |
| [Get](../api/printtask-get.md) | [printTask](printtask.md) | Obter detalhes sobre uma tarefa de impressão. |
| [Update](../api/printtaskdefinition-update-task.md) | [printTask](printtask.md) | Atualiza uma tarefa de impressão. |

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O identificador printTask. Somente leitura.|
|status|[printTaskStatus](printtaskstatus.md)|O status de execução atual deste printTask. **O aplicativo de chamada é responsável por atualizar esse status ao terminar o processamento, a menos que a impressão relacionadaJob tenha sido redirecionada para outra impressora.** A falha na conclusão do relatório resultará no bloqueio do trabalho de impressão relacionado à impressão e, eventualmente, excluído. |
|parentUrl|Cadeia de caracteres|A URL da entidade de impressão que disparou essa tarefa. Por exemplo, `https://graph.microsoft.com/v1.0/print/printers/{printerId}/jobs/{jobId}`. Somente leitura.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|trigger|[printTaskTrigger](printtasktrigger.md)|O printTaskTrigger que disparou a execução dessa tarefa. Somente leitura.|
|definition|[printTaskDefinition](printtaskdefinition.md)|A printTaskDefinition usada para criar essa tarefa. Somente leitura.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.printTask",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printTask",
  "id": "String (identifier)",
  "status": {
    "@odata.type": "microsoft.graph.printTaskStatus"
  },
  "parentUrl": "String"
}
```

