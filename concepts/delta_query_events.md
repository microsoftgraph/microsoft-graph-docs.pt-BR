# <a name="get-incremental-changes-to-events-in-a-calendar-view"></a>Obter as alterações incrementais para os eventos em um modo de exibição de calendário 

O modo de visualização de calendário em um conjunto de eventos em um intervalo de data/horário do calendário-padrão (../me/calendarview) ou algum outro calendário do usuário. Usando a consulta de delta, você pode obter eventos novos, atualizados ou excluídos em um modo de exibição de calendário. Os eventos retornados podem incluir ocorrências e exceções de uma série recorrente e instâncias únicas. Os dados-delta permitem manter e sincronizar o armazenamento local de eventos do usuário, sem ter de buscar todo o conjunto de eventos do usuário no servidor a cada vez que precise deles.

A consulta delta oferece suporte à sincronização completa que recupera todos os eventos no modo de exibição calendário especificado e a sincronização incremental que recupera os eventos ocorridos no modo de exibição de calendário desde a última sincronização. Normalmente, você faria uma sincronização completa inicial e, logo após, obteria, periodicamente, as alterações incrementais para esse modo de exibição de calendário. 

## <a name="track-event-changes-in-a-calendar-view"></a>Rastrear alterações de evento em um modo de exibição de calendário

A consulta delta para eventos é específica de um intervalo de calendário e data/hora que você especificar (ou seja, um modo de exibição de calendário). Para controlar as alterações em vários calendários, você precisa controlar cada calendário individualmente. 

O rastreamento de alterações de evento em um modo de exibição de calendário normalmente corresponde a uma série de eventos de uma ou mais solicitações GET com a função [delta](../api-reference/v1.0/api/event_delta.md). A solicitação GET inicial é muito semelhante à maneira como você [lista uma calendarView](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/calendar_list_calendarview), exceto se você incluir a função **delta**:

```
GET /me/calendarView/delta?startDateTime={start_datetime}&endDateTime={end_datetime}
```

Uma solicitação GET com a função **delta** retorna:

- Uma `nextLink` (que contém uma URL com chamada de função **delta** e um _skipToken_) ou 
- Uma `deltaLink` (que contém uma URL com chamada de função **delta** e _deltaToken_).

