---
title: 'evento: delta'
description: Obtém um conjunto de eventos que foram adicionados, excluídos ou atualizado em um **calendarView** (um intervalo de eventos)
localization_priority: Normal
author: harini84
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: efa0768fbb8cae441afc3d1fd48baa2e2a3567da
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50436236"
---
# <a name="event-delta"></a>evento: delta

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obter um conjunto de [recursos de](../resources/event.md) evento que foram adicionados, excluídos ou atualizados em um ou mais calendários. 

Você pode obter tipos específicos dessas alterações incrementais nos eventos em todos os calendários de uma caixa de correio ou em um calendário específico ou em uma coleção de eventos de **um calendarView** (intervalo de eventos definidos por datas de início e término) de um calendário. O calendário pode ser o calendário padrão ou algum outro calendário especificado do usuário. No caso de obter alterações incrementais em **calendarView**, o calendário também pode ser um calendário de grupo.

Uma **chamada** de função delta é semelhante a uma ou solicitação para o calendário especificado, exceto que, aplicando adequadamente `GET /events` `GET /calendarview` [tokens](/graph/delta-query-overview#state-tokens) de estado em uma ou mais dessas chamadas, você pode consultar alterações incrementais de eventos nesse calendário. Isso permite manter e sincronizar um armazenamento local de eventos no calendário especificado, sem precisar buscar todos os eventos desse calendário do servidor sempre.

A tabela a seguir lista as diferenças entre a **função delta** em eventos e a **função delta** em **um calendarView** em um calendário.

| Função Delta em eventos  | Função Delta no calendarView  |
|:--------------------------|:---------------------------------------------------------|
| Obtém alterações incrementais de todos os eventos em um calendário não limitado por um intervalo de datas inicial e final. Como alternativa, você pode obter alterações incrementais dos eventos em um calendário limitado por uma hora de início, começando em ou após essa data/hora. | Obtém alterações incrementais de eventos na data/hora inicial e final do **calendarView**. |
| Retorna apenas um conjunto limitado de propriedades **de** evento por motivos de desempenho. Cliente a ser usado posteriormente `GET /events/{id}` para expandir quaisquer eventos. | A expansão do lado do servidor retorna um conjunto mais completo de **propriedades de** evento. |
| A resposta inclui instâncias individuais e o mestre de série recorrente. | A resposta inclui instâncias únicas e ocorrências e exceções de séries recorrentes. |
| Aplica-se a eventos em calendários de usuários, mas não a calendários de grupo. | Aplica-se a eventos em calendários de usuários e grupos. |
| Atualmente disponível apenas na versão beta. | Disponível nas versões v1.0 e beta. |

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Calendars.Read, Calendars.ReadWrite    |
|Delegado (conta pessoal da Microsoft) | Calendars.Read, Calendars.ReadWrite    |
|Aplicativo | Calendars.Read, Calendars.ReadWrite |

## <a name="http-request"></a>Solicitação HTTP

Esta seção mostra a sintaxe de solicitação HTTP para a chamada de função **delta** inicial para iniciar uma sincronização completa que recupera todos os eventos no calendário ou no visualização de calendário especificado. Essa sintaxe não contém [tokens de estado](/graph/delta-query-overview#state-tokens). 

A URL de consulta retornada em uma `nextLink` ou de uma resposta `deltaLink` bem-sucedida inclui um token de estado. Para qualquer chamada **de função delta** subsequente, use a URL de consulta em uma ou `nextLink` `deltaLink` precedindo-a.

### <a name="delta-function-on-events-in-a-user-calendar-preview"></a>Função Delta em eventos em um calendário do usuário (visualização)
Aplique a **função delta** em todos os eventos ou eventos que começam em ou após uma data/hora específica, nos calendários do usuário especificados:

* Para obter alterações incrementais de todos os eventos ou de eventos que começam em ou após a data/hora especificada na caixa de correio _do usuário_:
  <!-- { "blockType": "ignored" } -->
  ```http
  GET /me/events/delta 
  GET /users/{id | userPrincipalName}/events/delta 

  GET /me/events/delta?startDateTime={start_datetime}
  GET /users/{id | userPrincipalName}/events/delta?startDateTime={start_datetime}
  ```

* Para obter alterações incrementais de todos os eventos ou de eventos que começam em ou após a data/hora especificada no calendário padrão _do usuário:_
  <!-- { "blockType": "ignored" } -->
  ```http
  GET /me/calendar/events/delta 
  GET /users/{id | userPrincipalName}/calendar/events/delta 

  GET /me/calendar/events/delta?startDateTime={start_datetime} 
  GET /users/{id | userPrincipalName}/calendar/events/delta?startDateTime={start_datetime}
  ```

* Para obter alterações incrementais de todos os eventos ou de eventos que começam em ou após a data/hora especificada no _calendário do usuário especificado:_
  <!-- { "blockType": "ignored" } -->
  ```http
  GET /me/calendars/{id}/events/delta 
  GET /users/{id | userPrincipalName}/calendars/{id}/events/delta 

  GET /me/calendars/{id}/events/delta?startDateTime={start_datetime} 
  GET /users/{id | userPrincipalName}/calendars/{id}/events/delta?startDateTime={start_datetime}
  ```

* Para obter alterações incrementais de todos os eventos ou de eventos que começam em ou após a data/hora especificada no grupo de calendários _especificado e no calendário_:
  <!-- { "blockType": "ignored" } -->
  ```http
  GET /me/calendargroups/{id}/calendars/{id}/events/delta 
  GET /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/delta 

  GET /me/calendargroups/{id}/calendars/{id}/events/delta?startDateTime={start_datetime} 
  GET /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/delta?startDateTime={start_datetime}
  ```

<!-- Add back and fix html when group calendars are supported

### Delta function on events in a group calendar (preview)
* To get incremental changes of all the events, or of events starting on or after the specified date/time _in a group calendar_:
  !-- { "blockType": "ignored" } --
  ```http
  GET /groups/{id}/events/delta
  GET /groups/{id}/calendar/events/delta

  GET /groups/{id}/events/delta?startDateTime={start_datetime}
  GET /groups/{id}/calendar/events/delta?startDateTime={start_datetime}
  ```

  -->

### <a name="delta-function-on-calendarview-in-a-user-calendar"></a>Função Delta no calendarView em um calendário do usuário
Aplique a **função delta** em um intervalo de eventos delimitados por data/hora inicial e final, no calendário do usuário especificado:

* Para obter alterações incrementais em um modo de exibição de calendário _do calendário padrão do usuário:_
  <!-- { "blockType": "ignored" } -->
  ```http
  GET /me/calendarView/delta?startDateTime={start_datetime}&endDateTime={end_datetime}
  GET /users/{id}/calendarView/delta?startDateTime={start_datetime}&endDateTime={end_datetime}
  ```

* Para obter alterações incrementais em uma exibição de calendário _do calendário de usuário especificado:_
  <!-- { "blockType": "ignored" } -->
  ```http
  GET /me/calendars/{id}/calendarView/delta?startDateTime={start_datetime}&endDateTime={end_datetime}
  GET /users/{id}/calendars/{id}/calendarView/delta?startDateTime={start_datetime}&endDateTime={end_datetime}
  ```

### <a name="delta-function-on-calendarview-in-a-group-calendar"></a>Função Delta no calendarView em um calendário de grupo
* Para obter alterações incrementais em uma exibição de calendário do _calendário de um grupo:_
  <!-- { "blockType": "ignored" } -->
  ```http
  GET /groups/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
  ```

## <a name="query-parameters"></a>Parâmetros de consulta

O controle de alterações incorre em uma rodada de uma ou mais chamadas **de função delta.** Se você usar qualquer parâmetro de consulta (diferente de `$deltatoken` e `$skiptoken`), especifique-o na primeira solicitação **delta**. O Microsoft Graph codifica automaticamente todos os parâmetros especificados na parte do token da URL `nextLink` ou `deltaLink` fornecida na resposta. Você só precisa especificar uma vez os parâmetros de consulta desejados antecipadamente.
Em solicitações subsequentes, basta copiar e aplicar a URL ou da resposta anterior, pois essa URL já inclui os `nextLink` `deltaLink` parâmetros codificados e desejados.

| Parâmetro de consulta      | Tipo   |Descrição|
|:---------------|:--------|:----------|
|startDateTime|String|A data e a hora de início do intervalo de tempo, representadas no formato ISO 8601. Por exemplo, "2019-11-08T19:00:00-08:00".<br>O timezone é especificado na parte de deslocamento de zona de tempo do valor do parâmetro e não é afetado pelo `Prefer: outlook.timezone` header, se presente. Se nenhum deslocamento de fuso horário estiver incluído no valor, ele será interpretado como UTC.<br>Opcional para **delta** em eventos em um calendário. <br>Obrigatório para **delta em** **calendarView**. |
|endDateTime|String|A data e a hora de término do intervalo de tempo, representadas no formato ISO 8601. Por exemplo, "2019-11-08T20:00:00-08:00".<br>O timezone é especificado na parte de deslocamento de zona de tempo do valor do parâmetro e não é afetado pelo `Prefer: outlook.timezone` header, se presente. Se nenhum deslocamento de fuso horário estiver incluído no valor, ele será interpretado como UTC.<br>_Não há suporte para_ **delta** em eventos em um calendário. <br>Obrigatório para **delta em** **calendarView**.|
| $deltatoken | string | Um [token de estado](/graph/delta-query-overview) retornado na URL `deltaLink` da chamada de função **delta** anterior do mesmo modo de exibição de calendário, indicando a conclusão da série de controle de alterações. Salve e aplique toda a URL `deltaLink`, incluindo esse token na primeira solicitação da próxima série de controle do modo de exibição de calendário.|
| $skiptoken | string | Um [token de estado](/graph/delta-query-overview) retornado na URL `nextLink` da chamada de função **delta** anterior indicando que não há mais alterações a serem controladas no mesmo modo de exibição de calendário. |

Não suporta `$expand` , , , e `$filter` `$orderby` `$select` `$search` .


## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome       | Tipo | Descrição |
|:---------------|:----------|:----------|
| Autorização  | string  | {token} de portador. Obrigatório. |
| Content-Type  | string  | application/json. Obrigatório. |
| Preferir | cadeia de caracteres  | odata.maxpagesize={x}. Opcional. |
| Preferir | string | outlook.timezone={Cadeia de caracteres de fuso horário}. Opcional, supõe-se o UTC se estiver ausente.|

## <a name="response"></a>Resposta

### <a name="delta-function-on-events-preview"></a>Função Delta em eventos (visualização)
Se tiver êxito, este método retornará um código `200 OK` de resposta e uma coleção [de](../resources/event.md) eventos no corpo da resposta. Cada **evento** na resposta contém apenas **as propriedades id**, **type**, **start** e **end** por motivos de desempenho. Use `GET /events/{id}` subsequentemente para expandir quaisquer eventos da resposta.  

### <a name="delta-function-on-calendarview"></a>Função Delta no calendarView
Se tiver êxito, este método retornará um código `200 OK` de resposta e uma coleção [de](../resources/event.md) eventos no corpo da resposta.

Espere obter todas as propriedades que você normalmente obteria de uma `GET /calendarview` solicitação. 

## <a name="examples"></a>Exemplos

### <a name="example-1-delta-function-on-events-in-a-calendar-preview"></a>Exemplo 1: função Delta em eventos em um calendário (visualização)
#### <a name="request"></a>Solicitação
O exemplo a seguir mostra a solicitação de sincronização inicial para obter eventos no calendário padrão do usuário in-loco, que ocorrem em ou após o parâmetro `startDateTime` especificado. A solicitação inicial não inclui nenhum token de estado. 

A solicitação usa `Prefer: odata.maxpagesize` o header para limitar o número máximo de eventos em cada resposta a 1. Continue chamando a `delta` função usando a consulta retornada até obter uma na `@odata.nextLink` `@odata.deltaLink` resposta.

<!-- {
  "blockType": "request",
  "name": "event_delta_events"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/calendar/events/delta?startDateTime=2020-06-12T00:00:00Z

Prefer: odata.maxpagesize=1
```

#### <a name="response"></a>Resposta

Se a solicitação for bem-sucedida, a resposta incluirá um token de estado, que é _um skipToken_ (em um header de resposta _\@ odata.nextLink)_ ou _um deltaToken_ (em um header de resposta _\@ odata.deltaLink)._
Respectivamente, eles indicam se você deve continuar com a rodada ou se você concluiu todas as alterações para essa rodada.

A resposta a seguir mostra _um skipToken_ em um header de resposta _\@ odata.nextLink._

<!-- {
  "blockType": "response",
  "name": "event_delta_events",
  "truncated": true,
  "@odata.type": "microsoft.graph.event",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.nextLink":"https://graph.microsoft.com/beta/me/calendar/events/delta?$skiptoken=R0usmcdvmMu7jxWP8",
  "value": [
    { 
      "id": " AAMkADllMWMwNDkzLWJlY2EtNDIyOS1iZjAA=", 
      "type": "singleInstance", 
      "start": {  
             "DateTime": "2020-02-19T10:00:00.0000000",  
             "TimeZone": "UTC" 
         },  
       "end": {  
                "DateTime": "2020-02-19T11:00:00.0000000",  
                "TimeZone": "UTC"        
          }  
        } 
  ]
}
```


### <a name="example-2-delta-function-on-calendarview"></a>Exemplo 2: função Delta em calendarView
#### <a name="request"></a>Solicitação

O exemplo a seguir mostra a solicitação de sincronização inicial para obter eventos no calendário especificado do usuário in-loco, dentro do intervalo de datas indicadas pelo **calendarView**. A solicitação inicial não inclui nenhum token de estado. 

A solicitação usa `Prefer: odata.maxpagesize` o header para limitar o número máximo de eventos em cada resposta a 2. Continue chamando a função usando a consulta retornada até que você receba todos os eventos nesse `delta` `@odata.nextLink` exibição de calendário e `@odata.deltaLink` um na resposta.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADI5M1BbeAAA="],
  "name": "event_delta_calendarview"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/calendars/AAMkADI5M1BbeAAA=/calendarview/delta?startDateTime=2020-06-01T00:00:00Z&endDateTime=2020-06-10T00:00:00Z

Prefer: odata.maxpagesize=2
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/event-delta-calendarview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/event-delta-calendarview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/event-delta-calendarview-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Resposta

Se a solicitação for bem-sucedida, a resposta incluirá um token de estado, que é _um skipToken_ (em um header de resposta _\@ odata.nextLink)_ ou _um deltaToken_ (em um header de resposta _\@ odata.deltaLink)._
Respectivamente, eles indicam se você deve continuar com a rodada ou se você concluiu todas as alterações para essa rodada.

A resposta a seguir mostra _um skipToken_ em um header de resposta _\@ odata.nextLink._

Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. 
<!-- {
  "blockType": "response",
  "name": "event_delta_calendarview",
  "truncated": true,
  "@odata.type": "microsoft.graph.event",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(event)",
    "@odata.nextLink": "https://graph.microsoft.com/beta/me/calendars/AAMkADI5M1BbeAAA=/calendarview/delta?$skiptoken=R0usmcdvmMu7jxWP8",
    "value": [
        {
            "@odata.type": "#microsoft.graph.event",
            "@odata.etag": "W/\"Jdsb3FEkPk2qoUHCdliYowACwixTgw==\"",
            "createdDateTime": "2020-06-16T04:05:43.8668791Z",
            "lastModifiedDateTime": "2020-06-16T04:08:27.354268Z",
            "changeKey": "Jdsb3FEkPk2qoUHCdliYowACwixTgw==",
            "categories": [],
            "transactionId": null,
            "originalStartTimeZone": "Pacific Standard Time",
            "originalEndTimeZone": "Pacific Standard Time",
            "uid": "040000008200E00074C5B7101A82E00800000000F088B8B95843D601000000000000000010000000165CD5547CFC9545B6492B261750B48C",
            "reminderMinutesBeforeStart": 15,
            "isReminderOn": false,
            "hasAttachments": false,
            "subject": "Summer party",
            "bodyPreview": "",
            "importance": "normal",
            "sensitivity": "normal",
            "isAllDay": false,
            "isCancelled": false,
            "isOrganizer": true,
            "IsRoomRequested": false,
            "AutoRoomBookingStatus": "None",
            "responseRequested": true,
            "seriesMasterId": null,
            "showAs": "busy",
            "type": "singleInstance",
            "webLink": "https://outlook.office365.com/owa/?itemid=AAMkADI5MAAKkeE1QAAA%3D&exvsurl=1&path=/calendar/item",
            "onlineMeetingUrl": null,
            "isOnlineMeeting": false,
            "onlineMeetingProvider": "unknown",
            "allowNewTimeProposals": true,
            "OccurrenceId": null,
            "isDraft": false,
            "recurrence": null,
            "AutoRoomBookingOptions": null,
            "onlineMeeting": null,
            "id": "AAMkADI5MAAKkeE1QAAA=",
            "responseStatus": {
                "response": "none",
                "time": "0001-01-01T00:00:00Z"
            },
            "body": {
                "contentType": "html",
                "content": "<html>\r\n<head></head>\r\n<body lang=\"EN-US\" link=\"#0563C1\" vlink=\"#954F72\" style=\"\">\r\n<div class=\"WordSection1\">\r\n<p class=\"MsoNormal\">&nbsp;</p>\r\n</div>\r\n</body>\r\n</html>\r\n"
            },
            "start": {
                "dateTime": "2020-06-02T20:00:00.0000000",
                "timeZone": "UTC"
            },
            "end": {
                "dateTime": "2020-06-02T22:30:00.0000000",
                "timeZone": "UTC"
            },
            "location": {
                "displayName": "",
                "locationType": "default",
                "uniqueIdType": "unknown",
                "address": {
                    "type": "unknown"
                },
                "coordinates": {}
            },
            "locations": [],
            "attendees": [
                {
                    "type": "required",
                    "status": {
                        "response": "none",
                        "time": "0001-01-01T00:00:00Z"
                    },
                    "emailAddress": {
                        "name": "Samantha Booth",
                        "address": "samanthab@contoso.onmicrosoft.com"
                    }
                }
            ],
            "organizer": {
                "emailAddress": {
                    "name": "Samantha Booth",
                    "address": "samanthab@contoso.onmicrosoft.com"
                }
            }
        },
        {
            "@odata.type": "#microsoft.graph.event",
            "@odata.etag": "W/\"Jdsb3FEkPk2qoUHCdliYowACwixTfw==\"",
            "createdDateTime": "2020-06-16T04:06:18.386713Z",
            "lastModifiedDateTime": "2020-06-16T04:08:19.5694048Z",
            "changeKey": "Jdsb3FEkPk2qoUHCdliYowACwixTfw==",
            "categories": [],
            "transactionId": null,
            "originalStartTimeZone": "Pacific Standard Time",
            "originalEndTimeZone": "Pacific Standard Time",
            "uid": "040000008200E00074C5B7101A82E0080000000060074BC55843D6010000000000000000100000002D33A89F36B10D43A12FD990B62858B2",
            "reminderMinutesBeforeStart": 15,
            "isReminderOn": true,
            "hasAttachments": false,
            "subject": "Summer party part 2",
            "bodyPreview": "",
            "importance": "normal",
            "sensitivity": "normal",
            "isAllDay": false,
            "isCancelled": false,
            "isOrganizer": true,
            "IsRoomRequested": false,
            "AutoRoomBookingStatus": "None",
            "responseRequested": true,
            "seriesMasterId": null,
            "showAs": "busy",
            "type": "singleInstance",
            "webLink": "https://outlook.office365.com/owa/?itemid=AAMkADI5MAAKkeE1RAAA%3D&exvsurl=1&path=/calendar/item",
            "onlineMeetingUrl": null,
            "isOnlineMeeting": false,
            "onlineMeetingProvider": "unknown",
            "allowNewTimeProposals": true,
            "OccurrenceId": null,
            "isDraft": false,
            "recurrence": null,
            "AutoRoomBookingOptions": null,
            "onlineMeeting": null,
            "id": "AAMkADI5MAAKkeE1RAAA=",
            "responseStatus": {
                "response": "none",
                "time": "0001-01-01T00:00:00Z"
            },
            "body": {
                "contentType": "html",
                "content": "<html>\r\n<head></head>\r\n<body lang=\"EN-US\" link=\"#0563C1\" vlink=\"#954F72\" style=\"\">\r\n<div class=\"WordSection1\">\r\n<p class=\"MsoNormal\">&nbsp;</p>\r\n</div>\r\n</body>\r\n</html>\r\n"
            },
            "start": {
                "dateTime": "2020-06-04T19:30:00.0000000",
                "timeZone": "UTC"
            },
            "end": {
                "dateTime": "2020-06-04T22:30:00.0000000",
                "timeZone": "UTC"
            },
            "location": {
                "displayName": "",
                "locationType": "default",
                "uniqueIdType": "unknown",
                "address": {
                    "type": "unknown"
                },
                "coordinates": {}
            },
            "locations": [],
            "attendees": [
                {
                    "type": "required",
                    "status": {
                        "response": "none",
                        "time": "0001-01-01T00:00:00Z"
                    },
                    "emailAddress": {
                        "name": "Samantha Booth",
                        "address": "samanthab@contoso.onmicrosoft.com"
                    }
                }
            ],
            "organizer": {
                "emailAddress": {
                    "name": "Samantha Booth",
                    "address": "samanthab@contoso.onmicrosoft.com"
                }
            }
        }
    ]
}
```

## <a name="see-also"></a>Confira também

- [Consulta delta do Microsoft Graph](/graph/delta-query-overview)
- [Obter as alterações incrementais para os eventos em uma pasta](/graph/delta-query-events)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "event: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


