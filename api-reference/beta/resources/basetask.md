---
title: Tipo de recurso baseTask
description: Representa uma tarefa, como um item pessoal ou de trabalho, que pode ser rastreada e concluída
author: avijityadav
ms.localizationpriority: medium
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 0a2eed88a85aa9d1b0e2e40c32e258d4e3b7c826
ms.sourcegitcommit: 6950d15d8cce5e04733738b8debb92cd8c1d63fe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2022
ms.locfileid: "63451143"
---
# <a name="basetask-resource-type"></a>Tipo de recurso baseTask

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma tarefa, como um item pessoal ou de trabalho, que pode ser rastreada e concluída.
Esse é um tipo de base abstrato herdado pelo [recurso task](task.md) .

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar baseTasks](../api/basetasklist-list-tasks.md)|[Coleção baseTask](../resources/basetask.md)|Obter uma lista dos [objetos baseTask](../resources/basetask.md) e suas propriedades.|
|[Criar baseTask](../api/basetasklist-post-tasks.md)|[baseTask](../resources/basetask.md)|Crie um novo [objeto baseTask](../resources/basetask.md) .|
|[Obter baseTask](../api/basetask-get.md)|[baseTask](../resources/basetask.md)|Leia as propriedades e as relações de um [objeto baseTask](../resources/basetask.md) .|
|[Atualizar baseTask](../api/basetask-update.md)|[baseTask](../resources/basetask.md)|Atualize as propriedades de um [objeto baseTask](../resources/basetask.md) .|
|[Excluir baseTask](../api/basetask-delete.md)|Nenhum|Exclui um [objeto baseTask](../resources/basetask.md) .|
|[move](../api/basetask-move.md)|[baseTask](../resources/basetask.md)|Mova a mensagem para uma lista diferente.|
|[delta](../api/basetask-delta.md)|[Coleção baseTask](../resources/basetask.md)|Obter um conjunto de **objetos baseTask** que foram adicionados, excluídos ou atualizados em uma lista especificada.|
|[Listar checklistItems](../api/basetask-list-checklistitems.md)|[Coleção checklistItem](../resources/checklistitem.md)|Obter os **recursos checklistItem** da propriedade de navegação checklistItems.|
|[Criar checklistItem](../api/basetask-post-checklistitems.md)|[checklistItem](../resources/checklistitem.md)|Crie um novo **objeto checklistItem** .|
|[Listar linkedResources](../api/basetask-list-linkedresources.md)|[linkedResource_v2](../resources/linkedresource_v2.md) coleção|Obter os **linkedResource_v2** da propriedade de navegação linkedResources.|
|[Criar linkedResource_v2](../api/basetask-post-linkedresources.md)|[linkedResource_v2](../resources/linkedresource_v2.md)|Crie um novo **objeto linkedResource_v2** .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|textBody|Cadeia de caracteres|O corpo da tarefa no formato de texto que normalmente contém informações sobre a tarefa. |
|bodyLastModifiedDateTime|DateTimeOffset|A data e hora da última modificação da tarefa. Por padrão, está definida em UTC. Você pode fornecer um fuso horário personalizado no cabeçalho da solicitação. O valor da propriedade usa o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1º de janeiro de 2020 teria esta aparência: '2020-01-01T00:00:00Z'. |
|completedDateTime|DateTimeOffset|A data em que a tarefa foi concluída. |
|createdDateTime|DateTimeOffset|A data e a hora da criação da tarefa. Por padrão, está definida em UTC. Você pode fornecer um fuso horário personalizado no cabeçalho da solicitação. O valor da propriedade usa o formato ISO 8601. Por exemplo, meia-noite UTC em 1º de janeiro de 2020 teria esta aparência: '2020-01-01T00:00:00Z'. |
|displayName|Cadeia de caracteres|O nome da tarefa. |
|dueDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)|A data no fuso horário especificado que a tarefa será concluída. |
|id|Cadeia de caracteres|Identificador exclusivo para a tarefa. Por padrão, esse valor não mudará se uma tarefa for movida de uma lista para outra. |
|importância|importância|A importância da tarefa. Os valores possíveis são: `low`, `normal`, `high`.  Os valores possíveis são: `low`, `normal`, `high`.|
|lastModifiedDateTime|DateTimeOffset|A data e hora da última modificação da tarefa. Por padrão, está definida em UTC. Você pode fornecer um fuso horário personalizado no cabeçalho da solicitação. O valor da propriedade usa o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1º de janeiro de 2020 teria esta aparência: '2020-01-01T00:00:00Z'. |
|mirante|[taskViewpoint](../resources/taskviewpoint.md)|Propriedades que são pessoais para um usuário, como **reminderDateTime** e **categorias**. |
|recurrence|[patternedRecurrence](../resources/patternedrecurrence.md)|O padrão de recorrência da tarefa. |
|startDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)|A data no fuso horário especificado que a tarefa será iniciada. |
|status|taskStatus_v2|Indica o estado ou o andamento da tarefa. Os valores possíveis são: `notStarted`, `inProgress`, , `completed`,`unknownFutureValue`. |

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|checklistItems|[Coleção checklistItem](../resources/checklistitem.md)|Uma coleção de checklistItems vinculados a uma tarefa. |
|extensions|Coleção [extension](../resources/extension.md)|A coleção de extensões abertas definidas para a tarefa . |
|linkedResources|[linkedResource_v2](../resources/linkedresource_v2.md) coleção|Uma coleção de recursos vinculados à tarefa. |
|parentList|[baseTaskList](../resources/basetasklist.md)|A lista que contém a tarefa. |

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.baseTask",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.baseTask",
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

