---
title: Obter as alterações incrementais para os eventos em um modo de exibição de calendário
description: Acompanhe as alterações de eventos no modo de exibição de calendário usando solicitações GET com a função delta. O exemplo mostra como sincronizar o calendário padrão de um usuário em um intervalo de tempo definido.
author: FaithOmbongi
ms.localizationpriority: high
ms.custom: graphiamtop20
ms.openlocfilehash: 9616e0c9f3d041495a68929045f68a87fbe7a24d
ms.sourcegitcommit: e48fe05125fe1e857225d20ab278352ff7f0911a
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2022
ms.locfileid: "66555685"
---
# <a name="get-incremental-changes-to-events-in-a-calendar-view"></a>Obter as alterações incrementais para os eventos em um modo de exibição de calendário

Ao usar a consulta delta, você pode obter eventos novos, atualizados ou excluídos em um calendário especificado, ou dentro de uma coleção definida de eventos (como um modo de exibição de calendário) no calendário. Este artigo descreve o último: obter essas alterações incrementais nos eventos em um modo de exibição de calendário.

> [!NOTE]
> O recurso para o primeiro&mdash;obter alterações incrementais nos eventos em um calendário não vinculado a um período fixo de datas de início e de término&mdash;está disponível atualmente apenas na versão beta. Para saber mais, confira a função[delta](/graph/api/event-delta).

O modo de visualização de calendário em um conjunto de eventos em um intervalo de data/horário (../me/calendarview) do calendário padrão, ou de outro calendário especificado ou de um calendário de grupo. Os eventos retornados podem incluir instâncias únicas, ou ocorrências e exceções de uma série recorrente. Os dados delta permitem manter e sincronizar o armazenamento local de eventos do usuário, sem ter de buscar todo o conjunto de eventos do usuário no servidor a cada vez que precise deles.

A consulta delta oferece suporte à sincronização completa que recupera todos os eventos no modo de exibição calendário especificado e a sincronização incremental que recupera os eventos ocorridos no modo de exibição de calendário desde a última sincronização. Normalmente, você faria uma sincronização completa inicial, e posteriormente obteria alterações incrementais para esse modo de exibição de calendário periodicamente.

## <a name="track-event-changes-in-a-calendar-view"></a>Rastrear alterações de evento em um modo de exibição de calendário

A consulta delta para eventos em uma exibição de calendário é específica para um calendário e um intervalo de data/hora que você especificar. Para controlar as alterações em vários calendários, você precisa acompanhar cada calendário individualmente.

O rastreamento de alterações de evento em um modo de exibição de calendário normalmente corresponde a uma série de eventos de uma ou mais solicitações GET com a função [delta](/graph/api/event-delta). A solicitação GET inicial é muito semelhante à maneira como você [lista uma calendarView](/graph/api/calendar-list-calendarview), exceto se você incluir a função **delta**. A seguir está a solicitação delta GET inicial de um modo de exibição de calendário no calendário padrão do usuário conectado:

```
GET /me/calendarView/delta?startDateTime={start_datetime}&endDateTime={end_datetime}
```

Uma solicitação GET com a função **delta** retorna:

- Uma `@odata.nextLink` (que contém uma URL com uma chamada de função **delta** e uma `$skipToken`) ou 
- Uma `@odata.deltaLink` (que contém uma URL com uma chamada de função **delta** e `$deltaToken`).

