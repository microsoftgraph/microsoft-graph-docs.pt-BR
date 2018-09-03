# <a name="automaticrepliesmailtips-resource-type"></a>tipo de recurso de automaticRepliesMailTips


[Dicas de e-mail](../resources/mailtips.md) sobre qualquer resposta automática configurada em uma caixa de correio.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:-----|:-----|:-----|
| message | Sequência de caracteres | A mensagem de resposta automática. |
| messageLanguage | [localeInfo](../resources/localeinfo.md) | O idioma em que a mensagem de resposta automática está. |
| scheduledEndTime | [dateTimeTimeZone](../resources/datetimetimezone.md) | A data e a hora em que as respostas automáticas estão definidas para terminar. |
| scheduledStartTime | [dateTimeTimeZone](../resources/datetimetimezone.md) | A data e a hora em que as respostas automáticas são definidas para começar. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "messageLanguage",
    "scheduledEndTime",
    "scheduledStartTime"
  ],
  "@odata.type": "microsoft.graph.automaticRepliesMailTips"
}-->

```json
{
  "message": "string",
  "messageLanguage": {"@odata.type": "microsoft.graph.localeInfo"},
  "scheduledEndTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "scheduledStartTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "automaticRepliesMailTips resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->