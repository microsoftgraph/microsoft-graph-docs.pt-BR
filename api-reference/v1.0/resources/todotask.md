---
title: Tipo de recurso todoTask
description: Um recurso todoTask rastreia um item de trabalho.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 043ba3e419db0ea3854a0f462b32553d288e25a11e1c27ea6dc9a7f7ad933095
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54196471"
---
# <a name="todotask-resource-type"></a>Tipo de recurso todoTask

Namespace: microsoft.graph

Um **todoTask** representa uma tarefa, como um item pessoal ou de trabalho, que pode ser rastreada e concluída. 

Um **todoTask** está sempre contido em [um todoTaskList](todotasklist.md). Ele inclui uma relação com uma coleção de [objetos linkedResource,](./linkedResource.md) acompanhando uma ou mais fontes da tarefa.

Esse recurso dá suporte ao seguinte:
* Adicionar seus dados como propriedades personalizadas em [extensões abertas.](/graph/extensibility-overview)
* Usando [a consulta delta para](/graph/delta-query-overview) rastrear adições incrementais, exclusões e atualizações.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar tarefas](../api/todotasklist-list-tasks.md)|Coleção [todoTask](todotask.md)|Obtenha todos os recursos [todoTask](todotask.md) na lista especificada.|
|[Criar tarefa](../api/todotasklist-post-tasks.md)|[todoTask](todotask.md)| Criar um [todoTask](todotask.md) na lista de tarefas especificada|
|[Obter tarefa](../api/todotask-get.md)|[todoTask](../resources/todotask.md)|Leia as propriedades e as relações de um [objeto todoTask.](../resources/todotask.md)|
|[Atualizar tarefa](../api/todotask-update.md)|[todoTask](../resources/todotask.md)|Atualize as propriedades de um [objeto todoTask.](../resources/todotask.md)|
|[Excluir tarefa](../api/todotask-delete.md)|None|Exclui um [objeto todoTask.](../resources/todotask.md)|
|[Listar linkedResources](../api/todotask-list-linkedresources.md)|[Coleção linkedResource](../resources/linkedresource.md)|Obter o linkedResources da propriedade de navegação linkedResources.|
|[Criar linkedResources](../api/todotask-post-linkedresources.md)|[linkedResource](../resources/linkedresource.md)|Crie um novo objeto linkedResources.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|corpo|[itemBody](../resources/itembody.md)|Corpo da tarefa que normalmente contém informações sobre a tarefa.|
|bodyLastModifiedDateTime|DateTimeOffset|A data e hora da última modificação da tarefa. Por padrão, está definida em UTC. Você pode fornecer um fuso horário personalizado no cabeçalho da solicitação. O valor da propriedade usa o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1º de janeiro de 2020 teria esta aparência: '2020-01-01T00:00:00Z'.|
|completedDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)|A data no fuso horário especificado que a tarefa foi concluída.|
|createdDateTime|DateTimeOffset|A data e a hora da criação da tarefa. Por padrão, está definida em UTC. Você pode fornecer um fuso horário personalizado no cabeçalho da solicitação. O valor da propriedade usa o formato ISO 8601. Por exemplo, meia-noite UTC em 1º de janeiro de 2020 teria esta aparência: '2020-01-01T00:00:00Z'.|
|dueDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)|A data no fuso horário especificado que a tarefa será concluída.|
|id|Cadeia de caracteres|Identificador exclusivo para a tarefa. Por padrão, esse valor muda quando o item é movido de uma lista para outra.|
|importância|importância|A importância da tarefa. Os valores possíveis são: `low`, `normal`, `high`.|
|isReminderOn|Booliano|Definido como verdadeiro se um alerta é definido para lembrar o usuário da tarefa.|
|lastModifiedDateTime|DateTimeOffset|A data e hora da última modificação da tarefa. Por padrão, está definida em UTC. Você pode fornecer um fuso horário personalizado no cabeçalho da solicitação. O valor da propriedade usa o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1º de janeiro de 2020 teria esta aparência: '2020-01-01T00:00:00Z'.|
|recurrence|[patternedRecurrence](../resources/patternedrecurrence.md)|O padrão de recorrência da tarefa.|
|reminderDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)|A data e hora do alerta de lembrete da tarefa.|
|status|taskStatus|Indica o estado ou o andamento da tarefa. Os valores possíveis são: `notStarted`, `inProgress`, `completed`, `waitingOnOthers`, `deferred`.|
|title|Cadeia de caracteres|Uma breve descrição da tarefa.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|extensions|[extension](extension.md) collection| A coleção de extensões abertas definidas para a tarefa. Anulável.|
|linkedResources|[Coleção linkedResource](../resources/linkedresource.md)|Uma coleção de recursos vinculados à tarefa.|


## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.todoTask",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.todoTask",
  "id": "String (identifier)",
  "body": {
    "@odata.type": "microsoft.graph.itemBody"
  },
  "completedDateTime": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone"
  },
  "dueDateTime": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone"
  },
  "importance": "String",
  "isReminderOn": "Boolean",
  "recurrence": {
    "@odata.type": "microsoft.graph.patternedRecurrence"
  },
  "reminderDateTime": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone"
  },
  "status": "String",
  "title": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "bodyLastModifiedDateTime": "String (timestamp)"
}
```