Esses tokens são [tokens de estado](delta-query-overview.md#state-tokens) que codificam os parâmetros _startDateTime_ e _endDateTime_, bem como qualquer outro parâmetro de consulta em sua solicitação GET de consulta delta inicial. Não é necessário incluir esses parâmetros em solicitações subsequentes, uma vez que eles são codificados nos tokens.

Estabeleça tokens de estado que sejam completamente opacos para o cliente. Para prosseguir com uma fase de controle de alterações, basta copiar e aplicar a URL `@odata.nextLink` ou `@odata.deltaLink` retornada da última solicitação GET para a próxima chamada de função **delta** do mesmo modo de exibição de calendário. Uma `@odata.deltaLink` retornada em uma resposta significa que a fase atual do rastreamento de alterações está concluída. Você pode salvar e usar a URL `@odata.deltaLink` quando começar a próxima fase.

Verifique o [exemplo](#example-synchronize-events-in-a-calendar-view) para aprender a usar essas URLs `@odata.nextLink` e `@odata.deltaLink`.

### <a name="use-query-parameters-in-a-delta-query-for-calendar-view"></a>Use os parâmetros de consulta de uma consulta delta para a visualização de calendário

- Inclua os parâmetros _startDateTime_ e _endDateTime_ para definir um intervalo de data/hora para o modo de exibição de calendário.
- Não há suporte para `$select`.


### <a name="optional-request-header"></a>Cabeçalhos de solicitação opcionais

Cada solicitação GET de consulta delta retorna um conjunto de um ou mais eventos na resposta. Como alternativa, você pode especificar o cabeçalho de solicitação, `Prefer: odata.maxpagesize={x}`, para configurar o máximo de eventos em uma resposta.


## <a name="example-synchronize-events-in-a-calendar-view"></a>Exemplo: sincronização de eventos em um modo de exibição de calendário

O exemplo a seguir mostra uma série de 3 solicitações para sincronizar o calendário de padrão do usuário em um intervalo de tempo específico. Há 5 eventos nesse modo de exibição de calendário.

- [Etapa 1: exemplo inicial de solicitação](#step-1-sample-initial-request) e [resposta](#sample-initial-response)
- [Etapa 2: segundo exemplo de solicitação](#step-2-sample-second-request) e [resposta](#sample-second-response)
- [Etapa 3: terceiro exemplo de solicitação](#step-3-sample-third-request) e [resposta](#sample-third-and-final-response)

Para economizar tempo, as respostas de exemplo exibem apenas um subconjunto das propriedades para um evento. Em uma chamada real, a maior parte das propriedades dos eventos são retornadas. 

Confira o que você fará na [próxima fase](#the-next-round-sample-first-response).


### <a name="step-1-sample-initial-request"></a>Passo 1: solicitação inicial de exemplo

Neste exemplo, a exibição de calendário especificada no calendário padrão do usuário conectado está sendo sincronizada pela primeira vez, portanto, a solicitação de sincronização inicial não inclui nenhum token de estado. Esta rodada retornará todos os eventos nesse modo de exibição de calendário.

A primeira solicitação especifica o seguinte:

- Data/horário valores para os parâmetros _startDateTime_ e _endDateTime_.
- O [cabeçalho de solicitação opcional](#optional-request-header), _odata.maxpagesize_, retornando 2 eventos de cada vez.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendarview_delta_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/calendarView/delta?startdatetime=2016-12-01T00:00:00Z&enddatetime=2016-12-30T00:00:00Z HTTP/1.1
Prefer: odata.maxpagesize=2
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendarview-delta-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendarview-delta-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendarview-delta-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-calendarview-delta-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="sample-initial-response"></a>Resposta inicial de exemplo

A resposta inclui dois eventos e um `@odata.nextLink`cabeçalho de resposta com um `skipToken`. A URL `@odata.nextLink` indica que há mais eventos no modo de exibição de calendário a ser obtidos.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#Collection(event)",
    "@odata.nextLink":"https://graph.microsoft.com/v1.0/me/calendarView/delta?$skiptoken=R0usmcCM996atia_s",
    "value":[
        {
            "@odata.type":"#microsoft.graph.event",
            "@odata.etag":"W/\"EZ9r3czxY0m2jz8c45czkwAAFXcvIQ==\"",
            "subject":"Plan shopping list",
            "body":{
                "contentType":"html",
                "content":""
            },
            "start":{
                "dateTime":"2016-12-09T20:30:00.0000000",
                "timeZone":"UTC"
            },
            "end":{
                "dateTime":"2016-12-09T22:00:00.0000000",
                "timeZone":"UTC"
            },
            "attendees":[

            ],
            "organizer":{
                "emailAddress":{
                    "name":"Samantha Booth",
                    "address":"samanthab@contoso.onmicrosoft.com"
                }
            },      
            "id":"AAMkADNVxRAAA="
        },
        {
            "@odata.type":"#microsoft.graph.event",
            "@odata.etag":"W/\"EZ9r3czxY0m2jz8c45czkwAAFXcvIg==\"",
            "subject":"Pick up car",
            "body":{
                "contentType":"html",
                "content":""
            },
            "start":{
                "dateTime":"2016-12-10T01:00:00.0000000",
                "timeZone":"UTC"
            },
            "end":{
                "dateTime":"2016-12-10T02:00:00.0000000",
                "timeZone":"UTC"
            },
            "attendees":[

            ],
            "organizer":{
                "emailAddress":{
                    "name":"Samantha Booth",
                    "address":"samanthab@contoso.onmicrosoft.com"
                }
            },
            "id":"AAMkADVxSAAA="
        }
    ]
}
```

### <a name="step-2-sample-second-request"></a>Etapa 2: segundo exemplo de solicitação

A segunda solicitação especifica a URL `@odata.nextLink` retornada da resposta anterior. Observe que não é mais necessário especificar os mesmos parâmetros _startDateTime_ e _endDateTime_ como na solicitação inicial, conforme o `skipToken` na URL `@odata.nextLink` os codifica e inclui.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendarview_delta_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/calendarView/delta?$skiptoken=R0usmcCM996atia_s HTTP/1.1
Prefer: odata.maxpagesize=2
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendarview-delta-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendarview-delta-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendarview-delta-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-calendarview-delta-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="sample-second-response"></a>Segunda resposta de exemplo 

A segunda resposta retorna os 2 próximos eventos no modo de visualização de calendário e outro `@odata.nextLink`, indicando que há mais eventos a ser obtidos no modo de exibição de calendário.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#Collection(event)",
    "@odata.nextLink":"https://graph.microsoft.com/v1.0/me/calendarView/delta?$skiptoken=R0usmci39OQxqJrxK4",
    "value":[
        {
            "@odata.type":"#microsoft.graph.event",
            "@odata.etag":"W/\"EZ9r3czxY0m2jz8c45czkwAAFXcvIw==\"",
            "subject":"Get food",
            "body":{
                "contentType":"html",
                "content":""
            },
            "start":{
                "dateTime":"2016-12-10T19:30:00.0000000",
                "timeZone":"UTC"
            },
            "end":{
                "dateTime":"2016-12-10T21:30:00.0000000",
                "timeZone":"UTC"
            },
            "attendees":[

            ],
            "organizer":{
                "emailAddress":{
                    "name":"Samantha Booth",
                    "address":"samanthab@contoso.onmicrosoft.com"
                }
            },
            "id":"AAMkADVxTAAA="
        },
        {
            "@odata.type":"#microsoft.graph.event",
            "@odata.etag":"W/\"EZ9r3czxY0m2jz8c45czkwAAFXcvJA==\"",
            "subject":"Prepare food",
            "body":{
                "contentType":"html",
                "content":""
            },
            "start":{
                "dateTime":"2016-12-10T22:00:00.0000000",
                "timeZone":"UTC"
            },
            "end":{
                "dateTime":"2016-12-11T00:00:00.0000000",
                "timeZone":"UTC"
            },
            "attendees":[

            ],
            "organizer":{
                "emailAddress":{
                    "name":"Samantha Booth",
                    "address":"samanthab@contoso.onmicrosoft.com"
                }
            },
            "id":"AAMkADVxUAAA="
        }
    ]
}
```


### <a name="step-3-sample-third-request"></a>Etapa 3: terceira solicitação de exemplo

A terceira solicitação continua a usar as últimas `@odata.nextLink` retornadas da última solicitação de sincronização. 
 


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendarview_delta_3"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/calendarView/delta?$skiptoken=R0usmci39OQxqJrxK4 HTTP/1.1
Prefer: odata.maxpagesize=2
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendarview-delta-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendarview-delta-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendarview-delta-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-calendarview-delta-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="sample-third-and-final-response"></a>Terceira e última resposta de exemplo

A terceira resposta retorna o único evento restante no modo de exibição calendário e uma URL `@odata.deltaLink` a indicar que a sincronização está concluída para esse modo de exibição de calendário. Salvar e usar a URL `@odata.deltaLink` para [sincronizar esse modo de exibição de calendário na próxima fase](#the-next-round-sample-first-request).


<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#Collection(event)",
    "@odata.deltaLink":"https://graph.microsoft.com/v1.0/me/calendarView/delta?$deltatoken=R0usmcMDNGg0J1E",
    "value":[
        {
            "@odata.type":"#microsoft.graph.event",
            "@odata.etag":"W/\"EZ9r3czxY0m2jz8c45czkwAALZu97g==\"",
            "subject":"Rest!",
            "body":{
                "contentType":"html",
                "content":""
            },
            "start":{
                "dateTime":"2016-12-12T02:00:00.0000000",
                "timeZone":"UTC"
            },
            "end":{
                "dateTime":"2016-12-12T07:30:00.0000000",
                "timeZone":"UTC"
            },
            "location":{
                "displayName":"Home"
            },
            "attendees":[

            ],
            "organizer":{
                "emailAddress":{
                    "name":"Samantha Booth",
                    "address":"samanthab@contoso.onmicrosoft.com"
                }
            },
            "id":"AAMkADj1HuAAA="
        }
    ]
}
```


### <a name="the-next-round-sample-first-request"></a>A próxima fase: primeira solicitação de exemplo

Usando o `@odata.deltaLink` da [última solicitação](#step-3-sample-third-request) na última fase, você poderá obter somente os eventos que sofreram alteração (por serem adicionados, excluídos ou atualizados) nesse modo de exibição de calendário desde então. Sua primeira solicitação na próxima fase terá aparência semelhante à seguinte, supondo que você prefira manter o mesmo tamanho máximo de página na resposta:


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendarview_delta_next"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/calendarView/delta?$deltatoken=R0usmcMDNGg0J1E HTTP/1.1
Prefer: odata.maxpagesize=2
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendarview-delta-next-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendarview-delta-next-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendarview-delta-next-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-calendarview-delta-next-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="the-next-round-sample-first-response"></a>A próxima fase: primeira resposta de exemplo

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#Collection(event)",
    "@odata.deltaLink":"https://graph.microsoft.com/v1.0/me/calendarView/delta?$deltatoken=R0usmcFuQtZdtpk4",
    "value":[
        {
            "@odata.type": "#microsoft.graph.event",
            "id": "AAMkADk0MGFkODE3LWE4MmYtNDRhOS04OGQLkRkXbBznTvAADb6ytyAAA=",
            "@removed": {
                "reason": "deleted"
            }
        },
        {
            "@odata.type":"#microsoft.graph.event",
            "@odata.etag":"W/\"EZ9r3czxY0m2jz8c45czkwAALZu97w==\"",
            "subject":"Attend service",
            "body":{
                "contentType":"html",
                "content":""
            },
            "start":{
                "dateTime":"2016-12-25T06:00:00.0000000",
                "timeZone":"UTC"
            },
            "end":{
                "dateTime":"2016-12-25T07:30:00.0000000",
                "timeZone":"UTC"
            },
            "location":{
                "displayName":"Chapel of Saint Ignatius",
                "address":{
                    "street":"900 Broadway",
                    "city":"Seattle",
                    "state":"WA",
                    "countryOrRegion":"United States",
                    "postalCode":""
                },
                "coordinates":{
                    "latitude":47.6105,
                    "longitude":-122.321
                }
            },
            "attendees":[

            ],
            "organizer":{
                "emailAddress":{
                    "name":"Samantha Booth",
                    "address":"samanthab@contoso.onmicrosoft.com"
                }
            },
            "id":"AAMkADj1HvAAA="
        }
    ]
}
```

## <a name="see-also"></a>Confira também

- [Consulta delta do Microsoft Graph](delta-query-overview.md)
- [Obter as alterações incrementais para mensagens](delta-query-messages.md)
- [Obter as alterações incrementais para grupos](delta-query-groups.md)
- [Obter as alterações incrementais para usuários](delta-query-users.md)
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example to synchronize events in a calendar view",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
