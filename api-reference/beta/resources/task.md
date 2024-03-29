---
title: tipo de recurso de tarefa
description: Representa uma tarefa, como um item pessoal ou de trabalho, que pode ser rastreada e concluída.
author: avijityadav
ms.localizationpriority: medium
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 6d07d876535115c26b42d808e6870ec65f5dd2eb
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/01/2022
ms.locfileid: "65821236"
---
# <a name="task-resource-type-deprecated"></a>tipo de recurso de tarefa (preterido)

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [todo-deprecate-basetaskapi](../includes/todo-deprecate-basetaskapi.md)]

Representa uma tarefa, como um item pessoal ou de trabalho, que pode ser rastreada e concluída. Uma **tarefa** está sempre contida em uma [lista de tarefas base](basetasklist.md). 

Esse recurso dá suporte ao seguinte:
* Adicionar seus dados como propriedades personalizadas [em extensões abertas](/graph/extensibility-overview).
* Assinar as [notificações de alteração](/graph/webhooks).
* Usando [a consulta delta para](/graph/delta-query-overview) acompanhar adições incrementais, exclusões e atualizações.

Herda de [baseTask](../resources/basetask.md).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar tarefas](../api/basetasklist-list-tasks.md)|[coleção de](../resources/task.md) tarefas|Obtenha uma lista dos objetos [de tarefa](../resources/task.md) e suas propriedades.|
|[Obter tarefa](../api/basetask-get.md)|[tarefa](../resources/task.md)|Leia as propriedades e as relações de um [objeto de](../resources/task.md) tarefa.|
|[Atualizar tarefa](../api/basetask-update.md)|[tarefa](../resources/task.md)|Atualize as propriedades de um [objeto de](../resources/task.md) tarefa.|
|[Excluir tarefa](../api/basetask-delete.md)|Nenhum|Exclui um objeto [de](../resources/task.md) tarefa.|
|[move](../api/basetask-move.md)|[baseTask](../resources/basetask.md)|Mova a mensagem para uma lista diferente.|
|[Listar checklistItems](../api/todotask-list-checklistitems.md)|[coleção checklistItem](../resources/checklistitem.md)|Obtenha os recursos checklistItem da propriedade de navegação checklistItems.|
|[Criar checklistItem](../api/todotask-post-checklistitems.md)|[checklistItem](../resources/checklistitem.md)|Crie um novo objeto checklistItem.|
|[Listar linkedResources](../api/basetask-list-linkedresources.md)|[linkedResource_v2](../resources/linkedresource_v2.md) coleção|Obtenha os linkedResource_v2 da propriedade de navegação linkedResources.|
|[Criar linkedResource](../api/basetask-post-linkedresources.md)|[linkedResource_v2](../resources/linkedresource_v2.md)|Crie um novo linkedResource_v2 objeto.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|Textbody|[itemBody](../resources/itembody.md)|O corpo da tarefa no formato de texto que normalmente contém informações sobre a tarefa. Herdado de [baseTask](../resources/basetask.md).|
|bodyLastModifiedDateTime|DateTimeOffset|A data e hora da última modificação da tarefa. Por padrão, está definida em UTC. Você pode fornecer um fuso horário personalizado no cabeçalho da solicitação. O valor da propriedade usa o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1º de janeiro de 2020 teria esta aparência: '2020-01-01T00:00:00Z'. Herdado de [baseTask](../resources/basetask.md).|
|completedDateTime|DateTimeOffset|A data em que a tarefa foi concluída. Herdado de [baseTask](../resources/basetask.md).|
|createdDateTime|DateTimeOffset|A data e a hora da criação da tarefa. Por padrão, está definida em UTC. Você pode fornecer um fuso horário personalizado no cabeçalho da solicitação. O valor da propriedade usa o formato ISO 8601. Por exemplo, meia-noite UTC em 1º de janeiro de 2020 teria esta aparência: '2020-01-01T00:00:00Z'. Herdado de [baseTask](../resources/basetask.md).|
|displayName|Cadeia de caracteres|O nome da tarefa. Herdado de [baseTask](../resources/basetask.md).|
|dueDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)|A data no fuso horário especificado que a tarefa será concluída. Herdado de [baseTask](../resources/basetask.md).|
|id|Cadeia de caracteres|Identificador exclusivo para a tarefa. Por padrão, esse valor não será alterado se uma tarefa for movida de uma lista para outra. Herdado de [baseTask](../resources/basetask.md).|
|importância|importância|A importância da tarefa. Os valores possíveis são: `low`, `normal`, `high`. Herdado de [baseTask](../resources/basetask.md). Os valores possíveis são: `low`, `normal`, `high`.|
|lastModifiedDateTime|DateTimeOffset|A data e hora da última modificação da tarefa. Por padrão, está definida em UTC. Você pode fornecer um fuso horário personalizado no cabeçalho da solicitação. O valor da propriedade usa o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1º de janeiro de 2020 teria esta aparência: '2020-01-01T00:00:00Z'. Herdado de [baseTask](../resources/basetask.md).|
|Vista|[taskViewpoint](../resources/taskviewpoint.md)|Propriedades que são pessoais para um usuário, como **reminderDateTime** e **categorias**. Herdado de [baseTask](../resources/basetask.md).|
|recurrence|[patternedRecurrence](../resources/patternedrecurrence.md)|O padrão de recorrência da tarefa. Herdado de [baseTask](../resources/basetask.md).|
|startDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)|A data no fuso horário especificado que a tarefa será iniciada. Herdado de [baseTask](../resources/basetask.md).|
|status|taskStatus_v2|Indica o estado ou o andamento da tarefa. Os valores possíveis são: `notStarted`, `inProgress`, `completed`,`unknownFutureValue`. Herdado de [baseTask](../resources/basetask.md).|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|checklistItems|[coleção checklistItem](../resources/checklistitem.md)|Uma coleção de checklistItems vinculados a uma tarefa. Herdado de [baseTask](../resources/basetask.md)|
|extensions|Coleção [extension](../resources/extension.md)|A coleção de extensões abertas definidas para a tarefa. Herdado de [baseTask](../resources/basetask.md)|
|Linkedresources|[linkedResource_v2](../resources/linkedresource_v2.md) coleção|Uma coleção de recursos vinculados à tarefa. Herdado de [baseTask](../resources/basetask.md)|
|parentList|[baseTaskList](../resources/basetasklist.md)|A lista que contém a tarefa. Herdado de [baseTask](../resources/basetask.md)|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.task",
  "baseType": "microsoft.graph.baseTask",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.task",
  "textBody": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "bodyLastModifiedDateTime": "String (timestamp)",
  "completedDateTime": "String (timestamp)",
  "dueDateTime": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone"
  },
  "startDateTime": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone"
  },
  "importance": "String",
  "recurrence": {
    "@odata.type": "microsoft.graph.patternedRecurrence"
  },
  "displayName": "String",
  "status": "String",
  "viewpoint": {
    "@odata.type": "microsoft.graph.taskViewpoint"
  },
  "id": "String (identifier)"
}
```

