---
title: tipo de recurso printTaskDefinition
description: Representa uma tarefa que pode ser disparada quando vários eventos ocorrem dentro da impressão universal.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 013d2756455abebc0f20bbe5a1d186a0a4d65648
ms.sourcegitcommit: 8a74c06be9c41390331ca1717efedc5b5a244db5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2020
ms.locfileid: "45091546"
---
# <a name="printtaskdefinition-resource-type"></a>tipo de recurso printTaskDefinition

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma definição abstrata de uma tarefa que pode ser disparada quando vários eventos ocorrem dentro da impressão universal.

Para obter detalhes sobre como usar esse recurso para adicionar suporte à impressão pull à impressão universal, consulte [estender a impressão universal para dar suporte à impressão pull](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Listar](../api/print-list-taskdefinitions.md) | coleção [printTaskDefinition](printtaskdefinition.md) | Obtenha uma lista completa de printTaskDefinitions criadas dentro da impressão universal. |
| [Criar](../api/print-post-taskdefinitions.md) | [printTaskDefinition](printtaskdefinition.md) | Criar um novo printTaskDefinition. |
| [Update](../api/print-update-taskdefinition.md) | [printTaskDefinition](printtaskdefinition.md) | Atualizar um printTaskDefinition. |
| [Delete](../api/print-delete-taskdefinition.md) | Nenhum | Excluir um printTaskDefinition. |
| [Listar tarefas](../api/printtaskdefinition-list-tasks.md) | [multitarefa](printtask.md) | Obtém uma lista de tarefas que foram criadas com base nessa definição. A lista inclui tarefas em execução no momento e tarefas concluídas recentemente. |
| [Obter tarefa](../api/printtask-get.md) | [multitarefa](printtask.md) | Obtém uma tarefa que foi criada com base nessa definição. |
| [Atualizar tarefa](../api/printtaskdefinition-update-task.md) | Nenhum | Atualizar uma tarefa que foi criada com base nessa definição. **Os aplicativos que registram gatilhos de tarefa são responsáveis por atualizar o status da tarefa quando o processamento é concluído, a menos que o printJob relacionado tenha sido Redirecionado para outra impressora.** A falha na conclusão do relatório fará com que o trabalho de impressão relacionado seja bloqueado da impressão e, eventualmente, excluído. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|String|O identificador do printTaskDefinition. Somente leitura.|
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