Esses tokens são [tokens de estado](delta_query_overview.md#state-tokens) que codificam os parâmetros refs/remotes/microsoftgraph/master _startDateTime_ e _endDateTime_, bem como qualquer outro parâmetro de consulta em sua solicitação GET de consulta delta inicial. 

Estabeleça tokens de estado que sejam completamente opacos para o cliente. Para prosseguir com uma fase de controle de alterações, basta copiar e aplicar a URL `nextLink` ou `deltaLink` retornada da última solicitação GET para a próxima chamada de função **delta** do mesmo modo de exibição de calendário. Uma `deltaLink` retornada em uma resposta significa que a fase atual do rastreamento de alterações está concluída. Você pode salvar e usar a URL `deltaLink` quando começar a próxima fase.

Verifique o [exemplo](#example-to-synchronize-events-in-a-calendar-view) abaixo para aprender a usar essas URLs `nextLink` e `deltaLink`.

### <a name="use-query-parameters-in-a-delta-query-for-calendar-view"></a>Use os parâmetros de consulta de uma consulta delta para a visualização de calendário

- Inclua os parâmetros _startDateTime_ e _endDateTime_ para definir um intervalo de data/hora para o modo de exibição de calendário.
- Não há suporte para `$select`.


### <a name="optional-request-header"></a>Cabeçalhos de solicitação opcionais

Cada solicitação GET de consulta delta retorna um conjunto de um ou mais eventos na resposta. Como alternativa, você pode especificar o cabeçalho de solicitação, _Prefer: odata.maxpagesize={x}_, para configurar o máximo de eventos em uma resposta.


## <a name="example-to-synchronize-events-in-a-calendar-view"></a>Exemplo de sincronização de eventos em um modo de exibição de calendário

O exemplo a seguir mostra uma série de 3 solicitações para sincronizar o calendário de padrão do usuário em um intervalo de tempo específico. Há 5 eventos nesse modo de exibição de calendário.

- [Etapa 1: exemplo inicial de solicitação](#step-1-sample-initial-request) e [resposta](#sample-initial-response)
- [Etapa 2: segundo exemplo de solicitação](#step-2-sample-second-request) e [resposta](#sample-second-response)
- [Etapa 3: terceiro exemplo de solicitação](#step-3-sample-third-request) e [resposta](#sample-third-and-final-response)

Para economizar tempo, as respostas de exemplo exibem apenas um subconjunto das propriedades para um evento. Em uma chamada real, a maior parte das propriedades dos eventos são retornadas. 

Consulte também o que você vai fazer na [próxima fase](#the-next-round-sample-first-response).


### <a name="step-1-sample-initial-request"></a>Passo 1: solicitação inicial de exemplo

Neste exemplo, o modo de exibição de calendário especificado está sendo sincronizado pela primeira vez, para que a solicitação de sincronização inicial não inclua nenhum token de estado. Esta fase retornará todos os eventos nesse modo de exibição de calendário.

A primeira solicitação especifica o seguinte:

- Data/horário valores para os parâmetros _startDateTime_ e _endDateTime_.
- O [cabeçalho de solicitação opcional](#optional-request-header), _odata.maxpagesize_, retornando 2 eventos de cada vez.

<!-- {
  "blockType": "request",
  "name": "get_calendarview_delta_1"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendarview/delta?startdatetime=2016-12-01T00:00:00Z&enddatetime=2016-12-30T00:00:00Z HTTP/1.1
Prefer: odata.maxpagesize=2
```


### <a name="sample-initial-response"></a>Resposta inicial de exemplo

A resposta inclui dois eventos e um `@odata.nextLink`cabeçalho de resposta com um `skipToken`. A URL `nextLink` indica que há mais eventos no modo de exibição de calendário a ser obtidos.

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
    "@odata.nextLink":"https://graph.microsoft.com/v1.0/me/calendarview/delta?$skiptoken=R0usmcCM996atia_s",
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
                    "name":"Fanny Downs",
                    "address":"fannyd@contoso.onmicrosoft.com"
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
                    "name":"Fanny Downs",
                    "address":"fannyd@contoso.onmicrosoft.com"
                }
            },
            "id":"AAMkADVxSAAA="
        }
    ]
}
```

### <a name="step-2-sample-second-request"></a>Etapa 2: segundo exemplo de solicitação

A segunda solicitação especifica a URL `nextLink` retornada da resposta anterior. Observe que não é mais necessário especificar os mesmos parâmetros _startDateTime_ e _endDateTime_ como na solicitação inicial, conforme o `skipToken` na URL `nextLink` os codifica e inclui.

<!-- {
  "blockType": "request",
  "name": "get_calendarview_delta_2"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendarview/delta?$skiptoken=R0usmcCM996atia_s HTTP/1.1
Prefer: odata.maxpagesize=2
```

### <a name="sample-second-response"></a>Segunda resposta de exemplo 

A segunda resposta retorna os 2 próximos eventos no modo de visualização de calendário e outro `nextLink`, indicando que há mais eventos a ser obtidos no modo de exibição de calendário.

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
    "@odata.nextLink":"https://graph.microsoft.com/v1.0/me/calendarview/delta?$skiptoken=R0usmci39OQxqJrxK4",
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
                    "name":"Fanny Downs",
                    "address":"fannyd@contoso.onmicrosoft.com"
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
                    "name":"Fanny Downs",
                    "address":"fannyd@contoso.onmicrosoft.com"
                }
            },
            "id":"AAMkADVxUAAA="
        }
    ]
}
```


### <a name="step-3-sample-third-request"></a>Etapa 3: terceira solicitação de exemplo

A terceira solicitação continua a usar as últimas `nextLink` retornadas da última solicitação de sincronização. 
 

<!-- {
  "blockType": "request",
  "name": "get_calendarview_delta_3"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendarview/delta?$skiptoken=R0usmci39OQxqJrxK4 HTTP/1.1
Prefer: odata.maxpagesize=2
```

### <a name="sample-third-and-final-response"></a>Terceira e última resposta de exemplo

A terceira resposta retorna o único evento restante no modo de exibição calendário e uma URL `deltaLink` a indicar que a sincronização está concluída para esse modo de exibição de calendário. Salvar e usar a URL `deltaLink` para [sincronizar esse modo de exibição de calendário na próxima fase](#the-next-round-sample-first-request).


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
    "@odata.deltaLink":"https://graph.microsoft.com/v1.0/me/calendarview/delta?$deltatoken=R0usmcMDNGg0J1E",
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
                    "name":"Fanny Downs",
                    "address":"fannyd@contoso.onmicrosoft.com"
                }
            },
            "id":"AAMkADj1HuAAA="
        }
    ]
}
```


### <a name="the-next-round-sample-first-request"></a>A próxima fase: primeira solicitação de exemplo

Usando o `deltaLink` da [última solicitação](#step-3-sample-third-request) na última fase, você poderá obter somente os eventos que sofreram alteração (por serem adicionados, excluídos ou atualizados) nesse modo de exibição de calendário desde então. Sua primeira solicitação na próxima fase terá aparência semelhante à seguinte, supondo que você prefira manter o mesmo tamanho máximo de página na resposta:

<!-- {
  "blockType": "request",
  "name": "get_calendarview_delta_next"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendarview/delta?$deltatoken=R0usmcMDNGg0J1E HTTP/1.1
Prefer: odata.maxpagesize=2
```

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
    "@odata.deltaLink":"https://graph.microsoft.com/v1.0/me/calendarview/delta?$deltatoken=R0usmcFuQtZdtpk4",
    "value":[
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
                    "type":"unknown",
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
                    "name":"Fanny Downs",
                    "address":"fannyd@contoso.onmicrosoft.com"
                }
            },
            "id":"AAMkADj1HvAAA="
        }
    ]
}
```

## <a name="see-also"></a>Veja também

- [Consulta delta do Microsoft Graph](../Concepts/delta_query_overview.md)
- [Obter as alterações incrementais para mensagens](../Concepts/delta_query_messages.md)
- [Obter as alterações incrementais para grupos](../Concepts/delta_query_groups.md)
- [Obter as alterações incrementais para usuários](../Concepts/delta_query_users.md)
