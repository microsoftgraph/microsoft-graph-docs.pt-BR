---
title: tipo de recurso outlookTask
description: 'Um item do Outlook que pode rastrear um item de trabalho. '
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: 71f649c0ef5fd23caafc9bcd3e35282287d35372
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27865559"
---
# <a name="outlooktask-resource-type"></a>tipo de recurso outlookTask

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Um item do Outlook que pode rastrear um item de trabalho. 

Você pode usar uma tarefa para controlar o início, devido e datas de conclusão reais e horas, seu progresso ou status, se ele for recorrente e requer lembrar.

Propriedades relacionadas a data no recurso **outlookTask** incluem o seguinte:

- completedDateTime
- createdDateTime
- dueDateTime
- lastModifiedDateTime
- reminderDateTime
- startDateTime

Por padrão, as operações de POST, GET, PATCH e [completa](../api/outlooktask-complete.md) retornam propriedades relacionadas a data em suas respostas REST em UTC. Você pode usar o cabeçalho `Prefer: outlook.timezone` para que todas as propriedades relacionadas à data na resposta sejam representadas em um fuso horário diferente de UTC. O exemplo a seguir retorna as propriedades relacionadas à data em EST na resposta correspondente:

```
Prefer: outlook.timezone="Eastern Standard Time"
```

## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter outlookTask](../api/outlooktask-get.md) | [outlookTask](outlooktask.md) |Obtenha as propriedades e relacionamentos de uma tarefa do Outlook na caixa de correio do usuário.|
|[Update](../api/outlooktask-update.md) | [outlookTask](outlooktask.md) |Alterar propriedades graváveis de uma tarefa do Outlook. |
|[Delete](../api/outlooktask-delete.md) | Nenhum |Exclua a tarefa especificada na caixa de correio do usuário. |
|[Conclusão](../api/outlooktask-complete.md)|coleção [outlookTask](outlooktask.md)|Concluir uma tarefa do Outlook que define a propriedade **completedDateTime** à data atual e a propriedade **status** para `completed`.|
|**Anexos**| | |
|[List attachments](../api/outlooktask-list-attachments.md) |Coleção [attachment](attachment.md)| Obtenha todos os anexos em uma tarefa do Outlook.|
|[Add attachment](../api/outlooktask-post-attachments.md) |[attachment](attachment.md)| Adicione um arquivo, um item (mensagem, evento ou contato) ou um link para um arquivo como um anexo para uma tarefa.|
|**Propriedades estendidas**| | |
|[Criar uma propriedade estendida de valor único](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[outlookTask](outlooktask.md)  |Crie um ou mais propriedades estendidas de valor único em uma tarefa do Outlook nova ou existente.   |
|[Obtenha a tarefa com a propriedade estendida de valor único](../api/singlevaluelegacyextendedproperty-get.md)  | [outlookTask](outlooktask.md) | Obtenha as tarefas do Outlook que contêm um valor único propriedade estendida usando `$expand` ou `$filter`. |
|[Criar propriedade estendida de vários valores](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [outlookTask](outlooktask.md) | Crie um ou mais propriedades estendidas de valores múltiplos em uma tarefa do Outlook nova ou existente.  |
|[Obtenha a tarefa com valor múltiplos de propriedade estendida](../api/multivaluelegacyextendedproperty-get.md)  | [outlookTask](outlooktask.md) | Obtenha uma tarefa do Outlook que contenha uma propriedade de valor múltiplos estendida usando `$expand`. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|assignedTo|Cadeia de caracteres|O nome da pessoa que tenha sido atribuído a tarefa.|
|body|[itemBody](itembody.md)|O corpo da tarefa que normalmente contém informações sobre a tarefa. Observe que apenas o tipo de HTML é suportado.|
|categories|String collection|As categorias associadas à tarefa. Cada categoria corresponde à propriedade **displayName** de um [outlookCategory](outlookcategory.md) que o usuário tenha definido.|
|changeKey|Cadeia de caracteres|A versão da tarefa.|
|completedDateTime|[dateTimeTimeZone](datetimetimezone.md)|A data no fuso horário especificado que a tarefa foi concluída.|
|createdDateTime|DateTimeOffset|A data e hora em que a tarefa foi criada. Por padrão, ela é em UTC. Você pode fornecer um fuso horário personalizado no cabeçalho da solicitação. O valor da propriedade usa o formato ISO 8601. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.|
|dueDateTime|[dateTimeTimeZone](datetimetimezone.md)|A data em que o fuso horário especificado que a tarefa deve ser concluído.|
|hasAttachments|Booliano|Defina como true se a tarefa tiver anexos.|
|id|Cadeia de caracteres|O identificador exclusivo da tarefa. Somente leitura.|
|importance|string|A importância do evento. Os valores possíveis são: `low`, `normal`, `high`.|
|isReminderOn|Booliano|Defina como true se um alerta for definido como lembrar o usuário da tarefa.|
|lastModifiedDateTime|DateTimeOffset|A data e a hora da última modificação a tarefa. Por padrão, ela é em UTC. Você pode fornecer um fuso horário personalizado no cabeçalho da solicitação. O valor da propriedade usa o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.|
|owner|Cadeia de caracteres|O nome da pessoa que criou a tarefa.|
|parentFolderId|Cadeia de caracteres|O identificador exclusivo para a pasta do pai da tarefa.|
|recurrence|[patternedRecurrence](patternedrecurrence.md)|O padrão de recorrência da tarefa.|
|reminderDateTime|[dateTimeTimeZone](datetimetimezone.md)|A data e hora para um alerta de lembrete da tarefa ocorra.|
|sensitivity|string|Indica o nível de privacidade para a tarefa. Os valores possíveis são: `normal`, `personal`, `private`, `confidential`.|
|startDateTime|[dateTimeTimeZone](datetimetimezone.md)|A data no fuso horário especificado quando a tarefa for começar.|
|status|string|Indica o estado ou o progresso da tarefa. Os valores possíveis são: `notStarted`, `inProgress`, `completed`, `waitingOnOthers`, `deferred`.|
|subject|Cadeia de caracteres|Uma breve descrição ou o título da tarefa.|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|attachments|Coleção [attachment](attachment.md)|A coleção de anexos [fileAttachment](fileattachment.md), [itemAttachment](itemattachment.md)e [referenceAttachment](referenceattachment.md) para a tarefa.  Somente leitura. Anulável.|
|multiValueExtendedProperties|Coleção [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)|A coleção de propriedades estendidas de valores múltiplos definidas para a tarefa. Somente leitura. Anulável.|
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
<!-- {
  "type": "#page.annotation",
  "description": "outlookTask resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
