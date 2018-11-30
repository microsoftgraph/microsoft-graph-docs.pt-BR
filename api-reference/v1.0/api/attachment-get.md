---
title: Obter anexo
description: 'Ler as propriedades e relacionamentos de um anexo, anexados a um evento, '
ms.openlocfilehash: 7405078f2c6408053e499a5fbb6aaac02f87f440
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27007399"
---
# <a name="get-attachment"></a><span data-ttu-id="98fa4-103">Obter anexo</span><span class="sxs-lookup"><span data-stu-id="98fa4-103">Get attachment</span></span>

<span data-ttu-id="98fa4-104">Leia as propriedades e as relações de um anexo, anexado a um [event](../resources/event.md), [message](../resources/message.md) ou [post](../resources/post.md).</span><span class="sxs-lookup"><span data-stu-id="98fa4-104">Read the properties and relationships of an attachment, attached to an [event](../resources/event.md), [message](../resources/message.md), or [post](../resources/post.md).</span></span> 

<span data-ttu-id="98fa4-105">Um anexo pode ser de um dos seguintes tipos:</span><span class="sxs-lookup"><span data-stu-id="98fa4-105">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="98fa4-106">Um arquivo (recurso [fileAttachment](../resources/fileattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="98fa4-106">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="98fa4-p101">Um item (contato, evento ou mensagem, representado por um recurso [itemAttachment](../resources/itemattachment.md)). Você pode usar `$expand` para obter ainda mais as propriedades desse item. Veja um [exemplo](#request-2) abaixo.</span><span class="sxs-lookup"><span data-stu-id="98fa4-p101">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource). You can use `$expand` to further get the properties of that item. See an [example](#request-2) below.</span></span>
* <span data-ttu-id="98fa4-110">Um link para um arquivo (recurso [referenceAttachment](../resources/referenceattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="98fa4-110">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource).</span></span>

<span data-ttu-id="98fa4-111">Todos esses tipos de recursos de anexo são derivados do recurso [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="98fa4-111">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span> 


## <a name="permissions"></a><span data-ttu-id="98fa4-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="98fa4-112">Permissions</span></span>
<span data-ttu-id="98fa4-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="98fa4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="98fa4-115">Se estiver acessando anexos em mensagens: Mail.Read.</span><span class="sxs-lookup"><span data-stu-id="98fa4-115">If accessing attachments in messages: Mail.Read.</span></span>
* <span data-ttu-id="98fa4-116">Se estiver acessando anexos em eventos: Calendars.Read.</span><span class="sxs-lookup"><span data-stu-id="98fa4-116">If accessing attachments in events: Calendars.Read.</span></span>
* <span data-ttu-id="98fa4-117">Se acessando anexos em postagens de grupo: Group.Read.All.</span><span class="sxs-lookup"><span data-stu-id="98fa4-117">If accessing attachments in group posts: Group.Read.All.</span></span>

<!--
* If accessing attachments in group events or posts: Group.Read.All.
-->

## <a name="http-request"></a><span data-ttu-id="98fa4-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="98fa4-118">HTTP request</span></span>
<span data-ttu-id="98fa4-119">Anexos em um [evento](../resources/event.md) do usuário padrão [calendário](../resources/calendar.md).</span><span class="sxs-lookup"><span data-stu-id="98fa4-119">Attachments for an [event](../resources/event.md) in the user's default [calendar](../resources/calendar.md).</span></span>

<!--
Attachments for an [event](../resources/event.md) in the user's or group's default [calendar](../resources/calendar.md).
-->
<!-- { "blockType": "ignored" } -->
```http
GET /me/events/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/events/{id}/attachments/{id}

GET /me/calendar/{id}/events/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/calendar/events/{id}/attachments/{id}
```

<!--
GET /groups/{id}/events/{id}/attachments/{id}
GET /groups/{id}/calendar/events/{id}/attachments/{id}
-->

<span data-ttu-id="98fa4-120">Anexos de um [event](../resources/event.md) em um [calendar](../resources/calendar.md) que pertence ao [calendarGroup](../resources/calendargroup.md) padrão do usuário.</span><span class="sxs-lookup"><span data-stu-id="98fa4-120">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to the user's default [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}/events/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/calendars/{id}/events/{id}/attachments/{id}

GET /me/calendargroup/calendars/{id}/events/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/attachments/{id}
```
<span data-ttu-id="98fa4-121">Anexos de um [event](../resources/event.md) em um [calendar](../resources/calendar.md) que pertence a um [calendarGroup](../resources/calendargroup.md) de um usuário.</span><span class="sxs-lookup"><span data-stu-id="98fa4-121">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to a user's [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendargroups/{id}/calendars/{id}/events/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/attachments/{id}
```
<span data-ttu-id="98fa4-122">Anexos de uma [message](../resources/message.md) em uma caixa de correio de usuário.</span><span class="sxs-lookup"><span data-stu-id="98fa4-122">Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/messages/{id}/attachments/{id}
```
<span data-ttu-id="98fa4-123">Anexos de uma [message](../resources/message.md) contidos em uma [mailFolder](../resources/mailfolder.md) de nível superior na caixa de correio de um usuário.</span><span class="sxs-lookup"><span data-stu-id="98fa4-123">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments/{id}
```
<span data-ttu-id="98fa4-124">Anexos de uma [mensagem](../resources/message.md) contidos em uma pasta filho de um [mailFolder](../resources/mailfolder.md) na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="98fa4-124">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>  <span data-ttu-id="98fa4-125">O exemplo a seguir mostra um nível de aninhamento, mas uma mensagem pode estar localizada no filho de um filho e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="98fa4-125">The example below shows one level of nesting, but a message can be located in a child of a child and so on.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```
<span data-ttu-id="98fa4-126">Anexos de uma [post](../resources/post.md) em um [thread](../resources/conversationthread.md) que pertence a uma [conversation](../resources/conversation.md) de um grupo.</span><span class="sxs-lookup"><span data-stu-id="98fa4-126">Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts/{id}/attachments/{id}
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="98fa4-127">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="98fa4-127">Optional query parameters</span></span>
<span data-ttu-id="98fa4-128">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="98fa4-128">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="98fa4-129">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="98fa4-129">Request headers</span></span>
| <span data-ttu-id="98fa4-130">Nome</span><span class="sxs-lookup"><span data-stu-id="98fa4-130">Name</span></span>       | <span data-ttu-id="98fa4-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="98fa4-131">Type</span></span> | <span data-ttu-id="98fa4-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="98fa4-132">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="98fa4-133">Autorização</span><span class="sxs-lookup"><span data-stu-id="98fa4-133">Authorization</span></span>  | <span data-ttu-id="98fa4-134">string</span><span class="sxs-lookup"><span data-stu-id="98fa4-134">string</span></span>  | <span data-ttu-id="98fa4-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="98fa4-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="98fa4-137">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="98fa4-137">Request body</span></span>
<span data-ttu-id="98fa4-138">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="98fa4-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="98fa4-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="98fa4-139">Response</span></span>

<span data-ttu-id="98fa4-p105">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto **attachment** no corpo da resposta. As propriedades desse tipo de anexo são retornadas: [fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md) ou [referenceAttachment](../resources/referenceattachment.md).</span><span class="sxs-lookup"><span data-stu-id="98fa4-p105">If successful, this method returns a `200 OK` response code and an **attachment** object in the response body. The properties of that type of attachment are returned: [fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md), or [referenceAttachment](../resources/referenceattachment.md).</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="98fa4-142">Exemplo (anexo de arquivo)</span><span class="sxs-lookup"><span data-stu-id="98fa4-142">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="98fa4-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="98fa4-143">Request</span></span>
<span data-ttu-id="98fa4-144">Veja um exemplo da solicitação para obter um anexo de arquivo em um evento.</span><span class="sxs-lookup"><span data-stu-id="98fa4-144">Here is an example of the request to get a file attachment on an event.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_file_attachment"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/events/{id}/attachments/{id}
```

##### <a name="response"></a><span data-ttu-id="98fa4-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="98fa4-145">Response</span></span>
<span data-ttu-id="98fa4-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="98fa4-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.fileAttachment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 199

{
  "@odata.type": "#microsoft.graph.fileAttachment",
  "contentType": "contentType-value",
  "contentLocation": "contentLocation-value",
  "contentBytes": "binary",
  "contentId": "null",
  "lastModifiedDateTime": "2016-01-01T12:00:00Z",
  "id": "id-value",
  "isInline": false,
  "name": "name-value",
  "size": 99
}
```
## <a name="example-item-attachment"></a><span data-ttu-id="98fa4-149">Exemplo (anexo de item)</span><span class="sxs-lookup"><span data-stu-id="98fa4-149">Example (item attachment)</span></span>

##### <a name="request-1"></a><span data-ttu-id="98fa4-150">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="98fa4-150">Request 1</span></span>
<span data-ttu-id="98fa4-p107">O primeiro exemplo mostra como obter um anexo do item em uma mensagem. As propriedades de **itemAttachment** são retornadas.</span><span class="sxs-lookup"><span data-stu-id="98fa4-p107">The first example shows how to get an item attachment on a message. The properties of the **itemAttachment** are returned.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADA1M-zAAA=", "AAMkADA1M-CJKtzmnlcqVgqI="],
  "name": "get_item_attachment"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/AAMkADA1M-zAAA=/attachments/AAMkADA1M-CJKtzmnlcqVgqI=
```

##### <a name="response-1"></a><span data-ttu-id="98fa4-153">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="98fa4-153">Response 1</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemAttachment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('d1a2fae9-db66-4cc9-8133-2184c77af1b8')/messages('AAMkADA1M-zAAA%3D')/attachments/$entity",
  "@odata.type":"#microsoft.graph.itemAttachment",
  "id":"AAMkADA1MCJKtzmnlcqVgqI=",
  "lastModifiedDateTime":"2017-07-21T00:20:34Z",
  "name":"Reminder - please bring laptop",
  "contentType":null,
  "size":32005,
  "isInline":false
}
```

##### <a name="request-2"></a><span data-ttu-id="98fa4-154">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="98fa4-154">Request 2</span></span>
<span data-ttu-id="98fa4-p108">O exemplo a seguir mostra como usar `$expand` para obter as propriedades do item que está anexado à mensagem. Neste exemplo, esse item é uma mensagem. As propriedades dessa mensagem anexadas também são retornadas.</span><span class="sxs-lookup"><span data-stu-id="98fa4-p108">The next example shows how to use `$expand` to get the properties of the item that is attached to the message. In this example, that item is a message; the properties of that attached message are also returned.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADA1M-zAAA=", "AAMkADA1M-CJKtzmnlcqVgqI="],
  "name": "get_and_expand_item_attachment"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/AAMkADA1M-zAAA=/attachments/AAMkADA1M-CJKtzmnlcqVgqI=/?$expand=microsoft.graph.itemattachment/item 
```

##### <a name="response-2"></a><span data-ttu-id="98fa4-157">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="98fa4-157">Response 2</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemAttachment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('d1a2fae9-db66-4cc9-8133-2184c77af1b8')/messages('AAMkADA1M-zAAA%3D')/attachments/$entity",
  "@odata.type":"#microsoft.graph.itemAttachment",
  "id":"AAMkADA1MCJKtzmnlcqVgqI=",
  "lastModifiedDateTime":"2017-07-21T00:20:34Z",
  "name":"Reminder - please bring laptop",
  "contentType":null,
  "size":32005,
  "isInline":false,
  "item@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('d1a2fae9-db66-4cc9-8133-2184c77af1b8')/messages('AAMkADA1M-zAAA%3D')/attachments('AAMkADA1M-CJKtzmnlcqVgqI%3D')/microsoft.graph.itemAttachment/item/$entity",
  "item":{
    "@odata.type":"#microsoft.graph.message",
    "id":"",
    "createdDateTime":"2017-07-21T00:20:41Z",
    "lastModifiedDateTime":"2017-07-21T00:20:34Z",
    "receivedDateTime":"2017-07-21T00:19:55Z",
    "sentDateTime":"2017-07-21T00:19:52Z",
    "hasAttachments":false,
    "internetMessageId":"<BY2PR15MB05189A084C01F466709E414F9CA40@BY2PR15MB0518.namprd15.prod.outlook.com>",
    "subject":"Reminder - please bring laptop",
    "importance":"normal",
    "conversationId":"AAQkADA1MzMyOGI4LTlkZDctNDkzYy05M2RiLTdiN2E1NDE3MTRkOQAQAMG_NSCMBqdKrLa2EmR-lO0=",
    "isDeliveryReceiptRequested":false,
    "isReadReceiptRequested":false,
    "isRead":false,
    "isDraft":false,
    "webLink":"https://outlook.office365.com/owa/?ItemID=AAMkADA1M3MTRkOQAAAA%3D%3D&exvsurl=1&viewmodel=ReadMessageItem",
    "body":{
      "contentType":"html",
      "content":"<html><head>\r\n</head>\r\n<body>\r\n</body>\r\n</html>"
    },
    "sender":{
      "emailAddress":{
        "name":"Adele Vance",
        "address":"AdeleV@contoso.onmicrosoft.com"
      }
    },
    "from":{
      "emailAddress":{
        "name":"Adele Vance",
        "address":"AdeleV@contoso.onmicrosoft.com"
      }
    },
    "toRecipients":[
      {
        "emailAddress":{
          "name":"Alex Wilbur",
          "address":"AlexW@contoso.onmicrosoft.com"
        }
      }
    ],
    "ccRecipients":[
      {
        "emailAddress":{
          "name":"Adele Vance",
          "address":"AdeleV@contoso.onmicrosoft.com"
        }
      }
    ]
  }
}
```



## <a name="example-reference-attachment"></a><span data-ttu-id="98fa4-158">Exemplo (anexo de referência)</span><span class="sxs-lookup"><span data-stu-id="98fa4-158">Example (reference attachment)</span></span>
##### <a name="request"></a><span data-ttu-id="98fa4-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="98fa4-159">Request</span></span>
<span data-ttu-id="98fa4-160">Aqui está um exemplo da solicitação para obter um anexo de referência em um evento.</span><span class="sxs-lookup"><span data-stu-id="98fa4-160">Here is an example of the request to get a reference attachment on an event.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_reference_attachment"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/events/{id}/attachments/{id}
```
##### <a name="response"></a><span data-ttu-id="98fa4-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="98fa4-161">Response</span></span>
<span data-ttu-id="98fa4-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="98fa4-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.referenceAttachment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 215

{
  "@odata.type": "#microsoft.graph.referenceAttachment",
  "contentType": "contentType-value",
  "lastModifiedDateTime": "datetime-value",
  "id": "id-value",
  "isInline": false,
  "name": "name-value",
  "size": 99,
}
```



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get attachment",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Error: get_and_expand_item_attachment/item:
      Property 'item' is of type Custom but has no custom members."
  ],
  "tocPath": ""
}-->
