---
title: tipo de recurso outlookTask
description: 'Um item do Outlook que pode acompanhar um item de trabalho. '
author: mashriv
localization_priority: Priority
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 1cf1958dc4d07c9bf2b322e6a4b576ce4a8191f6
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50956852"
---
# <a name="outlooktask-resource-type-deprecated"></a>tipo de recurso outlookTask (substituído)

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]

Um item do Outlook que pode acompanhar um item de trabalho.

Você pode usar uma tarefa para controlar as datas e horas de conclusão atuais ou anteriores, seu andamento ou status, se são recorrentes ou requerem um lembrete.

As propriedades relacionadas à data no recurso **outlookTask** incluem o seguinte:

- completedDateTime
- createdDateTime
- dueDateTime
- lastModifiedDateTime
- reminderDateTime
- startDateTime

Por padrão, as operações POST, GET, PATCH e [complete](../api/outlooktask-complete.md) retornam as propriedades relacionadas à data em suas respostas REST em UTC.
Você pode usar o `Prefer: outlook.timezone` cabeçalho para que todas as propriedades relacionadas às datas como resposta representada em um fuso horário diferente do UTC. O exemplo a seguir retorna propriedades de data no EST na resposta correspondente:

```
Prefer: outlook.timezone="Eastern Standard Time"
```

## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter outlookTask](../api/outlooktask-get.md) | [outlookTask](outlooktask.md) |Obtenha as propriedades e as relações de uma tarefa do Outlook na caixa de correio do usuário.|
|[Atualizar](../api/outlooktask-update.md) | [outlookTask](outlooktask.md) |Altere as propriedades graváveis ​​de uma tarefa do Outlook. |
|[Excluir](../api/outlooktask-delete.md) | Nenhum |Exclua a tarefa especificada na caixa de correio do usuário. |
|[Concluído](../api/outlooktask-complete.md)|coleção [outlookTask](outlooktask.md)|Concluir uma tarefa do Outlook que define a propriedade **completedDateTime** para a data atual e a propriedade de **status** para `completed`.|
|**Anexos**| | |
|[List attachments](../api/outlooktask-list-attachments.md) |Coleção [anexo](attachment.md)| Obtenha todos os anexos de uma tarefa do Outlook.|
|[Add attachment](../api/outlooktask-post-attachments.md) |[anexo](attachment.md)| Adiciona um arquivo, um item (mensagem, evento ou contato) ou um link a um arquivo como um anexo a uma tarefa.|
|**Propriedades estendidas**| | |
|[Criar uma propriedade estendida de valor único](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[outlookTask](outlooktask.md)  |Criar uma ou mais propriedades estendidas de valor único em uma tarefa do Outlook nova ou existente.   |
|[Obter tarefa com propriedade estendida de valor único](../api/singlevaluelegacyextendedproperty-get.md)  | [outlookTask](outlooktask.md) | Obter tarefas do Outlook que contenham uma propriedade estendida de valor único usando `$expand` ou `$filter`. |
|[Criar propriedade estendida de vários valores](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [outlookTask](outlooktask.md) | Criar uma ou mais propriedades estendidas de vários valores em uma tarefa do Outlook nova ou existente.  |
|[Obter postagem com propriedade estendida de vários valores](../api/multivaluelegacyextendedproperty-get.md)  | [outlookTask](outlooktask.md) | Obter uma tarefa do Outlook que contenha uma propriedade estendida de vários valores usando `$expand`. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|assignedTo|String|O nome da pessoa a qual foi atribuída a tarefa no Outlook. Somente leitura.|
|corpo|[itemBody](itembody.md)|Corpo da tarefa que normalmente contém informações sobre a tarefa. Observe para qual tipo de HTML há suporte.|
|Categorias|Coleção de cadeias de caracteres|As categorias associadas à postagem. Cada categoria corresponde à propriedade **displayName** de uma [outlookCategory](outlookcategory.md) definida pelo usuário.|
|changeKey|Cadeia de caracteres|A versão da tarefa.|
|completedDateTime|[dateTimeTimeZone](datetimetimezone.md)|A data no fuso horário especificado que a tarefa foi concluída.|
|createdDateTime|DateTimeOffset|A data e a hora da criação da tarefa. Por padrão, está definida em UTC. Você pode fornecer um fuso horário personalizado no cabeçalho da solicitação. O valor da propriedade usa o formato ISO 8601. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.|
|dueDateTime|[dateTimeTimeZone](datetimetimezone.md)|A data no fuso horário especificado que a tarefa será concluída.|
|hasAttachments|Booliano|Defina como verdadeiro se a tarefa tiver anexos.|
|id|Cadeia de caracteres| Identificador exclusivo para a tarefa. [!INCLUDE [outlook-beta-id](../../includes/outlook-beta-id.md)] Somente leitura. |
|importância|importância|A importância do evento. Os valores possíveis são: `low`, `normal`, `high`.|
|isReminderOn|Booliano|Definido como verdadeiro se um alerta é definido para lembrar o usuário da tarefa.|
|lastModifiedDateTime|DateTimeOffset|A data e hora da última modificação da tarefa. Por padrão, está definida em UTC. Você pode fornecer um fuso horário personalizado no cabeçalho da solicitação. O valor da propriedade usa o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.|
|owner|Cadeia de caracteres|O nome da pessoa que criou a tarefa.|
|parentFolderId|Cadeia de caracteres|O identificador exclusivo para a pasta pai da tarefa.|
|recorrência|[patternedRecurrence](patternedrecurrence.md)|O padrão de recorrência da tarefa.|
|reminderDateTime|[dateTimeTimeZone](datetimetimezone.md)|A data e hora do alerta de lembrete da tarefa.|
|sensibilidade|sensibilidade|Indica o nível de privacidade da tarefa. Os valores possíveis são: `normal`, `personal`, `private`, `confidential`.|
|startDateTime|[dateTimeTimeZone](datetimetimezone.md)|A data no fuso horário especificado que a tarefa será iniciada.|
|status|taskStatus|Indica o estado ou o andamento da tarefa. Os valores possíveis são: `notStarted`, `inProgress`, `completed`, `waitingOnOthers`, `deferred`.|
|assunto|Cadeia de caracteres|Uma breve descrição ou o título da tarefa.|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|attachments|Coleção [anexo](attachment.md)|A coleção de anexos [FileAttachment](fileattachment.md), [ItemAttachment](itemattachment.md) e [referenceAttachment](referenceattachment.md) da tarefa.  Somente leitura. Anulável.|
|multiValueExtendedProperties|Coleção [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)|A coleção de propriedades estendidas de vários valores definidas para a tarefa. Somente leitura. Anulável.|
|singleValueExtendedProperties|Coleção [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)|A coleção de propriedades estendidas de valor único definidas para a tarefa. Somente leitura. Anulável.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "attachments",
    "singleValueExtendedProperties",
    "multiValueExtendedProperties"
  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",
  "@odata.type": "microsoft.graph.outlookTask"
}-->

```json
{
  "assignedTo": "String",
  "body": {"@odata.type": "microsoft.graph.itemBody"},
  "categories": ["String"],
  "changeKey": "String",
  "completedDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "createdDateTime": "String (timestamp)",
  "dueDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "hasAttachments": true,
  "id": "String (identifier)",
  "importance": "string",
  "isReminderOn": true,
  "lastModifiedDateTime": "String (timestamp)",
  "owner": "String",
  "parentFolderId": "String",
  "recurrence": {"@odata.type": "microsoft.graph.patternedRecurrence"},
  "reminderDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "sensitivity": "string",
  "startDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "status": "string",
  "subject": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "outlookTask resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


