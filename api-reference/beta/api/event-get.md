---
title: Obter evento
description: Obtenha as propriedades e relacionamentos do objeto de evento especificado.
author: harini84
ms.localizationpriority: medium
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: c7ae6555e341d35507d0ebfa4725c57aebca8f56
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/12/2021
ms.locfileid: "60946227"
---
# <a name="get-event"></a>Obter evento

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obtenha as propriedades e as relações do objeto [event](../resources/event.md) especificado.

Um aplicativo pode obter um evento no calendário de outro usuário se:

* O aplicativo tem permissões de aplicativo
* O aplicativo tem as permissões delegadas [apropriadas](#permissions) de um usuário e outro usuário compartilhou um calendário com esse usuário ou deu acesso delegado a esse usuário. Confira os [detalhes e um exemplo](/graph/outlook-get-shared-events-calendars).

Como o **recurso event** dá suporte a [extensões,](/graph/extensibility-overview)você também pode usar a operação para obter propriedades personalizadas e dados de extensão em uma `GET` instância **de** evento.


### <a name="support-various-time-zones"></a>Suporte para vários fusos horários

Para todas as operações GET que retornam eventos, você pode usar o cabeçalho `Prefer: outlook.timezone` para especificar o fuso horário para as horas de início e de término do evento na resposta. 

Por exemplo, o seguinte cabeçalho `Prefer: outlook.timezone` define as horas de início e de término na resposta como Hora Padrão do Leste.
```http
Prefer: outlook.timezone="Eastern Standard Time"
```

Se o evento foi criado em um fuso horário diferente, as horas de início e de término serão ajustadas para o fuso horário especificado no cabeçalho `Prefer`. Veja esta [lista](../resources/datetimetimezone.md) para obter os nomes de fuso horário com suporte. Se o cabeçalho `Prefer: outlook.timezone` não for especificado, as horas de início e de término serão retornadas em UTC.

Você pode usar as propriedades **OriginalStartTimeZone** e **OriginalEndTimeZone** no recurso **event** para descobrir o fuso horário usado quando o evento foi criado.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Calendars.Read    |
|Delegado (conta pessoal da Microsoft) | Calendars.Read    |
|Aplicativo | Calendars.Read |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
GET /me/events/{id}
GET /users/{id | userPrincipalName}/events/{id}
GET /groups/{id}/events/{id}

GET /me/calendar/events/{id}
GET /users/{id | userPrincipalName}/calendar/events/{id}
GET /groups/{id}/calendar/events/{id}

GET /me/calendars/{id}/events/{id}
GET /users/{id | userPrincipalName}/calendars/{id}/events/{id}

GET /me/calendargroups/{id}/calendars/{id}/events/{id}
GET /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}
```
## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome       | Tipo | Descrição|
|:-----------|:------|:----------|
| Autorização  | string  | {token} de portador. Obrigatório. |
| Prefira: outlook.timezone | string | Use isso para especificar o fuso horário para os horários de início e término na resposta. Se não for especificado, esses valores de tempo serão retornados em UTC. Opcional. |
| Prefer: outlook.body-content-type | cadeia de caracteres | O formato da propriedade **corpo** a ser retornada. Os valores podem ser "text" ou "html". Um cabeçalho `Preference-Applied` é retornado como confirmação se este cabeçalho `Prefer` for especificado. Se o cabeçalho não for especificado, a propriedade **corpo** será retornada no formato HTML. Opcional. |

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna o código de resposta `200 OK` e um objeto [event](../resources/event.md) no corpo da resposta.
## <a name="examples"></a>Exemplos

### <a name="example-1-get-a-specified-event"></a>Exemplo 1: Obter um evento especificado
#### <a name="request"></a>Solicitação
O exemplo a seguir obtém o evento especificado. Especifica o seguinte:

- um cabeçalho `Prefer: outlook.timezone` para obter valores de data/hora retornados na Hora Oficial do Pacífico. 
- Um parâmetro de consulta `$select` para retornar propriedades específicas. Sem um parâmetro `$select`, todas as propriedades do evento serão retornadas.

A solicitação não especifica nenhum cabeçalho `Prefer: outlook.body-content-type` para indicar um formato específico para o corpo do evento retornado. 


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_event"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/events/AAMkAGIAAAoZDOFAAA=/?$select=subject,body,bodyPreview,organizer,attendees,start,end,location,hideAttendees 
Prefer: outlook.timezone="Pacific Standard Time"
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-event-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-event-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-event-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-event-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Como nenhum cabeçalho `Prefer: outlook.body-content-type` foi especificado, a propriedade **body** será retornada no formato HTML padrão. 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Preference-Applied: outlook.timezone="Pacific Standard Time"

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('cd209b0b-3f83-4c35-82d2-d88a61820480')/events(subject,body,bodyPreview,organizer,attendees,start,end,location,hideAttendees)/$entity",
    "@odata.etag":"W/\"ZlnW4RIAV06KYYwlrfNZvQAAKGWwbw==\"",
    "id":"AAMkAGIAAAoZDOFAAA=",
    "subject":"Orientation ",
    "bodyPreview":"Dana, this is the time you selected for our orientation. Please bring the notes I sent you.",
    "body":{
        "contentType":"html",
        "content":"<html><head></head><body><p>Dana, this is the time you selected for our orientation. Please bring the notes I sent you.</p></body></html>"
    },
    "start":{
        "dateTime":"2017-04-21T10:00:00.0000000",
        "timeZone":"Pacific Standard Time"
    },
    "end":{
        "dateTime":"2017-04-21T12:00:00.0000000",
        "timeZone":"Pacific Standard Time"
    },
    "location": {
        "displayName": "Assembly Hall",
        "locationType": "default",
        "uniqueId": "Assembly Hall",
        "uniqueIdType": "private"
    },
    "locations": [
        {
            "displayName": "Assembly Hall",
            "locationType": "default",
            "uniqueIdType": "unknown"
        }
    ],
    "attendees":[
        {
            "type":"required",
            "status":{
                "response":"none",
                "time":"0001-01-01T00:00:00Z"
            },
            "emailAddress":{
                "name":"Samantha Booth",
                "address":"samanthab@a830edad905084922E17020313.onmicrosoft.com"
            }
        },
        {
            "type":"required",
            "status":{
                "response":"tentativelyAccepted",
                "time":"0001-01-01T00:00:00Z"
            },
            "proposedNewTime": {
                "start": {
                    "dateTime": "2019-08-16T12:00:00.0000000",
                    "timeZone": "Pacific Standard Time"
                },
                "end": {
                    "dateTime": "2019-08-16T14:00:00.0000000",
                    "timeZone": "Pacific Standard Time"
                }
            },
            "emailAddress":{
                "name":"Dana Swope",
                "address":"danas@a830edad905084922E17020313.onmicrosoft.com"
            }
        }
    ],
    "hideAttendees": false,
    "organizer":{
        "emailAddress":{
            "name":"Samantha Booth",
            "address":"samanthab@a830edad905084922E17020313.onmicrosoft.com"
        }
    }
}
```
### <a name="example-2-get-the-body-property-in-text-format"></a>Exemplo 2: Obter a propriedade body no formato de texto
#### <a name="request"></a>Solicitação
O exemplo a seguir mostra como usar um header para obter a propriedade body do `Prefer: outlook.body-content-type="text"` evento especificado no formato de texto. 

