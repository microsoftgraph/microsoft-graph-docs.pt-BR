---
title: Obter eventMessage
description: Expanda ' parâmetro no **evento**
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 96df7d14adf4b5d2d46c559d31dcd935db29a070
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27922302"
---
# <a name="get-eventmessage"></a><span data-ttu-id="a7623-103">Obter eventMessage</span><span class="sxs-lookup"><span data-stu-id="a7623-103">Get eventMessage</span></span>

> <span data-ttu-id="a7623-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a7623-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a7623-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a7623-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a7623-106">Obtenha as propriedades e os relacionamentos do objeto [eventMessage](../resources/eventmessage.md).</span><span class="sxs-lookup"><span data-stu-id="a7623-106">Get the properties and relationships of the [eventMessage](../resources/eventmessage.md) object.</span></span> <span data-ttu-id="a7623-107">Aplicar o `$expand` parâmetro sobre a propriedade de navegação de **evento** para obter o [evento](../resources/event.md) de associado no calendário do participante.</span><span class="sxs-lookup"><span data-stu-id="a7623-107">Apply the `$expand` parameter on the **event** navigation property to get the associated [event](../resources/event.md) in an attendee's calendar.</span></span>

### <a name="get-the-event-message-body-in-html-or-text-format"></a><span data-ttu-id="a7623-108">Obtenha o corpo da mensagem de evento no formato HTML ou texto</span><span class="sxs-lookup"><span data-stu-id="a7623-108">Get the event message body in HTML or text format</span></span>

<span data-ttu-id="a7623-109">Corpos de mensagem de evento podem ser no formato HTML ou texto.</span><span class="sxs-lookup"><span data-stu-id="a7623-109">Event message bodies can be in HTML or text format.</span></span>

<span data-ttu-id="a7623-110">Você pode usar o `Prefer: outlook.body-content-type` cabeçalho para especificar o formato desejado retornado nas propriedades do **corpo** e **uniqueBody** em um `GET` solicitação:</span><span class="sxs-lookup"><span data-stu-id="a7623-110">You can use the `Prefer: outlook.body-content-type` header to specify the desired format returned in the **body** and **uniqueBody** properties in a `GET` request:</span></span>

- <span data-ttu-id="a7623-111">Especificar `Prefer: outlook.body-content-type="text"` para obter o corpo de uma mensagem de evento retornado em formato de texto.</span><span class="sxs-lookup"><span data-stu-id="a7623-111">Specify `Prefer: outlook.body-content-type="text"` to get a event message body returned in text format.</span></span>
- <span data-ttu-id="a7623-112">Especificar `Prefer: outlook.body-content-type="html"`, ou simplesmente ignore o cabeçalho, para retornar o corpo da mensagem de evento no formato HTML.</span><span class="sxs-lookup"><span data-stu-id="a7623-112">Specify `Prefer: outlook.body-content-type="html"`, or just skip the header, to return the event message body in HTML format.</span></span>

<span data-ttu-id="a7623-113">Se você especificar um dos cabeçalhos, a resposta incluirá o cabeçalho `Preference-Applied` correspondente como confirmação:</span><span class="sxs-lookup"><span data-stu-id="a7623-113">If you specify either header, the response will include the corresponding `Preference-Applied` header as confirmation:</span></span>

- <span data-ttu-id="a7623-114">Para solicitações de formato de texto: `Preference-Applied: outlook.body-content-type="text"`</span><span class="sxs-lookup"><span data-stu-id="a7623-114">For text format requests: `Preference-Applied: outlook.body-content-type="text"`</span></span>
- <span data-ttu-id="a7623-115">Para solicitações de formato HTML: `Preference-Applied: outlook.body-content-type="html"`</span><span class="sxs-lookup"><span data-stu-id="a7623-115">For HTML format requests: `Preference-Applied: outlook.body-content-type="html"`</span></span>

