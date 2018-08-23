# <a name="reminder-resource-type"></a>tipo de recurso de lembrete

Um lembrete para um [evento](event.md) no [calendário](calendar.md) de um usuário.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|changeKey|Sequência de caracteres|Identifica a versão do lembrete. Toda vez que o lembrete é alterado, **changeKey** também muda. Isso permite que o Exchange aplique as alterações na versão correta do objeto.|
|eventEndTime|[DateTimeTimeZone](datetimetimezone.md)|A data, a hora e o fuso horário em que o evento termina.|
|eventId|Sequência de caracteres|A ID exclusiva do evento. Somente leitura.|
|eventLocation|[Localização](location.md)|O local do evento.|
|eventStartTime|[DateTimeTimeZone](datetimetimezone.md)|A data, a hora e o fuso horário em que o evento começa.|
|eventSubject|Sequência de caracteres|O texto da linha de assunto do evento.|
|eventWebLink|Sequência de caracteres|A URL para abrir o evento no Outlook na Web.<br/><br/>O evento será aberto no navegador se você estiver conectado à sua caixa de correio através do Outlook na Web. Você será solicitado a fazer login se já não estiver conectado no navegador.<br/><br/>Essa URL pode ser acessada de um iFrame.|
|reminderFireTime|[DateTimeTimeZone](datetimetimezone.md)|A data, a hora e o fuso horário do lembrete.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.reminder"
}-->

```json
{
  "changeKey": "string",
  "eventEndTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "eventId": "string",
  "eventLocation": {"@odata.type": "microsoft.graph.location"},
  "eventStartTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "eventSubject": "string",
  "eventWebLink": "string",
  "reminderFireTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "reminder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->