A solicitação também usa um parâmetro de consulta `$select` para retornar propriedades específicas. Sem um parâmetro `$select`, todas as propriedades do evento serão retornadas.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_event_in_text"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/events/AAMkAGI1AAAoZDOFAAA=/?$select=subject,body,bodyPreview
Prefer: outlook.body-content-type="text"
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-event-in-text-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-event-in-text-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-event-in-text-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-event-in-text-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. A propriedade **body** é retornada no formato de texto. 

<!-- {
  "blockType": "response",
  "name": "get_event_in_text",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Preference-Applied: outlook.body-content-type="text"

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('cd209b0b-3f83-4c35-82d2-d88a61820480')/events(subject,body,bodyPreview)/$entity",
    "@odata.etag":"W/\"ZlnW4RIAV06KYYwlrfNZvQAAKGWwbw==\"",
    "id":"AAMkAGI1AAAoZDOFAAA=",
    "subject":"Orientation ",
    "bodyPreview":"Dana, this is the time you selected for our orientation. Please bring the notes I sent you.",
    "body":{
        "contentType":"text",
        "content":"Dana, this is the time you selected for our orientation. Please bring the notes I sent you.\r\n"
    }
}
```

### <a name="example-3-get-an-event-that-specifies-more-than-one-location"></a>Exemplo 3: Obter um evento que especifica mais de um local
#### <a name="request"></a>Solicitação

O exemplo a seguir mostra como obter um evento que especifica mais de um local. Uma solicitação especifica um parâmetro de consulta `$select` para retornar propriedades específicas. 


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_event_multiple_locations"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/events/AAMkADAGAADDdm4NAAA=/?$select=subject,body,bodyPreview,organizer,attendees,start,end,location,locations
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-event-multiple-locations-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-event-multiple-locations-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-event-multiple-locations-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-event-multiple-locations-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>Resposta
A propriedade **locations** inclui detalhes dos três locais para os quais o evento é organizado. 

Como a solicitação não especifica nenhum ou um header, as propriedades inicial e final são exibidas no fuso horário UTC padrão e o corpo está no `Prefer: outlook.timezone` `Prefer: outlook.body-content-type` formato HTML padrão.    

<!-- {
  "blockType": "response",
  "name": "get_event_multiple_locations",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('d1a2fae9-db66-4cc9-8133-2184c77af1b8')/events(subject,body,bodyPreview,organizer,attendees,start,end,location,locations)/$entity",
  "@odata.etag":"W/\"y53lbKh6jkaxHzFwGhgyxgAAw5zhug==\"",
  "id":"AAMkADAGAADDdm4NAAA=",
  "subject":"Plan summer company picnic",
  "bodyPreview":"Let's kick-start this event planning!",
  "body":{
    "contentType":"html",
    "content":"<html>\r\n<head>\r\n</head>\r\n<body>\r\nLet's kick-start this event planning!\r\n</body>\r\n</html>\r\n"
  },
  "start":{
    "dateTime":"2017-08-30T11:00:00.0000000",
    "timeZone":"UTC"
  },
  "end":{
    "dateTime":"2017-08-30T12:00:00.0000000",
    "timeZone":"UTC"
  },
  "location":{
    "displayName":"Conf Room 3; Fourth Coffee; Home Office",
    "locationType":"default",
    "uniqueId":"Conf Room 3; Fourth Coffee; Home Office",
    "uniqueIdType":"private"
  },
  "locations":[
    {
      "displayName":"Conf Room 3",
      "locationType":"default",
      "uniqueIdType":"unknown"
    },
    {
      "displayName":"Fourth Coffee",
      "locationType":"default",
      "uniqueId":"Fourth Coffee",
      "uniqueIdType":"private",
      "address":{
        "type":"unknown",
        "street":"4567 Main St",
        "city":"Redmond",
        "state":"WA",
        "countryOrRegion":"US",
        "postalCode":"32008"
      },
      "coordinates":{
        "latitude":47.672,
        "longitude":-102.103
      }
    },
    {
      "displayName":"Home Office",
      "locationType":"default",
      "uniqueIdType":"unknown"
    }
  ],
  "attendees":[
    {
      "type":"required",
      "status":{
        "response":"none",
        "time":"0001-01-01T00:00:00Z"
      },
      "emailAddress":{
        "name":"Dana Swope",
        "address":"DanaS@contoso.onmicrosoft.com"
      }
    },
    {
      "type":"required",
      "status":{
        "response":"none",
        "time":"0001-01-01T00:00:00Z"
      },
      "emailAddress":{
        "name":"Alex Wilber",
        "address":"AlexW@contoso.onmicrosoft.com"
      }
    }
  ],
  "organizer":{
    "emailAddress":{
      "name":"Adele Vance",
      "address":"AdeleV@contoso.onmicrosoft.com"
    }
  }
}
```
### <a name="example-4-expand-a-series-master-event"></a>Exemplo 4: Expandir um evento mestre de série
#### <a name="request"></a>Solicitação