## <a name="permissions"></a><span data-ttu-id="a7623-116">Permissions</span><span class="sxs-lookup"><span data-stu-id="a7623-116">Permissions</span></span>
<span data-ttu-id="a7623-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a7623-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a7623-119">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a7623-119">Permission type</span></span>      | <span data-ttu-id="a7623-120">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a7623-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a7623-121">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a7623-121">Delegated (work or school account)</span></span> | <span data-ttu-id="a7623-122">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="a7623-122">Mail.Read</span></span>    |
|<span data-ttu-id="a7623-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a7623-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a7623-124">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="a7623-124">Mail.Read</span></span>    |
|<span data-ttu-id="a7623-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a7623-125">Application</span></span> | <span data-ttu-id="a7623-126">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="a7623-126">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="a7623-127">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a7623-127">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}
GET /users/{id | userPrincipalName}/messages/{id}

GET /me/mailFolders/{id}/messages/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a7623-128">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a7623-128">Optional query parameters</span></span>
<span data-ttu-id="a7623-129">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a7623-129">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="a7623-130">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a7623-130">Request headers</span></span>
| <span data-ttu-id="a7623-131">Nome</span><span class="sxs-lookup"><span data-stu-id="a7623-131">Name</span></span>       | <span data-ttu-id="a7623-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="a7623-132">Type</span></span> | <span data-ttu-id="a7623-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="a7623-133">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a7623-134">Autorização</span><span class="sxs-lookup"><span data-stu-id="a7623-134">Authorization</span></span>  | <span data-ttu-id="a7623-135">string</span><span class="sxs-lookup"><span data-stu-id="a7623-135">string</span></span>  | <span data-ttu-id="a7623-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a7623-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a7623-138">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a7623-138">Request body</span></span>
<span data-ttu-id="a7623-139">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a7623-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a7623-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="a7623-140">Response</span></span>

<span data-ttu-id="a7623-141">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [eventMessage](../resources/eventmessage.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a7623-141">If successful, this method returns a `200 OK` response code and [eventMessage](../resources/eventmessage.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a7623-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a7623-142">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="a7623-143">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="a7623-143">Request 1</span></span>
<span data-ttu-id="a7623-144">O primeiro exemplo mostra como obter as propriedades de uma mensagem de evento com base no ID da mensagem do evento.</span><span class="sxs-lookup"><span data-stu-id="a7623-144">The first example shows how to get the properties of an event message based on the event message ID.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_eventmessage"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages('AAMkADYAAAImV_lAAA=')
```
##### <a name="response-1"></a><span data-ttu-id="a7623-145">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="a7623-145">Response 1</span></span>
<span data-ttu-id="a7623-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a7623-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


##### <a name="request-2"></a><span data-ttu-id="a7623-149">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="a7623-149">Request 2</span></span>
<span data-ttu-id="a7623-150">O segundo exemplo mostra como obter o evento associado a uma mensagem de evento.</span><span class="sxs-lookup"><span data-stu-id="a7623-150">The second example shows how to get the event associated with an event message.</span></span> <span data-ttu-id="a7623-151">Ele usa a ID da mensagem para obter a mensagem do evento, fornece explicitamente uma conversão na mensagem do evento para acessar a propriedade de navegação **event** e aplica um parâmetro $expand para obter as propriedades do evento.</span><span class="sxs-lookup"><span data-stu-id="a7623-151">It uses the event message ID to get the event message, explicitly provides a cast on the event message to access its **event** navigation property, and apply an $expand parameter to get the properties of the event.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_event_based_on_eventmessage"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages('AAMkADYAAAImV_jAAA=')?$expand=microsoft.graph.eventMessage/event
```
##### <a name="response-2"></a><span data-ttu-id="a7623-152">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="a7623-152">Response 2</span></span>
<span data-ttu-id="a7623-153">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a7623-153">Here is an example of the response.</span></span> <span data-ttu-id="a7623-154">As propriedades do evento correspondente são retornadas na resposta.</span><span class="sxs-lookup"><span data-stu-id="a7623-154">The properties of the associated event are returned in the response.</span></span>
<span data-ttu-id="a7623-155">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="a7623-155">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="a7623-156">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a7623-156">All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Get eventMessage",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
