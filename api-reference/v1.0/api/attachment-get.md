---
title: Obter anexo
description: 'Leia as propriedades e as relações de um anexo, anexados a um evento,  '
localization_priority: Priority
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 09fac27ef28fe30a69c03a7bfb18e8c3d95575f8
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35264803"
---
# <a name="get-attachment"></a><span data-ttu-id="74b8b-103">Obter anexo</span><span class="sxs-lookup"><span data-stu-id="74b8b-103">Get attachment</span></span>

<span data-ttu-id="74b8b-104">Leia as propriedades e as relações de um anexo, anexado a um [event](../resources/event.md), [message](../resources/message.md) ou [post](../resources/post.md).</span><span class="sxs-lookup"><span data-stu-id="74b8b-104">Read the properties and relationships of an attachment, attached to an [event](../resources/event.md), [message](../resources/message.md), or [post](../resources/post.md).</span></span> 

<span data-ttu-id="74b8b-105">Um anexo pode ser de um dos seguintes tipos:</span><span class="sxs-lookup"><span data-stu-id="74b8b-105">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="74b8b-106">Um arquivo (recurso [fileAttachment](../resources/fileattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="74b8b-106">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="74b8b-107">Um item (contato, evento ou mensagem, representado por um recurso [itemAttachment](../resources/itemattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="74b8b-107">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource).</span></span> <span data-ttu-id="74b8b-108">Você pode usar `$expand` para obter mais propriedades desse item.</span><span class="sxs-lookup"><span data-stu-id="74b8b-108">You can use `$expand` to further get the properties of that item.</span></span> <span data-ttu-id="74b8b-109">Veja um [exemplo](#request-2) abaixo.</span><span class="sxs-lookup"><span data-stu-id="74b8b-109">See an [example](#request-2) below.</span></span>
* <span data-ttu-id="74b8b-110">Um link para um arquivo (recurso [referenceAttachment](../resources/referenceattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="74b8b-110">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource).</span></span>

<span data-ttu-id="74b8b-111">Todos esses tipos de recursos de anexo são derivados do recurso [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="74b8b-111">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span> 


## <a name="permissions"></a><span data-ttu-id="74b8b-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="74b8b-112">Permissions</span></span>
<span data-ttu-id="74b8b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="74b8b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="74b8b-115">Se estiver acessando anexos em Mensagens: Mail.Read.</span><span class="sxs-lookup"><span data-stu-id="74b8b-115">If accessing attachments in Messages: Mail.Read</span></span>
* <span data-ttu-id="74b8b-116">Se estiver acessando anexos em Eventos: Calendars.Read.</span><span class="sxs-lookup"><span data-stu-id="74b8b-116">If accessing attachments in Events: Calendars.Read</span></span>
* <span data-ttu-id="74b8b-117">Se estiver acessando anexos em postagens de grupo: Group.Read.All.</span><span class="sxs-lookup"><span data-stu-id="74b8b-117">If accessing attachments in group events or posts: Group.Read.All</span></span>

<!--
* If accessing attachments in group events or posts: Group.Read.All.
-->

## <a name="http-request"></a><span data-ttu-id="74b8b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="74b8b-118">HTTP request</span></span>
<span data-ttu-id="74b8b-119">Anexos de um [event](../resources/event.md) no [calendar](../resources/calendar.md) padrão do usuário.</span><span class="sxs-lookup"><span data-stu-id="74b8b-119">Attachments for an [event](../resources/event.md) in the user's or group's default [calendar](../resources/calendar.md).</span></span>

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

<span data-ttu-id="74b8b-120">Anexos de um [event](../resources/event.md) em um [calendar](../resources/calendar.md) que pertence ao [calendarGroup](../resources/calendargroup.md) padrão do usuário.</span><span class="sxs-lookup"><span data-stu-id="74b8b-120">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to the user's default [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}/events/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/calendars/{id}/events/{id}/attachments/{id}

GET /me/calendargroup/calendars/{id}/events/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/attachments/{id}
```
<span data-ttu-id="74b8b-121">Anexos de um [event](../resources/event.md) em um [calendar](../resources/calendar.md) que pertence a um [calendarGroup](../resources/calendargroup.md) de um usuário.</span><span class="sxs-lookup"><span data-stu-id="74b8b-121">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to a user's [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendargroups/{id}/calendars/{id}/events/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/attachments/{id}
```
<span data-ttu-id="74b8b-122">Anexos de uma [message](../resources/message.md) em uma caixa de correio de usuário.</span><span class="sxs-lookup"><span data-stu-id="74b8b-122">Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/messages/{id}/attachments/{id}
```
<span data-ttu-id="74b8b-123">Anexos de uma [message](../resources/message.md) contidos em uma [mailFolder](../resources/mailfolder.md) de nível superior na caixa de correio de um usuário.</span><span class="sxs-lookup"><span data-stu-id="74b8b-123">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments/{id}
```
<span data-ttu-id="74b8b-p103">Anexos de uma [message](../resources/message.md) contidos em uma pasta filha de uma [mailFolder](../resources/mailfolder.md) na caixa de correio de um usuário.  O exemplo a seguir mostra um nível de aninhamento, mas uma mensagem pode estar localizada em um filho de um filho, e assim por diante. </span><span class="sxs-lookup"><span data-stu-id="74b8b-p103">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.  The example below shows one level of nesting, but a message can be located in a child of a child and so on. </span></span><!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```
<span data-ttu-id="74b8b-126">Anexos de uma [post](../resources/post.md) em um [thread](../resources/conversationthread.md) que pertence a uma [conversation](../resources/conversation.md) de um grupo.</span><span class="sxs-lookup"><span data-stu-id="74b8b-126">Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts/{id}/attachments/{id}
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="74b8b-127">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="74b8b-127">Optional query parameters</span></span>
<span data-ttu-id="74b8b-128">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="74b8b-128">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="74b8b-129">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="74b8b-129">Request headers</span></span>
| <span data-ttu-id="74b8b-130">Nome</span><span class="sxs-lookup"><span data-stu-id="74b8b-130">Name</span></span>       | <span data-ttu-id="74b8b-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="74b8b-131">Type</span></span> | <span data-ttu-id="74b8b-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="74b8b-132">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="74b8b-133">Autorização</span><span class="sxs-lookup"><span data-stu-id="74b8b-133">Authorization</span></span>  | <span data-ttu-id="74b8b-134">string</span><span class="sxs-lookup"><span data-stu-id="74b8b-134">string</span></span>  | <span data-ttu-id="74b8b-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="74b8b-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="74b8b-137">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="74b8b-137">Request body</span></span>
<span data-ttu-id="74b8b-138">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="74b8b-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="74b8b-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="74b8b-139">Response</span></span>

<span data-ttu-id="74b8b-140">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto **attachment** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="74b8b-140">If successful, this method returns a `200 OK` response code and **attachment** object in the response body.</span></span> <span data-ttu-id="74b8b-141">As propriedades desse tipo de anexo são retornadas: [fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md) ou [referenceAttachment](../resources/referenceattachment.md).</span><span class="sxs-lookup"><span data-stu-id="74b8b-141">The properties of that type of attachment are returned: [fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md), or [referenceAttachment](../resources/referenceattachment.md).</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="74b8b-142">Exemplo (anexo de arquivo)</span><span class="sxs-lookup"><span data-stu-id="74b8b-142">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="74b8b-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="74b8b-143">Request</span></span>
<span data-ttu-id="74b8b-144">Veja um exemplo da solicitação para obter um anexo de arquivo em um evento.</span><span class="sxs-lookup"><span data-stu-id="74b8b-144">Here is an example of the request to get a file attachment on an event.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_file_attachment"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/events/{id}/attachments/{id}
```

##### <a name="response"></a><span data-ttu-id="74b8b-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="74b8b-145">Response</span></span>
<span data-ttu-id="74b8b-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="74b8b-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="74b8b-149">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="74b8b-149">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="74b8b-150">C#</span><span class="sxs-lookup"><span data-stu-id="74b8b-150">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_file_attachment-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="74b8b-151">Javascript</span><span class="sxs-lookup"><span data-stu-id="74b8b-151">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_file_attachment-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="74b8b-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="74b8b-152">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_file_attachment-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
## <a name="example-item-attachment"></a><span data-ttu-id="74b8b-153">Exemplo (anexo de item)</span><span class="sxs-lookup"><span data-stu-id="74b8b-153">Example (item attachment)</span></span>

##### <a name="request-1"></a><span data-ttu-id="74b8b-154">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="74b8b-154">Request 1</span></span>
<span data-ttu-id="74b8b-155">O primeiro exemplo mostra como obter um anexo do item em uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="74b8b-155">The first example shows how to get an item attachment on a message.</span></span> <span data-ttu-id="74b8b-156">As propriedades de **itemAttachment** são retornadas.</span><span class="sxs-lookup"><span data-stu-id="74b8b-156">The properties of the **itemAttachment** are returned.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADA1M-zAAA=", "AAMkADA1M-CJKtzmnlcqVgqI="],
  "name": "get_item_attachment"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/AAMkADA1M-zAAA=/attachments/AAMkADA1M-CJKtzmnlcqVgqI=
```

##### <a name="response-1"></a><span data-ttu-id="74b8b-157">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="74b8b-157">Response 1</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="74b8b-158">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="74b8b-158">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="74b8b-159">C#</span><span class="sxs-lookup"><span data-stu-id="74b8b-159">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_item_attachment-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="74b8b-160">Javascript</span><span class="sxs-lookup"><span data-stu-id="74b8b-160">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_item_attachment-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="74b8b-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="74b8b-161">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_item_attachment-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

##### <a name="request-2"></a><span data-ttu-id="74b8b-162">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="74b8b-162">Request 2</span></span>
<span data-ttu-id="74b8b-163">O exemplo a seguir mostra como usar `$expand` para obter as propriedades do item que está anexado à mensagem.</span><span class="sxs-lookup"><span data-stu-id="74b8b-163">The next example shows how to use `$expand` to get the properties of the item that is attached to the message.</span></span> <span data-ttu-id="74b8b-164">Neste exemplo, esse item é uma mensagem. As propriedades dessa mensagem anexadas também são retornadas.</span><span class="sxs-lookup"><span data-stu-id="74b8b-164">In this example, that item is a message; the properties of that attached message are also returned.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADA1M-zAAA=", "AAMkADA1M-CJKtzmnlcqVgqI="],
  "name": "get_and_expand_item_attachment"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/AAMkADA1M-zAAA=/attachments/AAMkADA1M-CJKtzmnlcqVgqI=/?$expand=microsoft.graph.itemattachment/item 
```

##### <a name="response-2"></a><span data-ttu-id="74b8b-165">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="74b8b-165">Response 2</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="74b8b-166">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="74b8b-166">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="74b8b-167">C#</span><span class="sxs-lookup"><span data-stu-id="74b8b-167">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_and_expand_item_attachment-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="74b8b-168">Javascript</span><span class="sxs-lookup"><span data-stu-id="74b8b-168">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_and_expand_item_attachment-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="74b8b-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="74b8b-169">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_and_expand_item_attachment-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]



## <a name="example-reference-attachment"></a><span data-ttu-id="74b8b-170">Exemplo (anexo de referência)</span><span class="sxs-lookup"><span data-stu-id="74b8b-170">Example (reference attachment)</span></span>
##### <a name="request"></a><span data-ttu-id="74b8b-171">Solicitação</span><span class="sxs-lookup"><span data-stu-id="74b8b-171">Request</span></span>
<span data-ttu-id="74b8b-172">Aqui está um exemplo da solicitação para obter um anexo de referência em uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="74b8b-172">Here is an example of the request to get a reference attachment on an event.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_reference_attachment",
  "sampleKeys": ["AAMkAGUzY5QKgAAA=","AAMkAGUzY5QKgAAABEgAQAISJOe1FEqdNsMEQmpZjRW8="]
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/AAMkAGUzY5QKgAAA=/attachments/AAMkAGUzY5QKgAAABEgAQAISJOe1FEqdNsMEQmpZjRW8=
```
##### <a name="response"></a><span data-ttu-id="74b8b-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="74b8b-173">Response</span></span>
<span data-ttu-id="74b8b-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="74b8b-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "get_reference_attachment",
  "truncated": true,
  "@odata.type": "microsoft.graph.referenceAttachment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('bb8775a4-4d8c-42cf-a1d4-4d58c2bb668f')/messages('AAMkAGUzY5QKgAAA%3D')/attachments/$entity",
    "@odata.type": "#microsoft.graph.referenceAttachment",
    "id": "AAMkAGUzY5QKgAAABEgAQAISJOe1FEqdNsMEQmpZjRW8=",
    "lastModifiedDateTime": "2019-04-02T02:58:11Z",
    "name": "Sales Invoice Template.docx",
    "contentType": "application/vnd.openxmlformats-officedocument.wordprocessingml.document",
    "size": 1060,
    "isInline": true
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="74b8b-177">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="74b8b-177">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="74b8b-178">C#</span><span class="sxs-lookup"><span data-stu-id="74b8b-178">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_reference_attachment-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="74b8b-179">Javascript</span><span class="sxs-lookup"><span data-stu-id="74b8b-179">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_reference_attachment-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="74b8b-180">Objective-C</span><span class="sxs-lookup"><span data-stu-id="74b8b-180">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_reference_attachment-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get attachment",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Error: /api-reference/v1.0/api/attachment-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/attachment-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/attachment-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/attachment-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/attachment-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/attachment-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/attachment-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/attachment-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/attachment-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: get_and_expand_item_attachment/item:
      Property 'item' is of type Custom but has no custom members."
  ],
  "tocPath": ""
}-->
