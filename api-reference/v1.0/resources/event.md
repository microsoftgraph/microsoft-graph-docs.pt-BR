# <a name="event-resource-type"></a>tipo de recurso de evento

Um evento em um calendário.

Esse recurso permite:

- Adicionar seus próprios dados às propriedades personalizadas usando [extensions](../../../concepts/extensibility_overview.md).
- Usar a [consulta delta](../../../concepts/delta_query_overview.md) para controlar adições, exclusões e atualizações incrementais oferecendo uma função [delta](../api/event_delta.md).


## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Listar eventos](../api/user_list_events.md)|Coleção [event](event.md) |Recuperar uma lista de objetos [event](../resources/event.md) na caixa de correio do usuário. A lista contém reuniões de instância única e reuniões mestres em série.|
|[Criar evento](../api/user_post_events.md) |[event](event.md)| Criar um novo evento postando na coleção de instâncias.|
|[Obter evento](../api/event_get.md) | [event](event.md) |Ler as propriedades e as relações do objeto event.|
|[Atualizar](../api/event_update.md) | [event](event.md) |Atualizar o objeto event. |
|[Excluir](../api/event_delete.md) | Nenhum |Excluir o objeto event. |
|[accept](../api/event_accept.md)|Nenhum|Aceitar o evento especificado.|
|[tentativelyAccept](../api/event_tentativelyaccept.md)|Nenhum|Aceitar provisoriamente o evento especificado.|
|[decline](../api/event_decline.md)|Nenhum|Recusar o convite para o evento especificado.|
|[delta](../api/event_delta.md)|Coleção [event](event.md)|Obtenha um conjunto de eventos que foram adicionados, excluídos ou atualizados em um **calendarView** (um intervalo de eventos) do calendário principal do usuário.|
|[dismissReminder](../api/event_dismissreminder.md)|Nenhum|Descartar o lembrete para o evento especificado.|
|[snoozeReminder](../api/event_snoozereminder.md)|Nenhum|Adiar o lembrete para o evento especificado.|
|[Listar instâncias](../api/event_list_instances.md) |Coleção [event](event.md)| Obter as instâncias (ocorrências) de um evento para um intervalo de tempo especificado. Se o evento for do tipo `SeriesMaster`, isso retornará as exceções e ocorrências desse evento no intervalo de tempo especificado.|
|**Anexos**| | |
|[Listar anexos](../api/event_list_attachments.md) |Coleção [attachment](attachment.md)| Obtenha todos os anexos em um evento.|
|[Add attachment](../api/event_post_attachments.md) |[attachment](attachment.md)| Adicione um novo anexo a um evento postando na coleção attachments.|
|**Extensões abertas**| | |
|[Criar extensão aberta](../api/opentypeextension_post_opentypeextension.md) |[openTypeExtension](opentypeextension.md)| Criar uma extensão aberta e adicionar propriedades personalizadas em uma instância nova ou existente de um recurso.|
|[Obter extensão aberta](../api/opentypeextension_get.md) |Coleção [openTypeExtension](opentypeextension.md)| Obter um ou mais objetos de extensão ou identificados por nome ou nome totalmente qualificado.|
|**Propriedades estendidas**| | |
|[Criar uma propriedade estendida de valor único](../api/singlevaluelegacyextendedproperty_post_singlevalueextendedproperties.md) |[event](event.md)  |Criar uma ou mais propriedades estendidas de valor único em um evento novo ou existente.   |
|[Obter evento com propriedade estendida de valor único](../api/singlevaluelegacyextendedproperty_get.md)  | [event](event.md) | Obter eventos que contenham uma propriedade estendida de valor único usando `$expand` ou `$filter`. |
|[Criar propriedade estendida de vários valores](../api/multivaluelegacyextendedproperty_post_multivalueextendedproperties.md) | [event](event.md) | Criar uma ou mais propriedades estendidas de vários valores em um evento novo ou existente.  |
|[Obter evento com propriedade estendida de vários valores](../api/multivaluelegacyextendedproperty_get.md)  | [event](event.md) | Obter um evento que contenha uma propriedade estendida de vários valores usando `$expand`. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|attendees|Coleção [attendee](attendee.md)|A coleção de participantes do evento.|
|body|[itemBody](itembody.md)|O corpo da mensagem associada ao evento. Pode estar no formato HTML ou no formato de texto.|
|bodyPreview|String|A visualização da mensagem associada ao evento. Está no formato de texto.|
|categories|Coleção de cadeias de caracteres|As categorias associadas ao evento.|
|changeKey|String|Identifica a versão do objeto event. Toda vez que o evento muda, ChangeKey também muda. Isso permite que o Exchange aplique alterações à versão correta do objeto.|
|createdDateTime|DateTimeOffset|O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|end|[dateTimeTimeZone](datetimetimezone.md)|A data, a hora e o fuso horário em que o evento termina.|
|hasAttachments|Boolean|Defina como true se o evento tiver anexos.|
|iCalUId|String|Um identificador exclusivo que é compartilhado por todas as instâncias de um evento em calendários diferentes.|
|id|String| Somente leitura.|
|importance|String|A importância do evento: Low = 0, Normal = 1, High = 2. Os valores possíveis são: `Low`, `Normal`, `High`.|
|isAllDay|Boolean|Defina como true se o evento durar o dia inteiro.|
|isCancelled|Boolean|Defina como true se o evento tiver sido cancelado.|
|isOrganizer|Boolean|Defina como true se o remetente da mensagem também for o organizador.|
|isReminderOn|Boolean|Defina como true se um alerta estiver definido para lembrar o usuário sobre o evento.|
|lastModifiedDateTime|DateTimeOffset|O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|location|[location](location.md)|O local do evento.|
|onlineMeetingUrl|String|Uma URL para uma reunião online.|
|organizer|[recipient](recipient.md)|O organizador do evento.|
|originalEndTimeZone|String|O fuso horário de término que foi definido quando o evento foi criado. Um valor de `tzone://Microsoft/Custom` indica que um fuso horário personalizado herdado foi definido no Outlook para área de trabalho.|
|originalStart|DateTimeOffset|O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|originalStartTimeZone|String|O fuso horário de início que foi definido quando o evento foi criado. Um valor de `tzone://Microsoft/Custom` indica que um fuso horário personalizado herdado foi definido no Outlook para área de trabalho. |
|recurrence|[patternedRecurrence](patternedrecurrence.md)|O padrão de recorrência do evento.|
|reminderMinutesBeforeStart|Int32|O número de minutos antes da hora de início do evento em que o alerta de lembrete ocorre.|
|responseRequested|Boolean|Defina como true se o remetente quiser receber uma resposta quando o evento for aceito ou recusado.|
|responseStatus|[responseStatus](responsestatus.md)|Indica o tipo de resposta enviada em resposta a uma mensagem de evento.|
|sensitivity|String| Os valores possíveis são: `Normal`, `Personal`, `Private`, `Confidential`.|
|seriesMasterId|String|As categorias atribuídas ao item.|
|showAs|String|O status a ser exibido: Free = 0, Tentative = 1, Busy = 2, Oof = 3, WorkingElsewhere = 4, Unknown = -1. Os valores possíveis são: `Free`, `Tentative`, `Busy`, `Oof`, `WorkingElsewhere`, `Unknown`.|
|iniciar|[dateTimeTimeZone](datetimetimezone.md)|A data, a hora e o fuso horário em que o evento começa.|
|subject|String|O texto da linha de assunto do evento.|
|type|String|O tipo de evento: SingleInstance = 0, Occurrence = 1, Exception = 2, SeriesMaster = 3. Os valores possíveis são: `SingleInstance`, `Occurrence`, `Exception`, `SeriesMaster`.|
|webLink|String|A URL para abrir o evento no Outlook Web App.<br/><br/>O evento será aberto no navegador se você estiver conectado à sua caixa de correio por meio do Outlook Web App. Você será solicitado a fazer logon se ainda não estiver conectado no navegador.<br/><br/>Essa URL pode ser acessada de um iFrame.|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|attachments|Coleção [attachment](attachment.md)|A coleção de anexos [fileAttachment](fileAttachment.md) e [itemAttachment](itemAttachment.md) do evento. Propriedade de navegação. Somente leitura. Anulável.|
|calendário|[calendar](calendar.md)|O calendário que contém o evento. Propriedade de navegação. Somente leitura.|
|extensions|Coleção [Extension](extension.md)|A coleção de extensões abertas definidas para o evento. Somente leitura. Anulável.|
|instances|Coleção [event](event.md)|As instâncias do evento. Propriedade de navegação. Somente leitura. Anulável.|
|multiValueExtendedProperties|Coleção [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)| A coleção de propriedades estendidas de vários valores definidas para o evento. Somente leitura. Anulável.|
|singleValueExtendedProperties|Coleção [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)| A coleção de propriedades estendidas de valor único definidas para o evento. Somente leitura. Anulável.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "attachments",
    "calendar",
    "extensions",
    "instances",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.event"
}-->

