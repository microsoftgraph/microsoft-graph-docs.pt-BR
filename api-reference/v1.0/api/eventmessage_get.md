# <a name="get-eventmessage"></a><span data-ttu-id="4aa4b-101">Obter eventMessage</span><span class="sxs-lookup"><span data-stu-id="4aa4b-101">Get eventMessage</span></span>

<span data-ttu-id="4aa4b-102">Obtenha as propriedades e os relacionamentos do objeto [eventMessage](../resources/eventmessage.md).</span><span class="sxs-lookup"><span data-stu-id="4aa4b-102">Get the properties and relationships of the [eventMessage](../resources/eventmessage.md) object.</span></span> <span data-ttu-id="4aa4b-103">Aplique o parâmetro $expand na propriedade de navegação **event** para obter o [event](../resources/event.md) correspondente no calendário de um participante.</span><span class="sxs-lookup"><span data-stu-id="4aa4b-103">Apply the $expand parameter on the **event** navigation property to get the associated [event](../resources/event.md) in an attendee's calendar.</span></span>

<span data-ttu-id="4aa4b-104">No momento, essa operação retorna corpos de mensagens de eventos somente no formato HTML.</span><span class="sxs-lookup"><span data-stu-id="4aa4b-104">Currently, this operation returns event message bodies in only HTML format.</span></span>

## <a name="permissions"></a><span data-ttu-id="4aa4b-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="4aa4b-105">Permissions</span></span>
<span data-ttu-id="4aa4b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="4aa4b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4aa4b-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4aa4b-108">Permission type</span></span>      | <span data-ttu-id="4aa4b-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4aa4b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4aa4b-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4aa4b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4aa4b-111">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="4aa4b-111">Mail.Read</span></span>    |
|<span data-ttu-id="4aa4b-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4aa4b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4aa4b-113">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="4aa4b-113">Mail.Read</span></span>    |
|<span data-ttu-id="4aa4b-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4aa4b-114">Application</span></span> | <span data-ttu-id="4aa4b-115">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="4aa4b-115">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="4aa4b-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4aa4b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}
GET /users/{id | userPrincipalName}/messages/{id}

GET /me/mailFolders/{id}/messages/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4aa4b-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="4aa4b-117">Optional query parameters</span></span>
<span data-ttu-id="4aa4b-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="4aa4b-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="4aa4b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4aa4b-119">Request headers</span></span>
| <span data-ttu-id="4aa4b-120">Nome</span><span class="sxs-lookup"><span data-stu-id="4aa4b-120">Name</span></span>       | <span data-ttu-id="4aa4b-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="4aa4b-121">Type</span></span> | <span data-ttu-id="4aa4b-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="4aa4b-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="4aa4b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4aa4b-123">Authorization</span></span>  | <span data-ttu-id="4aa4b-124">string</span><span class="sxs-lookup"><span data-stu-id="4aa4b-124">string</span></span>  | <span data-ttu-id="4aa4b-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4aa4b-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4aa4b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4aa4b-127">Request body</span></span>
<span data-ttu-id="4aa4b-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4aa4b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4aa4b-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="4aa4b-129">Response</span></span>

