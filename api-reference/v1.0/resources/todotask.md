---
title: Tipo de recurso todoTask
description: Um recurso todoTask rastreia um item de trabalho.
author: avijityadav
ms.localizationpriority: medium
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: a96121caaaee5c2ace12a1b73281e156829d9e3d
ms.sourcegitcommit: 84db9d70672e7a36a1130ff4f4b9baf3554d287f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2022
ms.locfileid: "66810239"
---
# <a name="todotask-resource-type"></a>Tipo de recurso todoTask

Namespace: microsoft.graph

Um **todoTask** representa uma tarefa, como um item pessoal ou de trabalho, que pode ser rastreada e concluída. 

Um **todoTask** está sempre contido em [um todoTaskList](todotasklist.md). Ele inclui uma relação com uma coleção de [objetos linkedResource](./linkedResource.md) , acompanhando uma ou mais fontes da tarefa.

Esse recurso dá suporte ao seguinte:
* Adicionar seus dados como propriedades personalizadas [em extensões abertas](/graph/extensibility-overview).
* Usando [a consulta delta para](/graph/delta-query-overview) acompanhar adições incrementais, exclusões e atualizações.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar tarefas](../api/todotasklist-list-tasks.md)|Coleção [todoTask](todotask.md)|Obtenha todos os recursos [todoTask](todotask.md) na lista especificada.|
|[Criar tarefa](../api/todotasklist-post-tasks.md)|[todoTask](todotask.md)| Criar um [todoTask](todotask.md) na lista de tarefas especificada|
|[Obter tarefa](../api/todotask-get.md)|[todoTask](../resources/todotask.md)|Leia as propriedades e as relações de um [objeto todoTask](../resources/todotask.md) .|
|[Atualizar tarefa](../api/todotask-update.md)|[todoTask](../resources/todotask.md)|Atualize as propriedades de um [objeto todoTask](../resources/todotask.md) .|
|[Excluir tarefa](../api/todotask-delete.md)|Nenhum|Exclui um [objeto todoTask](../resources/todotask.md) .|
|[Listar checklistItems](../api/todotask-list-checklistitems.md)|[coleção checklistItem](../resources/checklistitem.md)|Obtenha os **recursos checklistItem** da propriedade de navegação checklistItems.|
|[Criar checklistItem](../api/todotask-post-checklistitems.md)|[checklistItem](../resources/checklistitem.md)|Crie um novo **objeto checklistItem** .|
|[Listar linkedResources](../api/todotask-list-linkedresources.md)|[Coleção linkedResource](../resources/linkedresource.md)|Obtenha o linkedResources da propriedade de navegação linkedResources.|
|[Criar linkedResources](../api/todotask-post-linkedresources.md)|[Linkedresource](../resources/linkedresource.md)|Crie um novo objeto linkedResources.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|corpo|[itemBody](../resources/itembody.md)|Corpo da tarefa que normalmente contém informações sobre a tarefa.|
|bodyLastModifiedDateTime|DateTimeOffset|A data e a hora em que o corpo da tarefa foi modificado pela última vez. Por padrão, está definida em UTC. Você pode fornecer um fuso horário personalizado no cabeçalho da solicitação. O valor da propriedade usa o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1º de janeiro de 2020 teria esta aparência: '2020-01-01T00:00:00Z'.|
|categories|Coleção de cadeias de caracteres|As categorias associadas à postagem. Cada categoria corresponde à propriedade **displayName** de uma [outlookCategory](../resources/outlookcategory.md) definida pelo usuário.|
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
|checklistItems|[coleção checklistItem](../resources/checklistitem.md)|Uma coleção de checklistItems vinculados a uma tarefa. |
|extensions|Coleção [extension](extension.md)| A coleção de extensões abertas definidas para a tarefa. Anulável.|
|Linkedresources|[Coleção linkedResource](../resources/linkedresource.md)|Uma coleção de recursos vinculados à tarefa.|

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
  "categories": ["string"],
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