```json
{
  "attendees": [{"@odata.type": "microsoft.graph.attendee"}],
  "body": {"@odata.type": "microsoft.graph.itemBody"},
  "bodyPreview": "string",
  "categories": ["string"],
  "changeKey": "string",
  "createdDateTime": "String (timestamp)",
  "end": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "hasAttachments": true,
  "iCalUId": "string",
  "id": "string (identifier)",
  "importance": "String",
  "isAllDay": true,
  "isCancelled": true,
  "isOrganizer": true,
  "isReminderOn": true,
  "lastModifiedDateTime": "String (timestamp)",
  "location": {"@odata.type": "microsoft.graph.location"},
  "onlineMeetingUrl": "string",
  "organizer": {"@odata.type": "microsoft.graph.recipient"},
  "originalEndTimeZone": "string",
  "originalStart": "String (timestamp)",
  "originalStartTimeZone": "string",
  "recurrence": {"@odata.type": "microsoft.graph.patternedRecurrence"},
  "reminderMinutesBeforeStart": 1024,
  "responseRequested": true,
  "responseStatus": {"@odata.type": "microsoft.graph.responseStatus"},
  "sensitivity": "String",
  "seriesMasterId": "string",
  "showAs": "String",
  "start": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "subject": "string",
  "type": "String",
  "webLink": "string",

  "attachments": [ { "@odata.type": "microsoft.graph.attachment" } ],
  "calendar": { "@odata.type": "microsoft.graph.calendar" },
  "extensions": [ { "@odata.type": "microsoft.graph.extension" } ],
  "instances": [ { "@odata.type": "microsoft.graph.event" }],
  "multiValueExtendedProperties": [ { "@odata.type": "microsoft.graph.multiValueLegacyExtendedProperty" }],
  "singleValueExtendedProperties": [ { "@odata.type": "microsoft.graph.singleValueLegacyExtendedProperty" }]

}

```


## <a name="see-also"></a>Veja também

- [Usar a consulta delta para controlar alterações nos dados do Microsoft Graph](../../../concepts/delta_query_overview.md)
- [Obter as alterações incrementais para os eventos em uma pasta](../../../concepts/delta_query_events.md)
- [Adicionar dados personalizados a recursos usando extensões](../../../concepts/extensibility_overview.md)
- [Adicionar dados personalizados aos usuários usando extensões abertas](../../../concepts/extensibility_open_users.md)
- [Adicionar dados personalizados a grupos usando as extensões do esquema](../../../concepts/extensibility_schema_groups.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "event resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
