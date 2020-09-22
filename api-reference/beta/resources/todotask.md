---
title: tipo de recurso todoTask
description: Um recurso todoTask controla um item de trabalho.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 58859f2781ecec713e547340606411302232ec06
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48003490"
---
# <a name="todotask-resource-type"></a>tipo de recurso todoTask

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um **todoTask** representa uma tarefa, como uma parte do trabalho ou item pessoal, que pode ser controlada e concluída. 

Um **todoTask** está sempre contido em um [todoTaskList](todotasklist.md). Ele inclui uma relação com uma coleção de objetos [linkedResource](./linkedResource.md) , controlando uma ou mais fontes da tarefa.

Esse recurso suporta o seguinte:
* Adicionar seus dados como propriedades personalizadas em [extensões abertas](/graph/extensibility-overview).
* Usando a [consulta Delta](/graph/delta-query-overview) para controlar adições, exclusões e atualizações incrementais.

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar tarefas](../api/todotasklist-list-tasks.md)|coleção [todoTask](todotask.md)|Obtenha todos os recursos do [todoTask](todotask.md) na lista especificada.|
|[Criar tarefa](../api/todotasklist-post-tasks.md)|[todoTask](todotask.md)| Criar um [todoTask](todotask.md) na lista de tarefas especificada|
|[Obter tarefa](../api/todotask-get.md)|[todoTask](../resources/todotask.md)|Leia as propriedades e os relacionamentos de um objeto [todoTask](../resources/todotask.md) .|
|[Atualizar tarefa](../api/todotask-update.md)|[todoTask](../resources/todotask.md)|Atualiza as propriedades de um objeto [todoTask](../resources/todotask.md) .|
|[Excluir tarefa](../api/todotask-delete.md)|Nenhum|Exclui um objeto [todoTask](../resources/todotask.md) .|
|[Listar linkedResources](../api/todotask-list-linkedresources.md)|coleção [linkedResource](../resources/linkedresource.md)|Obtenha o linkedResources da propriedade de navegação linkedResources.|
|[Criar linkedResources](../api/todotask-post-linkedresources.md)|[linkedResource](../resources/linkedresource.md)|Criar um novo objeto linkedResources.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|corpo|[itemBody](../resources/itembody.md)|Corpo da tarefa que normalmente contém informações sobre a tarefa.|
|bodyLastModifiedDateTime|DateTimeOffset|A data e hora da última modificação da tarefa. Por padrão, está definida em UTC. Você pode fornecer um fuso horário personalizado no cabeçalho da solicitação. O valor da propriedade usa o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1º de janeiro de 2020 teria a seguinte aparência: ' 2020-01-01T00:00:00Z '.|
|completedDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)|A data no fuso horário especificado que a tarefa foi concluída.|
|createdDateTime|DateTimeOffset|A data e a hora da criação da tarefa. Por padrão, está definida em UTC. Você pode fornecer um fuso horário personalizado no cabeçalho da solicitação. O valor da propriedade usa o formato ISO 8601. Por exemplo, meia-noite UTC em 1º de janeiro de 2020 teria a seguinte aparência: ' 2020-01-01T00:00:00Z '.|
|dueDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)|A data no fuso horário especificado que a tarefa será concluída.|
|id|Cadeia de caracteres|Identificador exclusivo para a tarefa. Por padrão, esse valor é alterado quando o item é movido de uma lista para outra.|
|importância|importância|A importância da tarefa. Os valores possíveis são: `low`, `normal`, `high`.|
|isReminderOn|Booliano|Definido como verdadeiro se um alerta é definido para lembrar o usuário da tarefa.|
|lastModifiedDateTime|DateTimeOffset|A data e hora da última modificação da tarefa. Por padrão, está definida em UTC. Você pode fornecer um fuso horário personalizado no cabeçalho da solicitação. O valor da propriedade usa o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1º de janeiro de 2020 teria a seguinte aparência: ' 2020-01-01T00:00:00Z '.|
|recorrência|[patternedRecurrence](../resources/patternedrecurrence.md)|O padrão de recorrência da tarefa.|
|reminderDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)|A data e hora do alerta de lembrete da tarefa.|
|status|taskStatus|Indica o estado ou o andamento da tarefa. Os valores possíveis são: `notStarted`, `inProgress`, `completed`, `waitingOnOthers`, `deferred`.|
|title|String|Uma breve descrição da tarefa.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|extensions|[extension](extension.md) collection| A coleção de extensões abertas definidas para a tarefa. Anulável.|
|linkedResources|coleção [linkedResource](../resources/linkedresource.md)|Uma coleção de recursos vinculados à tarefa.|


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



