---
title: Obter anexo
description: Leia as propriedades e relacionamentos de um anexo, anexados a um evento, mensagem, tarefa do Outlook ou postagem.
localization_priority: Normal
ms.openlocfilehash: 1618d7a8bd866bb36ee9e18475f6f9c40a8190e8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27809552"
---
# <a name="get-attachment"></a><span data-ttu-id="dbb6c-103">Obter anexo</span><span class="sxs-lookup"><span data-stu-id="dbb6c-103">Get attachment</span></span>

> <span data-ttu-id="dbb6c-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="dbb6c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dbb6c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="dbb6c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="dbb6c-106">Leia as propriedades e relacionamentos de um anexo, anexados a um [evento](../resources/event.md), [mensagem](../resources/message.md), [tarefa do Outlook](../resources/outlooktask.md)ou [postar](../resources/post.md).</span><span class="sxs-lookup"><span data-stu-id="dbb6c-106">Read the properties and relationships of an attachment, attached to an [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md).</span></span>

<span data-ttu-id="dbb6c-107">Um anexo pode ser de um dos seguintes tipos:</span><span class="sxs-lookup"><span data-stu-id="dbb6c-107">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="dbb6c-108">Um arquivo (recurso [fileAttachment](../resources/fileattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="dbb6c-108">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="dbb6c-p102">Um item (contato, evento ou mensagem, representado por um recurso [itemAttachment](../resources/itemattachment.md)). Você pode usar `$expand` para obter ainda mais as propriedades desse item. Veja um [exemplo](#request-2) abaixo.</span><span class="sxs-lookup"><span data-stu-id="dbb6c-p102">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource). You can use `$expand` to further get the properties of that item. See an [example](#request-2) below.</span></span>
* <span data-ttu-id="dbb6c-112">Um link para um arquivo (recurso [referenceAttachment](../resources/referenceattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="dbb6c-112">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource).</span></span>

<span data-ttu-id="dbb6c-113">Todos esses tipos de recursos de anexo são derivados do recurso [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="dbb6c-113">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="dbb6c-114">Permissões</span><span class="sxs-lookup"><span data-stu-id="dbb6c-114">Permissions</span></span>

<span data-ttu-id="dbb6c-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dbb6c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="dbb6c-117">Se acessando anexos em mensagens: Mail.Read</span><span class="sxs-lookup"><span data-stu-id="dbb6c-117">If accessing attachments in messages: Mail.Read</span></span>
* <span data-ttu-id="dbb6c-118">Se acessando anexos em eventos: Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="dbb6c-118">If accessing attachments in events: Calendars.Read</span></span>
* <span data-ttu-id="dbb6c-119">Se acessando anexos em tarefas do Outlook: Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="dbb6c-119">If accessing attachments in Outlook tasks: Tasks.Read</span></span>
* <span data-ttu-id="dbb6c-120">Se acessando anexos em postagens de grupo: Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="dbb6c-120">If accessing attachments in group posts: Group.Read.All</span></span>

<!--
* If accessing attachments in group events or posts: Group.Read.All
-->

## <a name="http-request"></a><span data-ttu-id="dbb6c-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dbb6c-121">HTTP request</span></span>

<span data-ttu-id="dbb6c-122">Anexos para um [evento](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="dbb6c-122">Attachments for an [event](../resources/event.md).</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/events/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/events/{id}/attachments/{id}
```

<!--
GET /groups/{id}/events/{id}/attachments/{id}
-->

<span data-ttu-id="dbb6c-123">Anexos de uma [message](../resources/message.md) em uma caixa de correio de usuário.</span><span class="sxs-lookup"><span data-stu-id="dbb6c-123">Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /me/messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/messages/{id}/attachments/{id}
```

<span data-ttu-id="dbb6c-124">Anexos de uma [message](../resources/message.md) contidos em uma [mailFolder](../resources/mailfolder.md) de nível superior na caixa de correio de um usuário.</span><span class="sxs-lookup"><span data-stu-id="dbb6c-124">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /me/mailFolders/{id}/messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments/{id}
```

<span data-ttu-id="dbb6c-125">Anexos de uma [mensagem](../resources/message.md) contidos em uma pasta filho de um [mailFolder](../resources/mailfolder.md) na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="dbb6c-125">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>  <span data-ttu-id="dbb6c-126">O exemplo a seguir mostra um nível de aninhamento, mas uma mensagem pode estar localizada no filho de um filho e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="dbb6c-126">The example below shows one level of nesting, but a message can be located in a child of a child and so on.</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```

<span data-ttu-id="dbb6c-127">Anexos para uma [tarefa do Outlook](../resources/outlooktask.md).</span><span class="sxs-lookup"><span data-stu-id="dbb6c-127">Attachments for an [Outlook task](../resources/outlooktask.md).</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /me/outlook/tasks/<id>/attachments/{id}
GET /users/<id>/outlook/tasks/<id>/attachments/{id}
```

<span data-ttu-id="dbb6c-128">Anexos de uma [post](../resources/post.md) em um [thread](../resources/conversationthread.md) que pertence a uma [conversation](../resources/conversation.md) de um grupo.</span><span class="sxs-lookup"><span data-stu-id="dbb6c-128">Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /groups/{id}/threads/{id}/posts/{id}/attachments/{id}
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="dbb6c-129">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="dbb6c-129">Optional query parameters</span></span>

<span data-ttu-id="dbb6c-130">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="dbb6c-130">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dbb6c-131">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dbb6c-131">Request headers</span></span>

| <span data-ttu-id="dbb6c-132">Nome</span><span class="sxs-lookup"><span data-stu-id="dbb6c-132">Name</span></span>       | <span data-ttu-id="dbb6c-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="dbb6c-133">Type</span></span> | <span data-ttu-id="dbb6c-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="dbb6c-134">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="dbb6c-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="dbb6c-135">Authorization</span></span>  | <span data-ttu-id="dbb6c-136">string</span><span class="sxs-lookup"><span data-stu-id="dbb6c-136">string</span></span>  | <span data-ttu-id="dbb6c-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dbb6c-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dbb6c-139">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dbb6c-139">Request body</span></span>

<span data-ttu-id="dbb6c-140">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="dbb6c-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dbb6c-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="dbb6c-141">Response</span></span>

<span data-ttu-id="dbb6c-142">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [attachment](../resources/attachment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dbb6c-142">If successful, this method returns a `200 OK` response code and [attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="dbb6c-143">Exemplo (anexo de arquivo)</span><span class="sxs-lookup"><span data-stu-id="dbb6c-143">Example (file attachment)</span></span>

### <a name="request"></a><span data-ttu-id="dbb6c-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dbb6c-144">Request</span></span>

<span data-ttu-id="dbb6c-145">Veja um exemplo da solicitação para obter um anexo de arquivo em um evento.</span><span class="sxs-lookup"><span data-stu-id="dbb6c-145">Here is an example of the request to get a file attachment on an event.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_file_attachment"
}-->

```http
GET https://graph.microsoft.com/beta/me/events/{id}/attachments/{id}
```

### <a name="response"></a><span data-ttu-id="dbb6c-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="dbb6c-146">Response</span></span>

<span data-ttu-id="dbb6c-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dbb6c-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "contentBytes": "contentBytes-value",
  "contentId": "null",
  "lastModifiedDateTime": "2016-01-01T12:00:00Z",
  "id": "id-value",
  "isInline": false,
  "name": "name-value",
  "size": 99
}
```

## <a name="example-item-attachment"></a><span data-ttu-id="dbb6c-150">Exemplo (anexo de item)</span><span class="sxs-lookup"><span data-stu-id="dbb6c-150">Example (item attachment)</span></span>

### <a name="request-1"></a><span data-ttu-id="dbb6c-151">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="dbb6c-151">Request 1</span></span>

<span data-ttu-id="dbb6c-p107">O primeiro exemplo mostra como obter um anexo do item em uma mensagem. As propriedades de **itemAttachment** são retornadas.</span><span class="sxs-lookup"><span data-stu-id="dbb6c-p107">The first example shows how to get an item attachment on a message. The properties of the **itemAttachment** are returned.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_item_attachment"
}-->

```http
GET https://graph.microsoft.com/beta/me/messages('AAMkADA1M-zAAA=')/attachments('AAMkADA1M-CJKtzmnlcqVgqI=')
```

### <a name="response-1"></a><span data-ttu-id="dbb6c-154">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="dbb6c-154">Response 1</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemAttachment"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('d1a2fae9-db66-4cc9-8133-2184c77af1b8')/messages('AAMkADA1M-zAAA%3D')/attachments/$entity",
  "@odata.type":"#microsoft.graph.itemAttachment",
  "id":"AAMkADA1MCJKtzmnlcqVgqI=",
  "lastModifiedDateTime":"2017-07-21T00:20:34Z",
  "name":"Reminder - please bring laptop",
  "contentType":null,
  "size":32005,
  "isInline":false
}
```

### <a name="request-2"></a><span data-ttu-id="dbb6c-155">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="dbb6c-155">Request 2</span></span>

<span data-ttu-id="dbb6c-p108">O exemplo a seguir mostra como usar `$expand` para obter as propriedades do item que está anexado à mensagem. Neste exemplo, esse item é uma mensagem. As propriedades dessa mensagem anexadas também são retornadas.</span><span class="sxs-lookup"><span data-stu-id="dbb6c-p108">The next example shows how to use `$expand` to get the properties of the item that is attached to the message. In this example, that item is a message; the properties of that attached message are also returned.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_and_expand_item_attachment"
}-->

```http
GET https://graph.microsoft.com/beta/me/messages('AAMkADA1M-zAAA=')/attachments('AAMkADA1M-CJKtzmnlcqVgqI=')/?$expand=microsoft.graph.itemattachment/item
```

### <a name="response-2"></a><span data-ttu-id="dbb6c-158">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="dbb6c-158">Response 2</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemAttachment"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('d1a2fae9-db66-4cc9-8133-2184c77af1b8')/messages('AAMkADA1M-zAAA%3D')/attachments/$entity",
  "@odata.type":"#microsoft.graph.itemAttachment",
  "id":"AAMkADA1MCJKtzmnlcqVgqI=",
  "lastModifiedDateTime":"2017-07-21T00:20:34Z",
  "name":"Reminder - please bring laptop",
  "contentType":null,
  "size":32005,
  "isInline":false,
  "item@odata.context":"https://graph.microsoft.com/beta/$metadata#users('d1a2fae9-db66-4cc9-8133-2184c77af1b8')/messages('AAMkADA1M-zAAA%3D')/attachments('AAMkADA1M-CJKtzmnlcqVgqI%3D')/microsoft.graph.itemAttachment/item/$entity",
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
    "conversationIndex":"AQHTAbcSwb41IIwGp0qstrYSZH+U7Q==",
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
    ],
    "flag":{
      "flagStatus":"notFlagged"
    }
  }
}
```

## <a name="example-reference-attachment"></a><span data-ttu-id="dbb6c-159">Exemplo (anexo de referência)</span><span class="sxs-lookup"><span data-stu-id="dbb6c-159">Example (reference attachment)</span></span>

### <a name="request"></a><span data-ttu-id="dbb6c-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dbb6c-160">Request</span></span>

<span data-ttu-id="dbb6c-161">Aqui está um exemplo da solicitação para obter um anexo de referência em um evento.</span><span class="sxs-lookup"><span data-stu-id="dbb6c-161">Here is an example of the request to get a reference attachment on an event.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_reference_attachment"
}-->

```http
GET https://graph.microsoft.com/beta/me/events/AAMkAGE1M88AADUv0uAAAG=/attachments/AAMkAGE1Mg72tgf7hJp0PICVGCc0g=
```

### <a name="response"></a><span data-ttu-id="dbb6c-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="dbb6c-162">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.referenceAttachment"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#users/ddfcd489-628b-40d7-b48b-57002df800e5/events/AAMkAGE1M88AADUv0uAAAG%3D/attachments/$entity",
  "@odata.type": "#microsoft.graph.referenceAttachment",
  "id": "AAMkAGE1Mg72tgf7hJp0PCGVCIc0g=",
  "lastModifiedDateTime": "2016-03-12T06:04:38Z",
  "name": "Personal pictures",
  "contentType": null,
  "size": 382,
  "isInline": false,
  "sourceUrl": "https://contoso.com/personal/mario_contoso_net/Documents/Pics",
  "providerType": "oneDriveConsumer",
  "thumbnailUrl": null,
  "previewUrl": null,
  "permission": "edit",
  "isFolder": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
