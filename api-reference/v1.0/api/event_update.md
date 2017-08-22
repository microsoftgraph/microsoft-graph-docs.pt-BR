# <a name="update-event"></a>Atualizar evento

Atualize as propriedades do objeto event.
## <a name="prerequisites"></a>Pré-requisitos
Um dos seguintes **escopos** é necessário para executar esta API: *Calendars.ReadWrite*
## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/events/{id}
PATCH /users/{id | userPrincipalName}/events/{id}
PATCH /groups/{id}/events/{id}

PATCH /me/calendar/events/{id}
PATCH /users/{id | userPrincipalName}/calendar/events/{id}
PATCH /groups/{id}/calendar/events/{id}

PATCH /me/calendars/{id}/events/{id}
PATCH /users/{id | userPrincipalName}/calendars/{id}/events/{id}

PATCH /me/calendargroup/calendars/{id}/events/{id}
PATCH /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}

PATCH /me/calendargroups/{id}/calendars/{id}/events/{id}
PATCH /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}
```
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome       | Tipo | Descrição|
|:-----------|:------|:----------|
| Autorização  | string  | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.

| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|attendees|[Attendee](../resources/attendee.md)|A coleção de participantes do evento.|
|corpo|[ItemBody](../resources/itembody.md)|O corpo da mensagem associada ao evento.|
|categories|String|As categorias associadas ao evento.|
|end|[DateTimeTimeZone](../resources/datetimetimezone.md)|A data e a hora em que o evento termina.<br/><br/>Por padrão, a hora de término é em UTC. Você pode especificar um fuso horário opcional em EndTimeZone, expressar a hora de término nesse fuso horário e incluir uma diferença de tempo em relação a UTC. Observe que, se usar EndTimeZone, você deverá especificar um valor para StartTimeZone também.<br/><br/>Este exemplo especifica 25 de fevereiro de 2015, 21: 34 na Hora Padrão do Pacífico: "2015-02-25T21:34:00-08:00". |
|importance|String|A importância do evento: Low = 0, Normal = 1, High = 2. Os valores possíveis são: `Low`, `Normal`, `High`.|
|isAllDay|Boolean|Defina como true se o evento durar o dia inteiro.|
|isReminderOn|Boolean|Defina como true se um alerta estiver definido para lembrar o usuário sobre o evento.|
|location|[Location](../resources/location.md)|O local do evento.|
|onlineMeetingUrl|String|Uma URL para uma reunião online.|
|recurrence|[PatternedRecurrence](../resources/patternedrecurrence.md)|O padrão de recorrência do evento.|
|reminderMinutesBeforeStart|Int32|O número de minutos antes da hora de início do evento em que o alerta de lembrete ocorre.|
|responseRequested|Boolean|Defina como true se o remetente quiser receber uma resposta quando o evento for aceito ou recusado.|
|sensitivity|String| Os valores possíveis são: `Normal`, `Personal`, `Private`, `Confidential`.|
|showAs|String|O status a ser exibido: Free = 0, Tentative = 1, Busy = 2, Oof = 3, WorkingElsewhere = 4, Unknown = -1. Os valores possíveis são: `Free`, `Tentative`, `Busy`, `Oof`, `WorkingElsewhere`, `Unknown`.|
|iniciar|[DateTimeTimeZone](../resources/datetimetimezone.md)|A hora de início do evento. <br/><br/>Por padrão, a hora de início é em UTC. Você pode especificar um fuso horário opcional em StartTimeZone, expressar a hora de início no fuso horário correspondente e incluir uma diferença de tempo em relação a UTC. Observe que, se usar StartTimeZone, você deverá especificar um valor para EndTimeZone também.<br/><br/>Este exemplo especifica 25 de fevereiro de 2015, 19:34 na Hora Padrão do Pacífico: "2015-02-25T19:34:00-08:00".  |
|subject|String|O texto da linha de assunto do evento.|

Como o recurso **event** dá suporte a [extensions](../../../concepts/extensibility_overview.md), você pode usar a operação `PATCH` para adicionar, atualizar ou excluir seus próprios dados específicos do aplicativo nas propriedades personalizadas de uma extensão em uma instância de **event** existente.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [event](../resources/event.md) atualizado no corpo da resposta.
## <a name="example"></a>Exemplo
##### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
<!-- {
  "blockType": "request",
  "name": "update_event"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/events/{id}
Content-type: application/json
Content-length: 285

{
  "originalStartTimeZone": "originalStartTimeZone-value",
  "originalEndTimeZone": "originalEndTimeZone-value",
  "responseStatus": {
    "response": "",
    "time": "datetime-value"
  },
  "iCalUId": "iCalUId-value",
  "reminderMinutesBeforeStart": 99,
  "isReminderOn": true
}
```
##### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 285

{
  "originalStartTimeZone": "originalStartTimeZone-value",
  "originalEndTimeZone": "originalEndTimeZone-value",
  "responseStatus": {
    "response": "",
    "time": "datetime-value"
  },
  "iCalUId": "iCalUId-value",
  "reminderMinutesBeforeStart": 99,
  "isReminderOn": true
}
```

## <a name="see-also"></a>Ver também

- [Adicionar dados personalizados a recursos usando extensões](../../../concepts/extensibility_overview.md)
- [Adicionar dados personalizados aos usuários usando extensões abertas (visualização)](../../../concepts/extensibility_open_users.md)
<!--
- [Add custom data to groups using schema extensions (preview)](../../../concepts/extensibility_schema_groups.md)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update event",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
