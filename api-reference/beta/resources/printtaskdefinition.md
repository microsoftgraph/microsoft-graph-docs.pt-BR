---
title: Tipo de recurso printTaskDefinition
description: Representa uma tarefa que pode ser disparada quando vários eventos ocorrem na Impressão Universal.
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: bbffceb08be336cd816d80f03236078b39348339
ms.sourcegitcommit: 744c2d8be5a1ce158068bcfeaad1aabf8166c556
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/22/2021
ms.locfileid: "49934853"
---
# <a name="printtaskdefinition-resource-type"></a>Tipo de recurso printTaskDefinition

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma definição abstrata para uma tarefa que pode ser disparada quando vários eventos ocorrem na Impressão Universal.

Para obter detalhes sobre como usar esse recurso para adicionar suporte de impressão pull à Impressão Universal, consulte Estendendo a impressão universal para dar suporte [à impressão pull.](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)

Esse recurso permite:
* [Assinatura para alterar notificações](/graph/universal-print-webhook-notifications).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [List](../api/print-list-taskdefinitions.md) | [Coleção printTaskDefinition](printtaskdefinition.md) | Obter uma lista completa de printTaskDefinitions criadas na Impressão Universal. |
| [Create](../api/print-post-taskdefinitions.md) | [printTaskDefinition](printtaskdefinition.md) | Crie uma nova printTaskDefinition. |
| [Update](../api/print-update-taskdefinition.md) | [printTaskDefinition](printtaskdefinition.md) | Atualize uma printTaskDefinition. |
| [Delete](../api/print-delete-taskdefinition.md) | Nenhum | Exclua uma printTaskDefinition. |
| [Listar tarefas](../api/printtaskdefinition-list-tasks.md) | [printTask](printtask.md) | Obter uma lista de tarefas que foram criadas com base nessa definição. A lista inclui tarefas em execução no momento e tarefas concluídas recentemente. |
| [Obter tarefa](../api/printtask-get.md) | [printTask](printtask.md) | Obtém uma tarefa que foi criada com base nessa definição. |
| [Atualizar tarefa](../api/printtaskdefinition-update-task.md) | Nenhum | Atualize uma tarefa que foi criada com base nessa definição. **Os aplicativos que registram gatilhos de tarefa são responsáveis por atualizar o status da tarefa quando o processamento é concluído, a menos que o printJob relacionado tenha sido redirecionado para outra impressora.** A falha ao relatar a conclusão fará com que o trabalho de impressão relacionado seja impedido de imprimir e, eventualmente, excluído. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|Cadeia de caracteres|O identificador de printTaskDefinition. Somente leitura.|
|displayName|Cadeia de caracteres|O nome da printTaskDefinition.|
|createdBy|[appIdentity](appidentity.md)|O aplicativo que criou a printTaskDefinition. Somente leitura.|

## <a name="relationships"></a>Relações
| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|tarefas|[Coleção printTask](printtask.md)|Uma lista de tarefas que foram criadas com base nessa definição. A lista inclui tarefas em execução no momento e tarefas concluídas recentemente. Somente leitura.|

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