<span data-ttu-id="4aa4b-130">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [eventMessage](../resources/eventmessage.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4aa4b-130">If successful, this method returns a `200 OK` response code and [eventMessage](../resources/eventmessage.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4aa4b-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4aa4b-131">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="4aa4b-132">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="4aa4b-132">Request 1</span></span>
<span data-ttu-id="4aa4b-133">O primeiro exemplo mostra como obter as propriedades de uma mensagem de evento com base no ID da mensagem do evento.</span><span class="sxs-lookup"><span data-stu-id="4aa4b-133">The first example shows how to get the properties of an event message based on the event message ID.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADYAAAImV_lAAA="],
  "name": "get_eventmessage"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/AAMkADYAAAImV_lAAA=
```
##### <a name="response-1"></a><span data-ttu-id="4aa4b-134">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="4aa4b-134">Response 1</span></span>
<span data-ttu-id="4aa4b-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4aa4b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "get_eventmessage",
  "truncated": true,
  "@odata.type": "microsoft.graph.eventMessage"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('8fd6e83b-3cc0-4bf0-8b26-950f4d7110f6')/messages/$entity",
    "@odata.type":"#microsoft.graph.eventMessage",
    "@odata.etag":"W/\"CwAAABYAAABXlB/SL0N4Q6g6o+jSYAEuAAAImkVD\"",
    "id":"AAMkADYAAAImV_lAAA=",
    "createdDateTime":"2017-12-27T21:58:36Z",
    "lastModifiedDateTime":"2017-12-27T23:26:38Z",
    "changeKey":"CwAAABYAAABXlB/SL0N4Q6g6o+jSYAEuAAAImkVD",
    "categories":[

    ],
    "receivedDateTime":"2017-12-27T21:58:36Z",
    "sentDateTime":"2017-12-27T21:58:36Z",
    "hasAttachments":false,
    "internetMessageId":"<MWHPR1301MB2110DCFC@MWHPR1301MB2110.namprd13.prod.outlook.com>",
    "subject":"Debrief from meetup",
    "bodyPreview":"Let's debrief after community meetup.",
    "importance":"normal",
    "parentFolderId":"AQMkADYAAAIBDAAAAA==",
    "conversationId":"AAQkADYCipTiRjXQORU=",
    "isDeliveryReceiptRequested":null,
    "isReadReceiptRequested":false,
    "isRead":false,
    "isDraft":false,
    "webLink":"https://outlook.office365.com/owa/?ItemID=AAMkADYAAAImV%2BlAAA%3D&exvsurl=1&viewmodel=ReadMessageItem",
    "inferenceClassification":"focused",
    "meetingMessageType":"meetingRequest",
    "body":{
        "contentType":"html",
        "content":"<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n<style type=\"text/css\" style=\"display:none\">\r\n<!--\r\np\r\n\t{margin-top:0;\r\n\tmargin-bottom:0}\r\n-->\r\n</style>\r\n</head>\r\n<body dir=\"ltr\">\r\n<div id=\"divtagdefaultwrapper\" dir=\"ltr\" style=\"font-size:12pt; color:#000000; font-family:Calibri,Helvetica,sans-serif\">\r\n<p style=\"margin-top:0; margin-bottom:0\">Let's debrief after community meetup.<br>\r\n</p>\r\n</div>\r\n</body>\r\n</html>\r\n"
    },
    "sender":{
        "emailAddress":{
            "name":"Administrator",
            "address":"admin@contoso.onmicrosoft.com"
        }
    },
    "from":{
        "emailAddress":{
            "name":"Administrator",
            "address":"admin@contoso.onmicrosoft.com"
        }
    },
    "toRecipients":[
        {
            "emailAddress":{
                "name":"Alex Wilber",
                "address":"AlexW@contoso.onmicrosoft.com"
            }
        }
    ],
    "ccRecipients":[

    ],
    "bccRecipients":[

    ],
    "replyTo":[

    ]
}
```

##### <a name="request-2"></a><span data-ttu-id="4aa4b-138">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="4aa4b-138">Request 2</span></span>
<span data-ttu-id="4aa4b-139">O segundo exemplo mostra como obter o evento associado a uma mensagem de evento.</span><span class="sxs-lookup"><span data-stu-id="4aa4b-139">The second example shows how to get the event associated with an event message.</span></span> <span data-ttu-id="4aa4b-140">Ele usa a ID da mensagem para obter a mensagem do evento, fornece explicitamente uma conversão na mensagem do evento para acessar a propriedade de navegação **event** e aplica um parâmetro $expand para obter as propriedades do evento.</span><span class="sxs-lookup"><span data-stu-id="4aa4b-140">It uses the event message ID to get the event message, explicitly provides a cast on the event message to access its **event** navigation property, and apply an $expand parameter to get the properties of the event.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADYAAAImV_jAAA="],
  "name": "get_event_based_on_eventmessage"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/AAMkADYAAAImV_jAAA=?$expand=microsoft.graph.eventMessage/event
```
##### <a name="response-2"></a><span data-ttu-id="4aa4b-141">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="4aa4b-141">Response 2</span></span>
<span data-ttu-id="4aa4b-142">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4aa4b-142">Here is an example of the response.</span></span> <span data-ttu-id="4aa4b-143">As propriedades do evento correspondente são retornadas na resposta.</span><span class="sxs-lookup"><span data-stu-id="4aa4b-143">The properties of the associated event are returned in the response.</span></span> <span data-ttu-id="4aa4b-144">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="4aa4b-144">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="4aa4b-145">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4aa4b-145">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "get_event_based_on_eventmessage",
  "truncated": true,
  "@odata.type": "microsoft.graph.eventMessage"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
   "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('8fd6e83b-3cc0-4bf0-8b26-950f4d7110f6')/messages/$entity",
   "@odata.type":"#microsoft.graph.eventMessage",
   "@odata.etag":"W/\"CwAAABYAAABXlB/SL0N4Q6g6o+jSYAEuAAAImkVF\"",
   "id":"AAMkADYAAAImV_jAAA=",
   "createdDateTime":"2017-12-27T21:54:55Z",
   "lastModifiedDateTime":"2017-12-27T23:26:38Z",
   "changeKey":"CwAAABYAAABXlB/SL0N4Q6g6o+jSYAEuAAAImkVF",
   "categories":[

   ],
   "receivedDateTime":"2017-12-27T21:54:55Z",
   "sentDateTime":"2017-12-27T21:54:54Z",
   "hasAttachments":false,
   "internetMessageId":"<MWHPR1301MB211042CF@MWHPR1301MB2110.namprd13.prod.outlook.com>",
   "subject":"Kick off planning",
   "bodyPreview":"Let's collect opinions from our teams and organize action items.",
   "importance":"normal",
    "parentFolderId":"AQMkADYAS4AAAIBDAAAAA==",
    "conversationId":"AAQkADYRuffB3wDlPn-ReFZarI60=",
   "isDeliveryReceiptRequested":null,
   "isReadReceiptRequested":false,
   "isRead":false,
   "isDraft":false,
   "webLink":"https://outlook.office365.com/owa/?ItemID=AAMkADYAAAImV%2BjAAA%3D&exvsurl=1&viewmodel=ReadMessageItem",
   "inferenceClassification":"focused",
   "meetingMessageType":"meetingRequest",
   "body":{
      "contentType":"html",
      "content":"<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n<style type=\"text/css\" style=\"display:none\">\r\n<!--\r\np\r\n\t{margin-top:0;\r\n\tmargin-bottom:0}\r\n-->\r\n</style>\r\n</head>\r\n<body dir=\"ltr\">\r\n<div id=\"divtagdefaultwrapper\" dir=\"ltr\" style=\"font-size:12pt; color:#000000; font-family:Calibri,Helvetica,sans-serif\">\r\n<p style=\"margin-top:0; margin-bottom:0\">Let's collect opinions from our teams and organize action items.<br>\r\n</p>\r\n</div>\r\n</body>\r\n</html>\r\n"
   },
   "sender":{
      "emailAddress":{
         "name":"Administrator",
         "address":"admin@contoso.onmicrosoft.com"
      }
   },
   "from":{
      "emailAddress":{
         "name":"Administrator",
         "address":"admin@contoso.onmicrosoft.com"
      }
   },
   "toRecipients":[
      {
         "emailAddress":{
            "name":"Alex Wilber",
            "address":"AlexW@contoso.onmicrosoft.com"
         }
      }
   ],
   "ccRecipients":[

   ],
   "bccRecipients":[

   ],
   "replyTo":[

   ],
   "event@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('8fd6e83b-3cc0-4bf0-8b26-950f4d7110f6')/messages('AAMkADYAAAImV_jAAA%3D')/microsoft.graph.eventMessage/event/$entity",
   "event":{
      "@odata.etag":"W/\"V5Qf0i9DeEOoOqPo0mABLgAACJpBWg==\"",
      "id":"AAMkADYAAAImVu6AAA=",
      "createdDateTime":"2017-12-27T21:54:55.2624551Z",
      "lastModifiedDateTime":"2017-12-27T22:19:16.6667889Z",
      "changeKey":"V5Qf0i9DeEOoOqPo0mABLgAACJpBWg==",
      "categories":[

      ],
      "originalStartTimeZone":"Pacific Standard Time",
      "originalEndTimeZone":"Pacific Standard Time",
      "iCalUId":"040000008200E00074C5B7101A82E00800000000A2A6F3535D7FD3010000000000000000100000003D770E2E8974F44B9471BDB348097FE3",
      "reminderMinutesBeforeStart":15,
      "isReminderOn":true,
      "hasAttachments":false,
      "subject":"Kick off planning",
      "bodyPreview":"Let's collect opinions from our teams and organize action items.",
      "importance":"normal",
      "sensitivity":"normal",
      "isAllDay":false,
      "isCancelled":false,
      "isOrganizer":false,
      "responseRequested":true,
      "seriesMasterId":null,
      "showAs":"tentative",
      "type":"singleInstance",
      "webLink":"https://outlook.office365.com/owa/?itemid=AAMkADYAAAImVu6AAA%3D&exvsurl=1&path=/calendar/item",
      "onlineMeetingUrl":null,
      "responseStatus":{
         "response":"tentativelyAccepted",
         "time":"2017-12-27T22:19:12.6197462Z"
      },
      "body":{
         "contentType":"html",
         "content":"<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n<style type=\"text/css\" style=\"display:none\">\r\n<!--\r\np\r\n\t{margin-top:0;\r\n\tmargin-bottom:0}\r\n-->\r\n</style>\r\n</head>\r\n<body dir=\"ltr\">\r\n<div id=\"divtagdefaultwrapper\" dir=\"ltr\" style=\"font-size:12pt; color:#000000; font-family:Calibri,Helvetica,sans-serif\">\r\n<p style=\"margin-top:0; margin-bottom:0\">Let's collect opinions from our teams and organize action items.<br>\r\n</p>\r\n</div>\r\n</body>\r\n</html>\r\n"
      },
      "start":{
         "dateTime":"2018-02-02T22:00:00.0000000",
         "timeZone":"UTC"
      },
      "end":{
         "dateTime":"2018-02-02T23:00:00.0000000",
         "timeZone":"UTC"
      },
      "location":{
         "displayName":"Mt. Hood"
      },
      "recurrence":null,
      "attendees":[
         {
            "type":"required",
            "status":{
               "response":"none",
               "time":"0001-01-01T00:00:00Z"
            },
            "emailAddress":{
               "name":"Administrator",
               "address":"admin@contoso.onmicrosoft.com"
            }
         },
         {
            "type":"required",
            "status":{
               "response":"tentativelyAccepted",
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
            "name":"Administrator",
            "address":"admin@contoso.onmicrosoft.com"
         }
      }
   }
}
``` 

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get eventMessage",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
