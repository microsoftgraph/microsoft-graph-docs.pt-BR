---
title: Obter eventMessage
description: Expanda ' parâmetro no **evento**
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: ffa2524939e5866bc74d255606a7a28297d691d2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32463991"
---
# <a name="get-eventmessage"></a><span data-ttu-id="6d8a2-103">Obter eventMessage</span><span class="sxs-lookup"><span data-stu-id="6d8a2-103">Get eventMessage</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6d8a2-104">Obtenha as propriedades e os relacionamentos do objeto [eventMessage](../resources/eventmessage.md).</span><span class="sxs-lookup"><span data-stu-id="6d8a2-104">Get the properties and relationships of the [eventMessage](../resources/eventmessage.md) object.</span></span> <span data-ttu-id="6d8a2-105">Aplique o `$expand` parâmetro na propriedade de navegação de **evento** para obter o [evento](../resources/event.md) associado no calendário de um participante.</span><span class="sxs-lookup"><span data-stu-id="6d8a2-105">Apply the `$expand` parameter on the **event** navigation property to get the associated [event](../resources/event.md) in an attendee's calendar.</span></span>

### <a name="get-the-event-message-body-in-html-or-text-format"></a><span data-ttu-id="6d8a2-106">Obter o corpo da mensagem de evento no formato HTML ou de texto</span><span class="sxs-lookup"><span data-stu-id="6d8a2-106">Get the event message body in HTML or text format</span></span>

<span data-ttu-id="6d8a2-107">Os corpos de mensagens de evento podem estar no formato HTML ou de texto.</span><span class="sxs-lookup"><span data-stu-id="6d8a2-107">Event message bodies can be in HTML or text format.</span></span>

<span data-ttu-id="6d8a2-108">Você pode usar o `Prefer: outlook.body-content-type` cabeçalho para especificar o formato desejado retornado nas propriedades **Body** e **uniqueBody** em uma `GET` solicitação:</span><span class="sxs-lookup"><span data-stu-id="6d8a2-108">You can use the `Prefer: outlook.body-content-type` header to specify the desired format returned in the **body** and **uniqueBody** properties in a `GET` request:</span></span>

- <span data-ttu-id="6d8a2-109">Especifique `Prefer: outlook.body-content-type="text"` para obter um corpo de mensagem de evento retornado no formato de texto.</span><span class="sxs-lookup"><span data-stu-id="6d8a2-109">Specify `Prefer: outlook.body-content-type="text"` to get a event message body returned in text format.</span></span>
- <span data-ttu-id="6d8a2-110">Especifique `Prefer: outlook.body-content-type="html"`ou apenas pule o cabeçalho para retornar o corpo da mensagem de evento no formato HTML.</span><span class="sxs-lookup"><span data-stu-id="6d8a2-110">Specify `Prefer: outlook.body-content-type="html"`, or just skip the header, to return the event message body in HTML format.</span></span>

<span data-ttu-id="6d8a2-111">Se você especificar um dos cabeçalhos, a resposta incluirá o cabeçalho `Preference-Applied` correspondente como confirmação:</span><span class="sxs-lookup"><span data-stu-id="6d8a2-111">If you specify either header, the response will include the corresponding `Preference-Applied` header as confirmation:</span></span>

- <span data-ttu-id="6d8a2-112">Para solicitações de formato de texto: `Preference-Applied: outlook.body-content-type="text"`</span><span class="sxs-lookup"><span data-stu-id="6d8a2-112">For text format requests: `Preference-Applied: outlook.body-content-type="text"`</span></span>
- <span data-ttu-id="6d8a2-113">Para solicitações de formato HTML: `Preference-Applied: outlook.body-content-type="html"`</span><span class="sxs-lookup"><span data-stu-id="6d8a2-113">For HTML format requests: `Preference-Applied: outlook.body-content-type="html"`</span></span>

## <a name="permissions"></a><span data-ttu-id="6d8a2-114">Permissões</span><span class="sxs-lookup"><span data-stu-id="6d8a2-114">Permissions</span></span>
<span data-ttu-id="6d8a2-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6d8a2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6d8a2-117">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6d8a2-117">Permission type</span></span>      | <span data-ttu-id="6d8a2-118">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6d8a2-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6d8a2-119">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6d8a2-119">Delegated (work or school account)</span></span> | <span data-ttu-id="6d8a2-120">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="6d8a2-120">Mail.Read</span></span>    |
|<span data-ttu-id="6d8a2-121">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6d8a2-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6d8a2-122">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="6d8a2-122">Mail.Read</span></span>    |
|<span data-ttu-id="6d8a2-123">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6d8a2-123">Application</span></span> | <span data-ttu-id="6d8a2-124">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="6d8a2-124">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="6d8a2-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6d8a2-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}
GET /users/{id | userPrincipalName}/messages/{id}

