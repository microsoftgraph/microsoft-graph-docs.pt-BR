---
title: Tipo de recurso printTaskDefinition
description: Representa uma tarefa que pode ser disparada quando vários eventos ocorrem em Impressão Universal.
author: nilakhan
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: d1173cfe72aacce5f422dc47c49f557e373c1ce2
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/12/2021
ms.locfileid: "60924191"
---
# <a name="printtaskdefinition-resource-type"></a>Tipo de recurso printTaskDefinition

Namespace: microsoft.graph

Representa uma definição abstrata para uma tarefa que pode ser disparada quando vários eventos ocorrem em Impressão Universal.

Para obter detalhes sobre como usar esse recurso para adicionar suporte à impressão pull à Impressão Universal, consulte [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).

Esse recurso permite:
* [Assinatura para alterar notificações](/graph/universal-print-webhook-notifications).

## <a name="methods"></a>Métodos
| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [List](../api/print-list-taskdefinitions.md) | [Coleção printTaskDefinition](printtaskdefinition.md) | Obter uma lista completa de printTaskDefinitions criados em Impressão Universal. |
| [Criar](../api/print-post-taskdefinitions.md) | [printTaskDefinition](printtaskdefinition.md) | Crie uma nova printTaskDefinition. |
| [Atualizar](../api/print-update-taskdefinition.md) | [printTaskDefinition](printtaskdefinition.md) | Atualize um printTaskDefinition. |
| [Delete](../api/print-delete-taskdefinition.md) | Nenhum(a) | Exclua um printTaskDefinition. |
| [Listar tarefas](../api/printtaskdefinition-list-tasks.md) | [printTask](printtask.md) | Obter uma lista de tarefas que foram criadas com base nessa definição. A lista inclui tarefas executadas no momento e tarefas concluídas recentemente. |
| [Obter tarefa](../api/printtask-get.md) | [printTask](printtask.md) | Obtém uma tarefa que foi criada com base nessa definição. |
| [Atualizar tarefa](../api/printtaskdefinition-update-task.md) | [printTask](printtask.md) | Atualize uma tarefa criada com base nessa definição. **Os aplicativos que registram gatilhos de tarefas são responsáveis por atualizar o status da tarefa ao terminar o processamento, a menos que a impressão relacionadaJob tenha sido redirecionada para outra impressora.** A falha na conclusão do relatório resultará no bloqueio do trabalho de impressão relacionado à impressão e, eventualmente, excluído. |

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O identificador printTaskDefinition. Somente leitura.|
|displayName|Cadeia de caracteres|O nome da printTaskDefinition.|
|createdBy|[appIdentity](appidentity.md)|O aplicativo que criou o printTaskDefinition. Somente leitura.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|tarefas|[Coleção printTask](printtask.md)|Uma lista de tarefas que foram criadas com base nessa definição. A lista inclui tarefas executadas no momento e tarefas concluídas recentemente. Somente leitura.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.printTaskDefinition",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printTaskDefinition",
  "id": "String (identifier)",
  "displayName": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.appIdentity"
  }
}
```

