---
title: Propor novos horários de reunião no Outlook
description: No Outlook, o organizador da reunião pode permitir que os convidados proponham horários alternativos.
author: harini84
ms.localizationpriority: high
ms.prod: outlook
ms.openlocfilehash: eb75a950f627dde2cf54f373e17435b501a082df
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59103946"
---
# <a name="propose-new-meeting-times-in-outlook"></a>Propor novos horários de reunião no Outlook

No Outlook, o organizador da reunião pode permitir que os convidados proponham horários de reunião alternativos, se não puderem se encontrar na data/hora original definida e aceitar provisoriamente ou recusar. O organizador pode aceitar uma proposta ajustando o horário da reunião conforme apropriado.

## <a name="example-attendee-responds-tentative-and-suggests-a-different-datetime"></a>Exemplo: o participante responde provisoriamente e sugere uma data/hora diferente
A seguir, é apresentado um exemplo em que Alex convida Adele para almoçar, Adele timidamente aceita e propõe uma data e hora alternativas. Alex aceita a proposta ajustando a reunião de acordo:

1. Como organizador, Alex envia uma solicitação de reunião para Adele. Ele define a propriedade **allowNewTimeProposals** do [evento](/graph/api/resources/event?view=graph-rest-1.0) para `true` para deixar Adele sugerir outro horário se ela precisar.

    <!-- {
      "blockType": "request",
      "name": "create_event"
    }-->
    ```http
    POST https://graph.microsoft.com/v1.0/me/events
    Prefer: outlook.timezone="Pacific Standard Time"
    Content-type: application/json

    {
      "subject": "Let's go for lunch",
      "body": {
        "contentType": "HTML",
        "content": "Does noon work for you?"
      },
      "start": {
          "dateTime": "2019-08-15T12:00:00",
          "timeZone": "Pacific Standard Time"
      },
      "end": {
          "dateTime": "2019-08-15T14:00:00",
          "timeZone": "Pacific Standard Time"
      },
      "allowNewTimeProposals": true,
      "location":{
          "displayName":"Harry's Bar"
      },
      "attendees": [
        {
          "emailAddress": {
          "address":"AdeleV@contoso.OnMicrosoft.com",
          "name": "Adele Vance"
          },
          "type": "required"
        }
      ]
    }
    ```

    Alex recebe a seguinte resposta: 
    <!-- {
      "blockType": "response",
      "name": "create_event",
      "truncated": true,
      "@odata.type": "microsoft.graph.event"
    } -->
    ```http
    HTTP/1.1 201 Created
    Content-type: application/json

    {
      "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('64339082-ed84-4b0b-b4ab-004ae54f3747')/events/$entity",
      "@odata.etag": "W/\"NEXywgsVrkeNsFsyVyRrtAAAAhBhkg==\"",
      "id": "AAMkADAwJXJGu0AAACEhWOAAA=",
      "createdDateTime": "2019-08-01T06:41:07.805128Z",
      "lastModifiedDateTime": "2019-08-01T06:41:08.3298275Z",
      "changeKey": "NEXywgsVrkeNsFsyVyRrtAAAAhBhkg==",
      "categories": [],
      "originalStartTimeZone": "Pacific Standard Time",
      "originalEndTimeZone": "Pacific Standard Time",
      "uid": "0400000082008A9979A0BD16",
      "reminderMinutesBeforeStart": 15,
      "isReminderOn": true,
      "hasAttachments": false,
      "subject": "Let's go for lunch",
      "bodyPreview": "Does noon work for you?",
      "importance": "normal",
      "sensitivity": "normal",
      "isAllDay": false,
      "isCancelled": false,
      "isOrganizer": true,
      "responseRequested": true,
      "seriesMasterId": null,
      "showAs": "busy",
      "type": "singleInstance",
      "webLink": "https://outlook.office365.com/owa/?itemid=AAMkADAwJXJGu0AAACEhWOAAA%3D&exvsurl=1&path=/calendar/item",
      "onlineMeetingUrl": null,
      "allowNewTimeProposals": true,
      "recurrence": null,
      "responseStatus": {
        "response": "organizer",
        "time": "0001-01-01T00:00:00Z"
      },
      "body": {
        "contentType": "html",
        "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\nDoes late morning work for you?\r\n</body>\r\n</html>\r\n"
      },
      "start": {
        "dateTime": "2019-08-15T12:00:00.0000000",
        "timeZone": "Pacific Standard Time"
      },
      "end": {
        "dateTime": "2019-08-15T14:00:00.0000000",
        "timeZone": "Pacific Standard Time"
      },
      "location": {
        "displayName": "Harry's Bar",
        "locationType": "default",
        "uniqueId": "Harry's Bar",
        "uniqueIdType": "private"
      },
     "locations": [
        {
            "displayName": "Harry's Bar",
            "locationType": "default",
            "uniqueId": "Harry's Bar",
            "uniqueIdType": "private"
        }
      ],
      "attendees": [
        {
            "type": "required",
            "status": {
                "response": "none",
                "time": "0001-01-01T00:00:00Z"
            },
            "emailAddress": {
                "name": "Adele Vance",
                "address": "AdeleV@contoso.OnMicrosoft.com"
            }
        }
      ],
      "organizer": {
        "emailAddress": {
            "name": "Alex Wilber",
            "address": "AlexW@contoso.OnMicrosoft.com"
        }
      }
    }
    ```

