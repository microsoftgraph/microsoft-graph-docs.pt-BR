# <a name="user-reminderview"></a>user: reminderView
Retorne uma lista de lembretes de calendário nas horas de início e término especificadas. 

## <a name="prerequisites"></a>Pré-requisitos
Um dos seguintes **escopos** é obrigatório para executar esta API: *Calendars.Read; Calendars.ReadWrite*
## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/reminderView(startDateTime=startDateTime-value,endDateTime=endDateTime-value)
```

## <a name="function-parameters"></a>Parâmetros de função
Forneça os seguintes parâmetros de função com valores na URL solicitada.

| Parâmetro       | Tipo    |Descrição|
|:---------------|:--------|:----------|
|startDateTime|String|A data e hora de início do evento para o qual o lembrete está definido. O valor é representado no formato ISO 8601, por exemplo, "2015-11-08T19:00:00.0000000".|
|endDateTime|String|A data e hora de término do evento para o qual o lembrete está definido. O valor é representado no formato ISO 8601, por exemplo, "2015-11-08T20:00:00.0000000".|


## <a name="request-headers"></a>Cabeçalhos de solicitação
| Cabeçalho       | Valor|
|:-----------|:------|
| Autorização  | <token> de portador. Obrigatório.  |
| Content-Type   | application/json |
| Preferir | <fuso horário>. Opcional, supõe-se o UTC se estiver ausente.| 

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta
Se bem sucedido, este método retorna o código de resposta `200, OK` e o objeto da coleção [reminder](../resources/reminder.md) no corpo da resposta.

## <a name="example"></a>Exemplo
Eis um exemplo de como chamar esta API.
##### <a name="request"></a>Solicitação
Veja a seguir um exemplo da solicitação.
<!-- {
  "blockType": "request",
  "name": "user_reminderview"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/reminderView?startDateTime=startDateTime-value&endDateTime=endDateTime-value
```

##### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.reminder",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 673

{
  "value": [
    {
      "eventId": "eventId-value",
      "eventStartTime": {
        "dateTime": "dateTime-value",
        "timeZone": "timeZone-value"
      },
      "eventEndTime": {
        "dateTime": "dateTime-value",
        "timeZone": "timeZone-value"
      },
      "changeKey": "changeKey-value",
      "eventSubject": "eventSubject-value",
      "eventLocation": {
        "displayName": "displayName-value",
        "address": {
          "street": "street-value",
          "city": "city-value",
          "state": "state-value",
          "countryOrRegion": "countryOrRegion-value",
          "postalCode": "postalCode-value"
        }
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: reminderView",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
