---
title: Tipo de recurso printTaskDefinition
description: Representa uma tarefa que pode ser disparada quando vários eventos ocorrem em Impressão Universal.
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 2495825ec64d73bb440d16e4eae9125f8dbd38eb
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2021
ms.locfileid: "51766305"
---
# <a name="printtaskdefinition-resource-type"></a>Tipo de recurso printTaskDefinition

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma definição abstrata para uma tarefa que pode ser disparada quando vários eventos ocorrem em Impressão Universal.

Para obter detalhes sobre como usar esse recurso para adicionar suporte à impressão pull à Impressão Universal, consulte [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).

Esse recurso permite:
* [Assinatura para alterar notificações](/graph/universal-print-webhook-notifications).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [List](../api/print-list-taskdefinitions.md) | [Coleção printTaskDefinition](printtaskdefinition.md) | Obter uma lista completa de printTaskDefinitions criados em Impressão Universal. |
| [Create](../api/print-post-taskdefinitions.md) | [printTaskDefinition](printtaskdefinition.md) | Crie uma nova printTaskDefinition. |
| [Atualizar](../api/print-update-taskdefinition.md) | [printTaskDefinition](printtaskdefinition.md) | Atualize um printTaskDefinition. |
| [Delete](../api/print-delete-taskdefinition.md) | Nenhum | Exclua um printTaskDefinition. |
| [Listar tarefas](../api/printtaskdefinition-list-tasks.md) | [printTask](printtask.md) | Obter uma lista de tarefas que foram criadas com base nessa definição. A lista inclui tarefas executadas no momento e tarefas concluídas recentemente. |
| [Obter tarefa](../api/printtask-get.md) | [printTask](printtask.md) | Obtém uma tarefa que foi criada com base nessa definição. |
| [Atualizar tarefa](../api/printtaskdefinition-update-task.md) | [printTask](printtask.md) | Atualize uma tarefa criada com base nessa definição. **Os aplicativos que registram gatilhos de tarefas são responsáveis por atualizar o status da tarefa ao terminar o processamento, a menos que a impressão relacionadaJob tenha sido redirecionada para outra impressora.** A falha na conclusão do relatório resultará no bloqueio do trabalho de impressão relacionado à impressão e, eventualmente, excluído. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|String|O identificador printTaskDefinition. Somente leitura.|
|displayName|String|O nome da printTaskDefinition.|
|createdBy|[appIdentity](appidentity.md)|O aplicativo que criou o printTaskDefinition. Somente leitura.|

## <a name="relationships"></a>Relações
| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|tarefas|[Coleção printTask](printtask.md)|Uma lista de tarefas que foram criadas com base nessa definição. A lista inclui tarefas executadas no momento e tarefas concluídas recentemente. Somente leitura.|

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