O exemplo a seguir mostra a expansão de um evento mestre de série de uma série recorrente com exceções e ocorrências canceladas. Uma solicitação especifica um parâmetro de consulta `$select` para retornar propriedades específicas. 

<!-- {
  "blockType": "request",
  "name": "get_event_seriesMaster_expansion"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/events/AAMkADAGAADDdm4NAAA=/?$select=subject,start,end,occurrenceId,exceptionOccurrences,cancelledOccurrences$expand=exceptionOccurrences
```
#### <a name="response"></a>Resposta
A operação GET retorna as propriedades selecionadas para o evento mestre da série. Especificamente, para eventos na coleção **exceptionOccurrences,** a operação retorna a propriedade **id** e as propriedades selecionadas aplicáveis (**subject**, **start**, **end**, **occurrenceId**). Quanto aos eventos na coleção **cancelledOccurrences,** como os eventos não existem mais, a operação retorna apenas seus valores de propriedade **occurrenceId.**

<!-- {
  "blockType": "response",
  "name": "get_event_seriesMaster_expansion",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('d1a2fae9-db66-4cc9-8133-2184c77af1b8')/events(subject,start,end,occurrenceId,exceptionOccurrences,cancelledOccurrences)/$entity",
  "@odata.etag":"W/\"y53lbKh6jkaxHzFwGhgyxgAAw5zhug==\"",
  "id":"AAMkADAGAADDdm4NAAA=",
  "subject": "Daily stand-up",
  "cancelledOccurrences": [
     "OID.AAMkADAGAADDdm4NAAA=.2020-04-30",
     "OID.AAMkADAGAADDdm4NAAA=.2020-05-07",
     "OID.AAMkADAGAADDdm4NAAA=.2020-05-14"
    ],
  "occurrenceId": null,
    "start": {
        "dateTime": "2020-04-23T11:30:00.0000000",
        "timeZone": "UTC"
    },
  "end": {
        "dateTime": "2020-04-23T12:00:00.0000000",
        "timeZone": "UTC"
    },
  "exceptionOccurrences": [
        {
            "id": "AAMkADM0ZGRhMjdjLTA==",
            "Subject": "SM update 24",
            "occurrenceId": "OID.AAMkADAGAADDdm4NAAA=.2020-05-21",
            "start": {
                "dateTime": "2020-05-21T11:30:00.0000000",
                "timeZone": "UTC"
            },
            "end": {
                "dateTime": "2020-05-21T12:00:00.0000000",
                "timeZone": "UTC"
            }
        }
    ]
}
```

## <a name="see-also"></a>Confira também

- [Adicionar dados personalizados a recursos usando extensões](/graph/extensibility-overview)
- [Adicionar dados personalizados aos usuários usando extensões abertas](/graph/extensibility-open-users)
- [Adicionar dados personalizados a grupos usando as extensões do esquema](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get event",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


