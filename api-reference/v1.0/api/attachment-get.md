---
title: Obter anexo
description: 'Leia as propriedades e as relações de um anexo, anexados a um evento,  '
localization_priority: Priority
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: faddcad421a588ccb6940239a05d9479bc7ec76d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36004082"
---
# <a name="get-attachment"></a>Obter anexo

Leia as propriedades e as relações de um anexo, anexado a um [event](../resources/event.md), [message](../resources/message.md) ou [post](../resources/post.md). 

Um anexo pode ser de um dos seguintes tipos:

* Um arquivo (recurso [fileAttachment](../resources/fileattachment.md)).
* Um item (contato, evento ou mensagem, representado por um recurso [itemAttachment](../resources/itemattachment.md)). Você pode usar `$expand` para obter mais propriedades desse item. Veja um [exemplo](#request-2) abaixo.
* Um link para um arquivo (recurso [referenceAttachment](../resources/referenceattachment.md)).

Todos esses tipos de recursos de anexo são derivados do recurso [attachment](../resources/attachment.md). 


## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

* Se estiver acessando anexos em Mensagens: Mail.Read.
* Se estiver acessando anexos em Eventos: Calendars.Read.
* Se estiver acessando anexos em postagens de grupo: Group.Read.All.

<!--
* If accessing attachments in group events or posts: Group.Read.All.
-->

## <a name="http-request"></a>Solicitação HTTP
Anexos de um [event](../resources/event.md) no [calendar](../resources/calendar.md) padrão do usuário.

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

Anexos de um [event](../resources/event.md) em um [calendar](../resources/calendar.md) que pertence ao [calendarGroup](../resources/calendargroup.md) padrão do usuário.
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}/events/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/calendars/{id}/events/{id}/attachments/{id}

GET /me/calendargroup/calendars/{id}/events/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/attachments/{id}
```
Anexos de um [event](../resources/event.md) em um [calendar](../resources/calendar.md) que pertence a um [calendarGroup](../resources/calendargroup.md) de um usuário.
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendargroups/{id}/calendars/{id}/events/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/attachments/{id}
```
Anexos de uma [message](../resources/message.md) em uma caixa de correio de usuário.
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/messages/{id}/attachments/{id}
```
Anexos de uma [message](../resources/message.md) contidos em uma [mailFolder](../resources/mailfolder.md) de nível superior na caixa de correio de um usuário.
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments/{id}
```
Anexos de uma [message](../resources/message.md) contidos em uma pasta filha de uma [mailFolder](../resources/mailfolder.md) na caixa de correio de um usuário.  O exemplo a seguir mostra um nível de aninhamento, mas uma mensagem pode estar localizada em um filho de um filho, e assim por diante. <!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```
Anexos de uma [post](../resources/post.md) em um [thread](../resources/conversationthread.md) que pertence a uma [conversation](../resources/conversation.md) de um grupo.
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts/{id}/attachments/{id}
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments/{id}
```
## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome       | Tipo | Descrição|
|:-----------|:------|:----------|
| Autorização  | string  | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto **attachment** no corpo da resposta. As propriedades desse tipo de anexo são retornadas: [fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md) ou [referenceAttachment](../resources/referenceattachment.md).

## <a name="example-file-attachment"></a>Exemplo (anexo de arquivo)

##### <a name="request"></a>Solicitação
Veja um exemplo da solicitação para obter um anexo de arquivo de um evento.

# <a name="httptabhttp"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_file_attachment"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/events/{id}/attachments/{id}
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-file-attachment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-file-attachment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-file-attachment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-file-attachment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
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
## <a name="example-item-attachment"></a>Exemplo (anexo de item)

##### <a name="request-1"></a>Solicitação 1
O primeiro exemplo mostra como obter um anexo do item em uma mensagem. As propriedades de **itemAttachment** são retornadas.

# <a name="httptabhttp"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADA1M-zAAA=", "AAMkADA1M-CJKtzmnlcqVgqI="],
  "name": "get_item_attachment"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/AAMkADA1M-zAAA=/attachments/AAMkADA1M-CJKtzmnlcqVgqI=
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-item-attachment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-item-attachment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-item-attachment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-item-attachment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response-1"></a>Resposta 1
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

##### <a name="request-2"></a>Solicitação 2
O exemplo a seguir mostra como usar `$expand` para obter as propriedades do item que está anexado à mensagem. Neste exemplo, esse item é uma mensagem. As propriedades dessa mensagem anexadas também são retornadas.

# <a name="httptabhttp"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADA1M-zAAA=", "AAMkADA1M-CJKtzmnlcqVgqI="],
  "name": "get_and_expand_item_attachment"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/AAMkADA1M-zAAA=/attachments/AAMkADA1M-CJKtzmnlcqVgqI=/?$expand=microsoft.graph.itemattachment/item 
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-and-expand-item-attachment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-and-expand-item-attachment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-and-expand-item-attachment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-and-expand-item-attachment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response-2"></a>Resposta 2
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



## <a name="example-reference-attachment"></a>Exemplo (anexo de referência)
##### <a name="request"></a>Solicitação
Aqui está um exemplo da solicitação para obter um anexo de referência de uma mensagem.

# <a name="httptabhttp"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_reference_attachment",
  "sampleKeys": ["AAMkAGUzY5QKgAAA=","AAMkAGUzY5QKgAAABEgAQAISJOe1FEqdNsMEQmpZjRW8="]
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/AAMkAGUzY5QKgAAA=/attachments/AAMkAGUzY5QKgAAABEgAQAISJOe1FEqdNsMEQmpZjRW8=
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-reference-attachment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-reference-attachment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-reference-attachment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-reference-attachment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
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