GET /me/mailFolders/{id}/messages/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6d8a2-126">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6d8a2-126">Optional query parameters</span></span>
<span data-ttu-id="6d8a2-127">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6d8a2-127">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="6d8a2-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6d8a2-128">Request headers</span></span>
| <span data-ttu-id="6d8a2-129">Nome</span><span class="sxs-lookup"><span data-stu-id="6d8a2-129">Name</span></span>       | <span data-ttu-id="6d8a2-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="6d8a2-130">Type</span></span> | <span data-ttu-id="6d8a2-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="6d8a2-131">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="6d8a2-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="6d8a2-132">Authorization</span></span>  | <span data-ttu-id="6d8a2-133">string</span><span class="sxs-lookup"><span data-stu-id="6d8a2-133">string</span></span>  | <span data-ttu-id="6d8a2-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6d8a2-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6d8a2-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6d8a2-136">Request body</span></span>
<span data-ttu-id="6d8a2-137">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6d8a2-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6d8a2-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="6d8a2-138">Response</span></span>

<span data-ttu-id="6d8a2-139">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [eventMessage](../resources/eventmessage.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6d8a2-139">If successful, this method returns a `200 OK` response code and [eventMessage](../resources/eventmessage.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6d8a2-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6d8a2-140">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="6d8a2-141">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="6d8a2-141">Request 1</span></span>
<span data-ttu-id="6d8a2-142">O primeiro exemplo mostra como obter as propriedades de uma mensagem de evento com base no ID da mensagem do evento.</span><span class="sxs-lookup"><span data-stu-id="6d8a2-142">The first example shows how to get the properties of an event message based on the event message ID.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_eventmessage"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages('AAMkADYAAAImV_lAAA=')
```
##### <a name="response-1"></a><span data-ttu-id="6d8a2-143">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="6d8a2-143">Response 1</span></span>
<span data-ttu-id="6d8a2-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6d8a2-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "get_eventmessage",
  "truncated": true,
  "@odata.type": "microsoft.graph.eventMessageRequest"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('8fd6e83b-3cc0-4bf0-8b26-950f4d7110f6')/messages/$entity",
    "@odata.type":"#microsoft.graph.eventMessageRequest",
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
    "conversationIndex":"AdN/Xdgnql4N9FlrT0KKlOJGNdA5FQ==",
    "isDeliveryReceiptRequested":null,
    "isReadReceiptRequested":false,
    "isRead":false,
    "isDraft":false,
    "webLink":"https://outlook.office365.com/owa/?ItemID=AAMkADYAAAImV%2BlAAA%3D&exvsurl=1&viewmodel=ReadMessageItem",
    "inferenceClassification":"focused",
    "unsubscribeData":[

    ],
    "unsubscribeEnabled":false,
    "meetingMessageType":"meetingRequest",
    "type":"singleInstance",
    "isOutOfDate":false,
    "isAllDay":false,
    "isDelegated":false,
    "responseRequested":true,
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

    ],
    "mentionsPreview":null,
    "flag":{
        "flagStatus":"notFlagged"
    },
    "startDateTime":{
        "dateTime":"2018-02-19T19:00:00.0000000",
        "timeZone":"UTC"
    },
    "endDateTime":{
        "dateTime":"2018-02-19T19:30:00.0000000",
        "timeZone":"UTC"
    },
    "location":{
        "displayName":"Mt. Hood",
        "locationType":"default",
        "uniqueIdType":"unknown"
    },
    "recurrence":null,
    "previousLocation":null,
    "previousStartDateTime":null,
    "previousEndDateTime":null
}
```


##### <a name="request-2"></a><span data-ttu-id="6d8a2-147">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="6d8a2-147">Request 2</span></span>
<span data-ttu-id="6d8a2-148">O segundo exemplo mostra como obter o evento associado a uma mensagem de evento.</span><span class="sxs-lookup"><span data-stu-id="6d8a2-148">The second example shows how to get the event associated with an event message.</span></span> <span data-ttu-id="6d8a2-149">Ele usa a ID da mensagem para obter a mensagem do evento, fornece explicitamente uma conversão na mensagem do evento para acessar a propriedade de navegação **event** e aplica um parâmetro $expand para obter as propriedades do evento.</span><span class="sxs-lookup"><span data-stu-id="6d8a2-149">It uses the event message ID to get the event message, explicitly provides a cast on the event message to access its **event** navigation property, and apply an $expand parameter to get the properties of the event.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_event_based_on_eventmessage"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages('AAMkADYAAAImV_jAAA=')?$expand=microsoft.graph.eventMessage/event
```
##### <a name="response-2"></a><span data-ttu-id="6d8a2-150">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="6d8a2-150">Response 2</span></span>
<span data-ttu-id="6d8a2-151">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6d8a2-151">Here is an example of the response.</span></span> <span data-ttu-id="6d8a2-152">As propriedades do evento correspondente são retornadas na resposta.</span><span class="sxs-lookup"><span data-stu-id="6d8a2-152">The properties of the associated event are returned in the response.</span></span>
<span data-ttu-id="6d8a2-153">Observação: o objeto de resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="6d8a2-153">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="6d8a2-154">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6d8a2-154">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "get_event_based_on_eventmessage",
  "truncated": true,
  "@odata.type": "microsoft.graph.eventMessageRequest"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('8fd6e83b-3cc0-4bf0-8b26-950f4d7110f6')/messages/$entity",
    "@odata.type":"#microsoft.graph.eventMessageRequest",
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
    "internetMessageId":"<MWHPR1301MB211042CFBF@MWHPR1301MB2110.namprd13.prod.outlook.com>",
    "subject":"Kick off planning",
    "bodyPreview":"Let's collect opinions from our teams and organize action items.",
    "importance":"normal",
    "parentFolderId":"AQMkADYAS4AAAIBDAAAAA==",
    "conversationId":"AAQkADYRuffB3wDlPn-ReFZarI60=",
    "conversationIndex":"AdN/XVP4JG598HfAOU+f9F4VlqsjrQ==",
    "isDeliveryReceiptRequested":null,
    "isReadReceiptRequested":false,
    "isRead":false,
    "isDraft":false,
    "webLink":"https://outlook.office365.com/owa/?ItemID=AAMkADYAAAImV%2BjAAA%3D&exvsurl=1&viewmodel=ReadMessageItem",
    "inferenceClassification":"focused",
    "unsubscribeData":[

    ],
    "unsubscribeEnabled":false,
    "meetingMessageType":"meetingRequest",
    "type":"singleInstance",
    "isOutOfDate":false,
    "isAllDay":false,
    "isDelegated":false,
    "responseRequested":true,
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
    "mentionsPreview":null,
    "flag":{
        "flagStatus":"notFlagged"
    },
    "startDateTime":{
        "dateTime":"2018-02-02T22:00:00.0000000",
        "timeZone":"UTC"
    },
    "endDateTime":{
        "dateTime":"2018-02-02T23:00:00.0000000",
        "timeZone":"UTC"
    },
    "location":{
        "displayName":"Mt. Hood",
        "locationType":"default",
        "uniqueIdType":"unknown"
    },
    "recurrence":null,
    "previousLocation":null,
    "previousStartDateTime":null,
    "previousEndDateTime":null,
    "event@odata.context":"https://graph.microsoft.com/beta/$metadata#users('8fd6e83b-3cc0-4bf0-8b26-950f4d7110f6')/messages('AAMkADYAAAImV_jAAA%3D')/microsoft.graph.eventMessage/event/$entity",
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
        "uid":"040000008200E00074C5B7101A82E00800000000A2A6F3535D7FD3010000000000000000100000003D770E2E8974F44B9471BDB348097FE3",
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
            "displayName":"Mt. Hood",
            "locationType":"default",
            "uniqueId":"Mt. Hood",
            "uniqueIdType":"private"
        },
        "locations":[
            {
                "displayName":"Mt. Hood",
                "locationType":"default",
                "uniqueId":"Mt. Hood",
                "uniqueIdType":"private"
            }
        ],
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
        },
        "OnlineMeeting":null
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get eventMessage",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/eventmessage-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
