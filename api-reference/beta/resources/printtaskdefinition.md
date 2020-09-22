---
title: tipo de recurso printTaskDefinition
description: Representa uma tarefa que pode ser disparada quando vários eventos ocorrem dentro da impressão universal.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 970b4169dcf4d94eed01be7a15654daa51760151
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48078308"
---
# <a name="printtaskdefinition-resource-type"></a>tipo de recurso printTaskDefinition

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma definição abstrata de uma tarefa que pode ser disparada quando vários eventos ocorrem dentro da impressão universal.

Para obter detalhes sobre como usar esse recurso para adicionar suporte à impressão pull à impressão universal, consulte [estender a impressão universal para dar suporte à impressão pull](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [List](../api/print-list-taskdefinitions.md) | coleção [printTaskDefinition](printtaskdefinition.md) | Obtenha uma lista completa de printTaskDefinitions criadas dentro da impressão universal. |
| [Create](../api/print-post-taskdefinitions.md) | [printTaskDefinition](printtaskdefinition.md) | Criar um novo printTaskDefinition. |
| [Update](../api/print-update-taskdefinition.md) | [printTaskDefinition](printtaskdefinition.md) | Atualizar um printTaskDefinition. |
| [Delete](../api/print-delete-taskdefinition.md) | Nenhum | Excluir um printTaskDefinition. |
| [Listar tarefas](../api/printtaskdefinition-list-tasks.md) | [printTask](printtask.md) | Obtém uma lista de tarefas que foram criadas com base nessa definição. A lista inclui tarefas em execução no momento e tarefas concluídas recentemente. |
| [Obter tarefa](../api/printtask-get.md) | [printTask](printtask.md) | Obtém uma tarefa que foi criada com base nessa definição. |
| [Atualizar tarefa](../api/printtaskdefinition-update-task.md) | Nenhum | Atualizar uma tarefa que foi criada com base nessa definição. **Os aplicativos que registram gatilhos de tarefa são responsáveis por atualizar o status da tarefa quando o processamento é concluído, a menos que o printJob relacionado tenha sido Redirecionado para outra impressora.** A falha na conclusão do relatório fará com que o trabalho de impressão relacionado seja bloqueado da impressão e, eventualmente, excluído. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|Cadeia de caracteres|O identificador do printTaskDefinition. Somente leitura.|
|displayName|Cadeia de caracteres|O nome do printTaskDefinition.|
|createdBy|[appIdentity](appidentity.md)|O aplicativo que criou o printTaskDefinition. Somente leitura.|

## <a name="relationships"></a>Relações
| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|tarefas|coleção [multitask](printtask.md)|Uma lista de tarefas que foram criadas com base nessa definição. A lista inclui tarefas em execução no momento e tarefas concluídas recentemente. Somente leitura.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printTaskDefinition",
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity"
}-->

```json
{
  "id": "String (identifier)",
  "displayName": "String",
  "createdBy": {"@odata.type": "microsoft.graph.appIdentity"},
  "tasks": [{"@odata.type": "microsoft.graph.printTask"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printTaskDefinition resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