2. Adele recebe o convite na caixa de entrada como um [eventMessageRequest](/graph/api/resources/eventmessagerequest?view=graph-rest-1.0). Ela observa que a propriedade **allowNewTimeProposals** está definida. [Ao usar o **evento** associado](/graph/api/eventmessage-get?view=graph-rest-1.0#example-2) a esse **eventMessageRequest**, ela responde provisoriamente e propõe o dia seguinte no mesmo horário, no parâmetro de corpo **proposedNewTime**. Ela também define o parâmetro **sendResponse** como verdadeiro.

    <!-- {
      "blockType": "request",
      "name": "event_tentativelyaccept"
    }-->
    ```http
    POST https://graph.microsoft.com/v1.0/me/events/AAMkADU5NRaRqdoI4oeRpAAAB_woNAAA=/tentativelyAccept
    Content-type: application/json

    { 
      "comment": "Can you make the next day instead?", 
      "sendResponse": "true", 
      "proposedNewTime": {
         "Start": { 
              "DateTime": "2019-08-16T12:00:00", 
              "TimeZone": "Pacific Standard Time" 
         }, 
         "End": { 
              "DateTime": "2019-08-16T14:00:00", 
              "TimeZone": "Pacific Standard Time" 
         }
      }
    } 
    ```

    A resposta da Adele é bem-sucedida e ela recebe a seguinte resposta:

    <!-- {
      "blockType": "response",
      "name": "event_tentativelyaccept"
      "truncated": true
    } -->
    ```http
    HTTP/1.1 202 Accepted
    ```

3. Alex recebe um email do tipo [eventMessageResponse](/graph/api/resources/eventmessageresponse?view=graph-rest-1.0). Ele observa o seguinte:

   - O assunto inclui um prefixo e diz "Novo Horário Proposto: Vamos almoçar"
   - O remetente é Adele Vance
   - O **responseType** é `tentativelyAccepted`
   - A proposta de Adele está na propriedade **proposedNewTime** do **eventMessageResponse**

    <!-- {
      "blockType": "request",
      "name": "get_messages"
    }-->
    ```http
    GET https://graph.microsoft.com/v1.0/me/messages?$top=1
    Prefer: outlook.timezone="Pacific Standard Time"
    ```

    Para fins de demonstração, suponha que a resposta de Adele seja a mensagem mais recente na caixa de correio de Alex, e Alex pode simplesmente solicitar a mensagem mais recente.

    <!-- {
      "blockType": "response",
      "name": "get_messages",
      "truncated": true,
      "@odata.type": "microsoft.graph.message",
      "isCollection": true
    } -->
    ```http
    HTTP/1.1 200 OK
    Content-type: application/json
    Preference-Applied: outlook.timezone="Pacific Standard Time"

    {
       "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('64339082-ed84-4b0b-b4ab-004ae54f3747')/messages",
       "@odata.nextLink": "https://graph.microsoft.com/v1.0/me/messages?$top=1&$skip=4"",
       "value": [
          {
            "@odata.type": "#microsoft.graph.eventMessageResponse",
            "@odata.etag": "W/\"DAAAABYAAAA0RfLCCxWuR42wWzJXJGu0AAACEGHC\"",
            "id": "AAMkADAwJXJGu0AAACEiVAAAA=",
            "createdDateTime": "2019-08-01T07:06:27Z",
            "lastModifiedDateTime": "2019-08-01T07:06:28Z",
            "changeKey": "DAAAABYAAAA0RfLCCxWuR42wWzJXJGu0AAACEGHC",
            "categories": [],
            "receivedDateTime": "2019-08-01T07:06:28Z",
            "sentDateTime": "2019-08-01T07:06:24Z",
            "hasAttachments": false,
            "internetMessageId": "<BY5PR17MB38759D33B8925D525A476F33D9DE0@contoso.outlook.com>",
            "subject": "New Time Proposed: Let's go for lunch",
            "bodyPreview": "Can you make the next day instead?",
            "importance": "normal",
            "parentFolderId": "AQMkADAwQAAAIBDAAAAA==",
            "conversationId": "AAQkADAwQAQAMkh89RO3QpBiUCETTtVbIo=",
            "conversationIndex": "AdVINBlgySHz1E7dCkGJQIRNO1VsigAA4n6R",
            "isDeliveryReceiptRequested": null,
            "isReadReceiptRequested": false,
            "isRead": false,
            "isDraft": false,
            "webLink": "https://outlook.office365.com/owa/?ItemID=AAMkADAwJXJGu0AAACEiVAAAA%3D&exvsurl=1&viewmodel=ReadMessageItem",
            "inferenceClassification": "focused",
            "unsubscribeData": [],
            "unsubscribeEnabled": false,
            "meetingMessageType": "meetingTentativelyAccepted",
            "type": "singleInstance",
            "isOutOfDate": false,
            "isAllDay": false,
            "isDelegated": false,
            "responseType": "tentativelyAccepted",
            "recurrence": null,
            "body": {
                "contentType": "html",
                "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\nCan you make the next day instead?\r\n</body>\r\n</html>\r\n"
            },
            "sender": {
                "emailAddress": {
                    "name": "Adele Vance",
                    "address": "AdeleV@contoso.OnMicrosoft.com"
                }
            },
            "from": {
                "emailAddress": {
                    "name": "Adele Vance",
                    "address": "AdeleV@contoso.OnMicrosoft.com"
                }
            },
            "toRecipients": [
                {
                    "emailAddress": {
                        "name": "Alex Wilber",
                        "address": "AlexW@contoso.OnMicrosoft.com"
                    }
                }
            ],
            "ccRecipients": [],
            "bccRecipients": [],
            "replyTo": [],
            "flag": {
                "flagStatus": "notFlagged"
            },
            "startDateTime": {
                "dateTime": "2019-08-15T12:00:00.0000000",
                "timeZone": "Pacific Standard Time"
            },
            "endDateTime": {
                "dateTime": "2019-08-15T14:00:00.0000000",
                "timeZone": "Pacific Standard Time"
            },
            "location": {
                "displayName": "Harry's Bar",
                "locationType": "default",
                "uniqueIdType": "unknown"
            },
            "proposedNewTime": {
                "start": {
                    "dateTime": "2019-08-16T12:00:00", 
                    "timeZone": "Pacific Standard Time"
                },
                "end": {
                    "dateTime": "2019-08-16T14:00:00", 
                    "timeZone": "Pacific Standard Time"
                }
            }
         }
        ]
    }
    ```

4. Alex também observa que o **evento** do almoço agora inclui uma propriedade **proposedNewTime** que indica a proposta de Adele. Essa propriedade só estará presente como parte de uma instância [participante](/graph/api/resources/attendee?view=graph-rest-1.0) se o participante correspondente sugerir um horário de reunião alternativo. 

    <!-- {
      "blockType": "request",
      "name": "event_get"
    }-->
    ```http
    GET https://graph.microsoft.com/v1.0/me/events/AAMkADAwJXJGu0AAACEhWOAAA=?$select=subject,allowNewTimeProposals,start,end,attendees,organizer
    Prefer: outlook.timezone="Pacific Standard Time"
    ```

    <!-- {
      "blockType": "response",
      "name": "event_get",
      "truncated": true,
      "@odata.type": "microsoft.graph.event"
    } -->
    ```http
    HTTP/1.1 200 Ok

    {
        "@odata.context": "https://graph.microsoft.com/testexchangev1.0/$metadata#users('64339082-ed84-4b0b-b4ab-004ae54f3747')/events(subject,allowNewTimeProposals,start,end,attendees,organizer)/$entity",
        "@odata.etag": "W/\"NEXywgsVrkeNsFsyVyRrtAAAAhEDMA==\"",
        "id": "AAMkADAwJXJGu0AAACEhWOAAA=",
        "subject": "Let's go for lunch",
        "allowNewTimeProposals": true,
        "start": {
            "dateTime": "2019-08-15T12:00:00.0000000",
            "timeZone": "Pacific Standard Time"
        },
        "end": {
            "dateTime": "2019-08-15T14:00:00.0000000",
            "timeZone": "Pacific Standard Time"
        },
        "attendees": [
            {
                "type": "required",
                "status": {
                    "response": "tentativelyAccepted",
                    "time": "2019-08-01T07:06:24.5046431Z"
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
                "emailAddress": {
                    "name": "Adele Vance",
                    "address": "AdeleV@contoso.OnMicrosoft.com"
                }
            }
        ],
        "organizer": {
            "emailAddress": {
                "name": "Alex Wilber",
                "address": "AlexW@contoso.OnMicrosoft.com"
            }
        }
    }
    ```


5. Alex decide aceitar a proposta de Adele, atualizando o **evento** para a data/hora de **início** e **fim** que foi proposto.

    <!-- {
      "blockType": "request",
      "name": "event_update"
    }-->
    ```http
    PATCH https://graph.microsoft.com/v1.0/me/events/AAMkADAwJXJGu0AAACEhWOAAA=
    Prefer: outlook.timezone="Pacific Standard Time"
    Content-type: application/json

    {
        "start": {
            "dateTime": "2019-08-16T12:00:00.0000000",
            "timeZone": "Pacific Standard Time"
        },
        "end": {
            "dateTime": "2019-08-16T14:00:00.0000000",
            "timeZone": "Pacific Standard Time"
        }
    }
    ```

    A atualização de Alex é bem-sucedida e obtém a seguinte resposta.

    <!-- {
      "blockType": "response",
      "name": "event_update",
      "truncated": true,
      "@odata.type": "microsoft.graph.event"
    } -->
    ```http
    HTTP/1.1 200 Ok

    {
      "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('64339082-ed84-4b0b-b4ab-004ae54f3747')/events/$entity",
      "@odata.etag": "W/\"NEXywgsVrkeNsFsyVyRrtAAAAhBizA==\"",
      "id": "AAMkADAwJXJGu0AAACEhWOAAA=",
      "createdDateTime": "2019-08-01T06:41:07.805128Z",
      "lastModifiedDateTime": "2019-08-01T08:21:43.5696529Z",
      "changeKey": "NEXywgsVrkeNsFsyVyRrtAAAAhBizA==",
      "categories": [],
      "originalStartTimeZone": "Pacific Standard Time",
      "originalEndTimeZone": "Pacific Standard Time",
      "uid": "0400000082008A9979A0BD16",
      "reminderMinutesBeforeStart": 15,
      "isReminderOn": true,
      "hasAttachments": false,
      "subject": "Let's go for lunch",
      "bodyPreview": "Does noon work for you?",
      "importance": "normal",
      "sensitivity": "normal",
      "isAllDay": false,
      "isCancelled": false,
      "isOrganizer": true,
      "responseRequested": true,
      "seriesMasterId": null,
      "showAs": "busy",
      "type": "singleInstance",
      "webLink": "https://outlook.office365.com/owa/?itemid=AAMkADAwJXJGu0AAACEhWOAAA%3D&exvsurl=1&path=/calendar/item",
      "onlineMeetingUrl": null,
      "allowNewTimeProposals": true,
      "recurrence": null,
      "responseStatus": {
        "response": "organizer",
        "time": "0001-01-01T00:00:00Z"
      },
      "body": {
        "contentType": "html",
        "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\nDoes noon work for you?\r\n</body>\r\n</html>\r\n"
      },
      "start": {
        "dateTime": "2019-08-16T12:00:00.0000000",
        "timeZone": "Pacific Standard Time"
      },
      "end": {
        "dateTime": "2019-08-16T14:00:00.0000000",
        "timeZone": "Pacific Standard Time"
      },
      "location": {
        "displayName": "Harry's Bar",
        "locationType": "default",
        "uniqueId": "Harry's Bar",
        "uniqueIdType": "private"
      },
      "locations": [
        {
            "displayName": "Harry's Bar",
            "locationType": "default",
            "uniqueId": "Harry's Bar",
            "uniqueIdType": "private"
        }
      ],
      "attendees": [
        {
            "type": "required",
            "status": {
                "response": "notResponded",
                "time": "4501-01-01T00:00:00Z"
            },
            "emailAddress": {
                "name": "Adele Vance",
                "address": "AdeleV@contoso.OnMicrosoft.com"
            }
        }
      ],
      "organizer": {
        "emailAddress": {
            "name": "Alex Wilber",
            "address": "AlexW@contoso.OnMicrosoft.com"
        }
      }
    }
    ```


## <a name="no-attendee-proposes-alternative-time"></a>Nenhum participante propõe um horário alternativo

Na etapa 2, se Adele responder provisoriamente ou recusar e não propor uma data/hora diferente, acontecerá o seguinte:

- Na etapa 3, Alex receberia um **eventMessageResponse** com a propriedade **responseType** definida como `tentativelyAccepted` (ou `decline` se Adele recusasse). Alex não localizaria uma propriedade **proposedNewTime** nesta instância de **eventMessageResponse**.
- Na etapa 4, Alex também não localizaria uma propriedade **proposedNewTime** no **evento** associado.

## <a name="see-also"></a>Confira também
- [Encontrar possíveis horários de reunião no calendário do Outlook](findmeetingtimes-example.md)
- [Obter informações de disponibilidade de usuários e recursos](outlook-get-free-busy-schedule.md)
- [Agendar compromissos repetidos como eventos recorrentes no Outlook](outlook-schedule-recurring-events.md)
