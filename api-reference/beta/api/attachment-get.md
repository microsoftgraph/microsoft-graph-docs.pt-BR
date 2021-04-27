---
title: Obter anexo
description: Leia as propriedades e as relações de um anexo, anexado a um evento, mensagem, Outlook tarefa ou postagem.
localization_priority: Normal
doc_type: apiPageType
author: abheek-das
ms.prod: outlook
ms.openlocfilehash: 39c8be1eb33bd5843fe38c3715a3ee207e57c9f6
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048026"
---
# <a name="get-attachment"></a>Obter anexo

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-sharedfeature](../../includes/outlooktask-deprecate-sharedfeature.md)]

Leia as propriedades, relações ou conteúdo bruto de um anexo anexado a um evento de [usuário,](../resources/event.md) [mensagem,](../resources/message.md)Outlook [tarefa](../resources/outlooktask.md)ou postagem de [grupo.](../resources/post.md) 

Um anexo pode ser de um dos seguintes tipos:

* Um arquivo. Programaticamente, este é um recurso [fileAttachment](../resources/fileattachment.md). Veja [exemplo 1](#example-1-get-the-properties-of-a-file-attachment).
* Um item do Outlook (contato, evento ou mensagem). Programaticamente, um anexo de item é um recurso [itemAttachment](../resources/itemattachment.md). Você pode usar `$expand` para obter ainda mais as propriedades desse item, incluindo quaisquer anexos aninhados em até 30 níveis. Veja o [exemplo 3](#example-3-expand-and-get-the-properties-of-the-item-attached-to-a-message) e o [exemplo 4](#example-4-expand-and-get-the-properties-of-an-item-attached-to-a-message-including-any-attachment-to-the-item).
* Um link para um arquivo armazenado na nuvem. Programaticamente, este é um recurso [referenceAttachment](../resources/referenceattachment.md). Veja o[exemplo 5](#example-5-get-the-properties-of-a-reference-attachment).

Todos esses tipos de anexos são derivados do recurso [anexo](../resources/attachment.md). 

### <a name="get-the-raw-contents-of-a-file-or-item-attachment"></a>Obter o conteúdo bruto de um arquivo ou anexo de item
Você pode anexar o segmento do caminho `/$value` para obter o conteúdo bruto de um arquivo ou anexo de item. 

Para um anexo de arquivo, o tipo de conteúdo é baseado no tipo de conteúdo original. Consulte um [exemplo 6](#example-6-get-the-raw-contents-of-a-file-attachment-on-a-message).

Para um anexo de item que é um [contato](../resources/contact.md), [evento](../resources/event.md) ou [mensagem](../resources/message.md), o conteúdo bruto retornado está no formato MIME.

| Tipo de anexo do item  | Conteúdo bruto retornado |
|:-----------|:----------|
| **contato** | Formato [vCard](http://www.faqs.org/rfcs/rfc2426.html) MIME. Consulte [o exemplo 7](#example-7-get-the-mime-raw-contents-of-a-contact-attachment-on-a-message). |
| **event** | Formato iCal MIME. Consulte [o exemplo 8](#example-8-get-the-mime-raw-contents-of-an-event-attachment-on-a-message). |
| **message** | Formato MIME. Consulte [o exemplo 9](#example-9-get-the-mime-raw-contents-of-a-meeting-invitation-item-attachment-on-a-message). |

A tentativa de obter o `$value` de um anexo de referência retorna HTTP 405.

## <a name="permissions"></a>Permissões

Dependendo do recurso (**evento** **,** mensagem , **outlookTask** ou **postagem**) ao qual o anexo está anexado e o tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é o mínimo privilegiado necessário para chamar essa API. Para saber mais, incluindo [tomar cuidado](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) antes de escolher as permissões mais privilegiadas, pesquise as seguintes permissões em [Permissões](/graph/permissions-reference).

| Recurso com suporte | Delegada (conta corporativa ou de estudante) | Delegada (conta pessoal da Microsoft) | Aplicativo |
|:-----|:-----|:-----|:-----|
| [evento](../resources/event.md) | Calendars.Read | Calendars.Read | Calendars.Read |
| [message](../resources/message.md) | Mail.Read | Mail.Read | Mail.Read |
| [outlookTask](../resources/outlooktask.md) |  Tasks.Read | Tasks.Read | Sem suporte |
| [postagem](../resources/post.md) | Group.Read.All | Sem suporte | Sem suporte |


<!--
* If accessing attachments in group events or posts: Group.Read.All
-->

## <a name="http-request"></a>Solicitação HTTP

Esta seção mostra a sintaxe de solicitação GET HTTP para cada uma das entidades ([evento,](../resources/event.md) [mensagem,](../resources/message.md)Outlook [tarefa](../resources/outlooktask.md)e [postagem](../resources/post.md)) que suportam anexos:

- Para obter as propriedades e as relações de um anexo, especifique a ID do anexo para indexar na coleção **attachments,** anexada ao evento especificado [,](../resources/event.md)mensagem [,](../resources/message.md) [Outlook tarefa](../resources/outlooktask.md)ou instância de [postagem.](../resources/post.md)
- Se o anexo for um arquivo ou item do Outlook (contato, evento ou mensagem), você poderá obter ainda mais o conteúdo bruto do anexo anexando o segmento de caminho `/$value` à URL da solicitação.

Um anexo de um [evento](../resources/event.md):

<!-- { "blockType": "ignored" } -->

```http
GET /me/events/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/events/{id}/attachments/{id}
GET /me/events/{id}/attachments/{id}/$value
GET /users/{id | userPrincipalName}/events/{id}/attachments/{id}/$value
```

<!--
GET /groups/{id}/events/{id}/attachments/{id}
-->

Um anexo de [uma mensagem](../resources/message.md) na caixa de correio de um usuário:
<!-- { "blockType": "ignored" } -->

```http
GET /me/messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/messages/{id}/attachments/{id}
GET /me/messages/{id}/attachments/{id}/$value
GET /users/{id | userPrincipalName}/messages/{id}/attachments/{id}/$value
```

Um anexo de uma [mensagem](../resources/message.md) contida em uma [mailFolder](../resources/mailfolder.md) de nível superior na caixa de correio de um usuário:
<!-- { "blockType": "ignored" } -->

```http
GET /me/mailFolders/{id}/messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments/{id}
GET /me/mailFolders/{id}/messages/{id}/attachments/{id}/$value
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments/{id}/$value
```

Um anexo de uma [mensagem contida](../resources/message.md) em uma pasta filha de [uma mailFolder](../resources/mailfolder.md) na caixa de correio de um usuário:
<!-- { "blockType": "ignored" } -->

```http
GET /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
GET /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}/$value
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}/$value
```

O exemplo anterior mostra um nível de aninhamento, mas uma mensagem pode ser localizada em um filho de um filho e assim por diante.

Um anexo de uma [tarefa Outlook:](../resources/outlooktask.md)
<!-- { "blockType": "ignored" } -->

```http
GET /me/outlook/tasks/{id}/attachments/{id}
GET /users/{id}/outlook/tasks/{id}/attachments/{id}
GET /me/outlook/tasks/{id}/attachments/{id}/$value
GET /users/{id}/outlook/tasks/{id}/attachments/{id}/$value
```

Um anexo de uma [postagem](../resources/post.md) em [um thread](../resources/conversationthread.md) pertencente a uma [conversa](../resources/conversation.md) de um grupo:
<!-- { "blockType": "ignored" } -->

```http
GET /groups/{id}/threads/{id}/posts/{id}/attachments/{id}
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments/{id}
GET /groups/{id}/threads/{id}/posts/{id}/attachments/{id}/$value
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments/{id}/$value
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Este método também dá suporte a alguns [Parâmetros de Consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.

Use `$expand` para obter as propriedades de um anexo de item (contato, evento ou mensagem). Veja o [exemplo 3](#example-3-expand-and-get-the-properties-of-the-item-attached-to-a-message) e o [exemplo 4](#example-4-expand-and-get-the-properties-of-an-item-attached-to-a-message-including-any-attachment-to-the-item).

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome       | Tipo | Descrição|
|:-----------|:------|:----------|
| Autorização  | string  | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, o método GET retornará um `200 OK` código de resposta. 

Se você estiver obtendo as propriedades e os relacionamentos de um anexo, o corpo da resposta incluirá um objeto de [anexo](../resources/attachment.md).
As propriedades desse tipo de anexo são retornadas: [fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md) ou [referenceAttachment](../resources/referenceattachment.md).

Se você estiver obtendo o conteúdo bruto de um anexo de arquivo ou de item, o corpo da resposta incluirá o valor bruto do anexo.

## <a name="examples"></a>Exemplos

### <a name="example-1-get-the-properties-of-a-file-attachment"></a>Exemplo 1: Obter as propriedades de um anexo de arquivo

#### <a name="request"></a>Solicitação

Aqui está um exemplo da solicitação para obter as propriedades de um anexo de arquivo em uma mensagem.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_file_attachment_beta",
  "sampleKeys": ["AAMkAGUzY5QKjAAA=","AAMkAGUzY5QKjAAABEgAQAMkpJI_X-LBFgvrv1PlZYd8="]
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/messages/AAMkAGUzY5QKjAAA=/attachments/AAMkAGUzY5QKjAAABEgAQAMkpJI_X-LBFgvrv1PlZYd8=
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-file-attachment-beta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-file-attachment-beta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-file-attachment-beta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-file-attachment-beta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Resposta

Veja a seguir um exemplo da resposta. Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "name": "get_file_attachment_beta",
  "truncated": true,
  "@odata.type": "microsoft.graph.fileAttachment"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('bb8775a4-4d8c-42cf-a1d4-4d58c2bb668f')/messages('AAMkAGUzY5QKjAAA%3D')/attachments/$entity",
    "@odata.type": "#microsoft.graph.fileAttachment",
    "id": "AAMkAGUzY5QKjAAABEgAQAMkpJI_X-LBFgvrv1PlZYd8=",
    "lastModifiedDateTime": "2019-04-02T03:41:29Z",
    "name": "Draft sales invoice template.docx",
    "contentType": "application/vnd.openxmlformats-officedocument.wordprocessingml.document",
    "size": 13068,
    "isInline": false,
    "contentId": null,
    "contentLocation": null,
    "contentBytes": "UEsDBBQABgAIAAAAIQ4AAAAA"
}
```

### <a name="example-2-get-the-properties-of-an-item-attachment"></a>Exemplo 2: Obter as propriedades de um anexo de item

#### <a name="request"></a>Solicitação

O próximo exemplo mostra como obter um anexo de item em uma mensagem. As propriedades de **itemAttachment** são retornadas.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_item_attachment",
  "sampleKeys": ["AAMkADA1M-zAAA=","AAMkADA1M-CJKtzmnlcqVgqI="]
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/messages('AAMkADA1M-zAAA=')/attachments('AAMkADA1M-CJKtzmnlcqVgqI=')
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-item-attachment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-item-attachment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-item-attachment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-item-attachment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "name": "get_item_attachment",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemAttachment"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('d1a2fae9-db66-4cc9-8133-2184c77af1b8')/messages('AAMkADA1M-zAAA%3D')/attachments/$entity",
  "@odata.type":"#microsoft.graph.itemAttachment",
  "id":"AAMkADA1M-CJKtzmnlcqVgqI=",
  "lastModifiedDateTime":"2017-07-21T00:20:34Z",
  "name":"Reminder - please bring laptop",
  "contentType":null,
  "size":32005,
  "isInline":false
}
```

### <a name="example-3-expand-and-get-the-properties-of-the-item-attached-to-a-message"></a>Exemplo 3: Expandir e obter as propriedades do item anexado a uma mensagem
#### <a name="request"></a>Solicitação

O próximo exemplo mostra como usar `$expand` para obter as propriedades do item (contato, evento ou mensagem) anexado à mensagem. Neste exemplo, esse item é uma mensagem. As propriedades dessa mensagem anexadas também são retornadas.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_and_expand_item_attachment",
  "sampleKeys": ["AAMkADA1M-zAAA=","AAMkADA1M-CJKtzmnlcqVgqI="]
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/messages('AAMkADA1M-zAAA=')/attachments('AAMkADA1M-CJKtzmnlcqVgqI=')/?$expand=microsoft.graph.itemattachment/item
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-and-expand-item-attachment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-and-expand-item-attachment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-and-expand-item-attachment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-and-expand-item-attachment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "name": "get_and_expand_item_attachment",
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
    "bodyPreview": "PFA\r\n\r\nThanks,\r\nRob",
    "importance":"normal",
    "conversationId":"AAQkADA1MzMyOGI4LTlkZDctNDkzYy05M2RiLTdiN2E1NDE3MTRkOQAQAMG_NSCMBqdKrLa2EmR-lO0=",
    "conversationIndex":"AQHTAbcSwb41IIwGp0qstrYSZH+U7Q==",
    "isDeliveryReceiptRequested":false,
    "isReadReceiptRequested":false,
    "isRead":false,
    "isDraft":false,
    "webLink":"https://outlook.office365.com/owa/?ItemID=AAMkADA1M3MTRkOQAAAA%3D%3D&exvsurl=1&viewmodel=ReadMessageItem",
    "internetMessageHeaders": [ ],
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

### <a name="example-4-expand-and-get-the-properties-of-an-item-attached-to-a-message-including-any-attachment-to-the-item"></a>Exemplo 4: Expanda e obtenha as propriedades de um item anexado a uma mensagem, incluindo qualquer anexo do item
#### <a name="request"></a>Solicitação
O próximo exemplo usa a mesma solicitação do [exemplo 3](#example-3-expand-and-get-the-properties-of-the-item-attached-to-a-message) para obter as propriedades de um anexo de item em uma mensagem usando `$expand`. Nesse caso, como o item anexado também contém um anexo de arquivo, a resposta também inclui as propriedades do anexo de arquivo. 

<!-- {
  "blockType": "request",
  "name": "get_and_expand_nested_item_attachment",
  "sampleKeys": ["AAMkADA1M-zAAA=","AAMkADA1M-CJKtzmnlcqVgqI="]
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/messages('AAMkADA1M-zAAA=')/attachments('AAMkADA1M-CJKtzmnlcqVgqI=')/?$expand=microsoft.graph.itemattachment/item
```

#### <a name="response"></a>Resposta
<!-- {
  "blockType": "response",
  "name": "get_and_expand_nested_item_attachment",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemAttachment"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('d1a2fae9-db66-4cc9-8133-2184c77af1b8')/messages('AAMkADA1M-zAAA%3D')/attachments(microsoft.graph.itemAttachment/item())/$entity",
    "@odata.type": "#microsoft.graph.itemAttachment",
    "id": "AAMkADA1MCJKtzmnlcqVgqI=",
    "lastModifiedDateTime": "2021-01-06T13:28:11Z",
    "name": "Nested Message With Attachment",
    "contentType": null,
    "size": 465916,
    "isInline": false,
    "item@odata.context": "https://graph.microsoft.com/beta/$metadata#users('d1a2fae9-db66-4cc9-8133-2184c77af1b8')/messages('AAMkADA1M-zAAA%3D')/attachments('AAMkADA1M-CJKtzmnlcqVgqI%3D')/microsoft.graph.itemAttachment/item/$entity",
    "item": {
        "@odata.type": "#microsoft.graph.message",
        "id": "",
        "createdDateTime": "2021-01-06T13:28:30Z",
        "lastModifiedDateTime": "2021-01-06T13:27:40Z",
        "receivedDateTime": "2021-01-06T13:27:25Z",
        "sentDateTime": "2021-01-06T13:27:04Z",
        "hasAttachments": true,
        "internetMessageId": "<BY2PR15MB05189A084C01F466709E414F9CA40@BY2PR15MB0518.namprd15.prod.outlook.com>",
        "subject": "Nested Message With Attachment",
        "bodyPreview": "PFAThanks,Adele",
        "importance": "normal",
        "conversationId": "AAQkADg3NTY5MDg4LWMzYmQtNDQzNi05OTgwLWQyZjg2YWQwMTNkZAAQAO6hkp84oMdGm6ZBsSH72sE=",
        "conversationIndex": "AQHW5C+U7qGSnzigx0abpkGxIfvawQ==",
        "isDeliveryReceiptRequested": false,
        "isReadReceiptRequested": false,
        "isRead": true,
        "isDraft": false,
        "webLink": "https://outlook.office365.com/owa/?ItemID=AAMkADA1M3MTRkOQAAAA%3D%3D&exvsurl=1&viewmodel=ItemAttachment",
        "internetMessageHeaders": [],
        "body": {
            "contentType": "html",
            "content": "<html><head>\r\n</head>\r\n<body>\r\n</body>\r\n</html>"
        },
        "sender": {
            "emailAddress": {
                "name": "Adele Vance",
                "address": "Adele.Vance@microsoft.com"
            }
        },
        "from": {
            "emailAddress": {
                "name": "Adele Vance",
                "address": "Adele.Vance@microsoft.com"
            }
        },
        "toRecipients": [
            {
                "emailAddress": {
                    "name": "Adele Vance",
                    "address": "Adele.Vance@microsoft.com"
                }
            }
        ],
        "flag": {
            "flagStatus": "notFlagged"
        },
        "attachments@odata.context": "https://graph.microsoft.com/beta/$metadata#users('d1a2fae9-db66-4cc9-8133-2184c77af1b8')/messages('AAMkADA1M-zAAA%3D')/attachments('AAMkADA1M-CJKtzmnlcqVgqI%3D')/microsoft.graph.itemAttachment/microsoft.graph.itemAttachment/item/microsoft.graph.message/microsoft.graph.message/microsoft.graph.message/microsoft.graph.message/microsoft.graph.message/microsoft.graph.message/microsoft.graph.message/attachments",
        "attachments": [
            {
                "@odata.type": "#microsoft.graph.fileAttachment",
                "@odata.mediaContentType": "application/pdf",
                "id": "AAMkADg3NTYULmbsDYNg==",
                "lastModifiedDateTime": "2021-01-21T14:56:18Z",
                "name": "Info.pdf",
                "contentType": "application/pdf",
                "size": 417351,
                "isInline": false,
                "contentId": null,
                "contentLocation": null,
                "contentBytes": "JVBERi0xLjUNCiW1tbW1DQoxIDAgb2JqDQo8PC9UeXBlL0NhdGFsb2cvUGFnZXMgMiAwIFIvTGFuZyhlbi1JTikgL1N0cnVjdFRyZWVSb29"
            }
        ]
    }
}
```

### <a name="example-5-get-the-properties-of-a-reference-attachment"></a>Exemplo 5: Obtenha as propriedades de um anexo de referência

#### <a name="request"></a>Solicitação

Aqui está um exemplo da solicitação para obter um anexo de referência em um evento.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_reference_attachment",
  "sampleKeys": ["AAMkAGE1M88AADUv0uAAAG=","AAMkAGE1Mg72tgf7hJp0PICVGCc0g="]
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/events/AAMkAGE1M88AADUv0uAAAG=/attachments/AAMkAGE1Mg72tgf7hJp0PICVGCc0g=
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-reference-attachment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-reference-attachment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-reference-attachment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-reference-attachment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
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


### <a name="example-6-get-the-raw-contents-of-a-file-attachment-on-a-message"></a>Exemplo 6: Obtenha o conteúdo bruto de um anexo de arquivo em uma mensagem

#### <a name="request"></a>Solicitação

Aqui está um exemplo da solicitação para obter o conteúdo bruto de um arquivo do Word que foi anexado a uma mensagem.
<!-- {
  "blockType": "ignored",
  "name": "get_value_file_attachment",
  "sampleKeys": ["AAMkAGUzY5QKjAAA=","AAMkAGUzY5QKjAAABEgAQAMkpJI_X-LBFgvrv1PlZYd8="]
}-->

```http
GET https://graph.microsoft.com/beta/me/messages/AAMkAGUzY5QKjAAA=/attachments/AAMkAGUzY5QKjAAABEgAQAMkpJI_X-LBFgvrv1PlZYd8=/$value
```

#### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. O corpo da resposta real inclui os bytes brutos do anexo do arquivo, que são abreviados aqui por questões de brevidade.

<!-- {
  "blockType": "ignored",
  "name": "get_value_file_attachment",
  "truncated": true
} -->

```http
HTTP/1.1 200 OK

{Raw bytes of the file}
```


### <a name="example-7-get-the-mime-raw-contents-of-a-contact-attachment-on-a-message"></a>Exemplo 7: Obtenha o conteúdo bruto MIME de um anexo de contato em uma mensagem

#### <a name="request"></a>Solicitação

Aqui está um exemplo da solicitação para obter o conteúdo bruto de um item de contato que foi anexado a uma mensagem. 
<!-- {
  "blockType": "ignored",
  "name": "get_value_contact_attachment",
  "sampleKeys": ["AAMkADI5MAAGjk2PxAAA=","AAMkADI5MAAGjk2PxAAABEgAQACEJqrbJZBNIlr3pGFvd9K8="]
}-->

```http
GET https://graph.microsoft.com/beta/me/messages/AAMkADI5MAAGjk2PxAAA=/attachments/AAMkADI5MAAGjk2PxAAABEgAQACEJqrbJZBNIlr3pGFvd9K8=/$value
```

#### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. 

<!-- {
  "blockType": "ignored",
  "name": "get_value_contact_attachment",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK

BEGIN:VCARD
PROFILE:VCARD
VERSION:3.0
MAILER:Microsoft Exchange
PRODID:Microsoft Exchange
FN:Alex Wilbur
N:Wilbur;Alex;;;
NOTE:Sunday\, June 10\, 2012 5:44 PM:\nGutter\, window cleaning\, pressure 
 washing\, roof debris blowing\n
ORG:Contoso;
CLASS:PUBLIC
ADR;TYPE=WORK,PREF:;;4567 Main St;Buffalo;NY;98052;United States of America
LABEL;TYPE=WORK,PREF:4567 Main St\nBuffalo\, NY 98052
ADR;TYPE=HOME:;;;;;;
ADR;TYPE=POSTAL:;;;;;;
TEL;TYPE=WORK:(425) 555-0100
TITLE:
X-MS-IMADDRESS:
REV;VALUE=DATE-TIME:2019-04-09T02:13:31,161Z
END:VCARD
```


### <a name="example-8-get-the-mime-raw-contents-of-an-event-attachment-on-a-message"></a>Exemplo 8: Obtenha o conteúdo bruto MIME de um anexo de evento em uma mensagem

#### <a name="request"></a>Solicitação

Aqui está um exemplo da solicitação para obter o conteúdo bruto de um evento que foi anexado a uma mensagem. 
<!-- {
  "blockType": "ignored",
  "name": "get_value_event_attachment",
  "sampleKeys": ["AAMkADVIOAAA=","AAMkADVIOAAABEgAQACvkutl6c4FMifPyS6NvXsM="]
}-->

```http
GET https://graph.microsoft.com/beta/me/messages/AAMkADVIOAAA=/attachments/AAMkADVIOAAABEgAQACvkutl6c4FMifPyS6NvXsM=/$value
```

#### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. 

<!-- {
  "blockType": "ignored",
  "name": "get_value_event_attachment",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK

BEGIN:VCALENDAR
METHOD:PUBLISH
PRODID:Microsoft Exchange Server 2010
VERSION:2.0
BEGIN:VTIMEZONE
TZID:Pacific Standard Time
BEGIN:STANDARD
DTSTART:16010101T020000
TZOFFSETFROM:-0700
TZOFFSETTO:-0800
RRULE:FREQ=YEARLY;INTERVAL=1;BYDAY=1SU;BYMONTH=11
END:STANDARD
BEGIN:DAYLIGHT
DTSTART:16010101T020000
TZOFFSETFROM:-0800
TZOFFSETTO:-0700
RRULE:FREQ=YEARLY;INTERVAL=1;BYDAY=2SU;BYMONTH=3
END:DAYLIGHT
END:VTIMEZONE
BEGIN:VEVENT
ORGANIZER;CN=Adele Vance:MAILTO:adelev@contoso.com
ATTENDEE;ROLE=REQ-PARTICIPANT;PARTSTAT=NEEDS-ACTION;RSVP=TRUE;CN=Adele Vance:MAILTO:adelev@contoso.com
DESCRIPTION;LANGUAGE=en-US:\n
UID:040000008200
SUMMARY;LANGUAGE=en-US:Review Megan's docs
DTSTART;TZID=Pacific Standard Time:20190409T140000
DTEND;TZID=Pacific Standard Time:20190409T160000
CLASS:PUBLIC
PRIORITY:5
DTSTAMP:20190409T211833Z
TRANSP:OPAQUE
STATUS:CONFIRMED
SEQUENCE:0
LOCATION;LANGUAGE=en-US:
X-MICROSOFT-CDO-APPT-SEQUENCE:0
X-MICROSOFT-CDO-OWNERAPPTID:0
X-MICROSOFT-CDO-BUSYSTATUS:BUSY
X-MICROSOFT-CDO-INTENDEDSTATUS:BUSY
X-MICROSOFT-CDO-ALLDAYEVENT:FALSE
X-MICROSOFT-CDO-IMPORTANCE:1
X-MICROSOFT-CDO-INSTTYPE:0
X-MICROSOFT-DONOTFORWARDMEETING:FALSE
X-MICROSOFT-DISALLOW-COUNTER:FALSE
X-MICROSOFT-LOCATIONS:[]
BEGIN:VALARM
DESCRIPTION:REMINDER
TRIGGER;RELATED=START:-PT15M
ACTION:DISPLAY
END:VALARM
END:VEVENT
END:VCALENDAR
```


### <a name="example-9-get-the-mime-raw-contents-of-a-meeting-invitation-item-attachment-on-a-message"></a>Exemplo 9: Obtenha o conteúdo bruto MIME de um anexo de item de convite de reunião em uma mensagem

#### <a name="request"></a>Solicitação

Aqui está um exemplo da solicitação para obter o conteúdo bruto de um convite para reunião (do tipo [eventMessage](../resources/eventmessage.md)) que foi anexado a uma mensagem. A entidade **eventMessage** é baseada no tipo de **mensagem**.
<!-- {
  "blockType": "ignored",
  "name": "get_value_message_attachment",
  "sampleKeys": ["AAMkAGUzY5QKiAAA=","AAMkAGUzY5QKiAAABEgAQAK8ktgiIO19OqkvUZAqLmyQ="]
}-->

```http
GET https://graph.microsoft.com/beta/me/messages/AAMkAGUzY5QKiAAA=/attachments/AAMkAGUzY5QKiAAABEgAQAK8ktgiIO19OqkvUZAqLmyQ=/$value
```

#### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. 

O corpo da resposta inclui o anexo **eventMessage** no formato MIME. O corpo do **eventMessage** é truncado por questões de brevidade. O corpo completo da mensagem é retornado de uma chamada real.

<!-- {
  "blockType": "ignored",
  "name": "get_value_message_attachment",
  "truncated": true
} -->

```http
HTTP/1.1 200 OK

From: Megan Bowen <MeganB@contoso.OnMicrosoft.com>
To: Adele Vance <AdeleV@contoso.OnMicrosoft.com>
Subject: Let's go for lunch
Thread-Topic: Let's go for lunch
Thread-Index: AdTPqxOmg4AXoJV960a1j5NrJCHYjA==
X-MS-Exchange-MessageSentRepresentingType: 1
Date: Thu, 28 Feb 2019 21:17:58 +0000
Message-ID:
    <CY4PR2201MB1046E9C83FC42478EF4EE283C9750@CY4PR2201MB1046.namprd22.prod.outlook.com>
Content-Language: en-US
X-MS-Has-Attach:
X-MS-Exchange-Organization-SCL: -1
X-MS-TNEF-Correlator:
X-MS-Exchange-Organization-RecordReviewCfmType: 0
Content-Type: multipart/alternative;
    boundary="_000_CY4PR2201MB1046E9C83FC42478EF4EE283C9750CY4PR2201MB1046_"
MIME-Version: 1.0

--_000_CY4PR2201MB1046E9C83FC42478EF4EE283C9750CY4PR2201MB1046_
Content-Type: text/plain; charset="us-ascii"

Does mid month work for you?

--_000_CY4PR2201MB1046E9C83FC42478EF4EE283C9750CY4PR2201MB1046_
Content-Type: text/html; charset="us-ascii"

<html>
<head>
<meta http-equiv="Content-Type" content="text/html; charset=us-ascii">
</head>
<body>
Does mid month work for you?
</body>
</html>

--_000_CY4PR2201MB1046E9C83FC42478EF4EE283C9750CY4PR2201MB1046_
Content-Type: text/calendar; charset="utf-8"; method=REQUEST
Content-Transfer-Encoding: base64

QkVHSU46VkNBTEVOREFSDQpNRVRIT0Q6UkVRVUVTVA0KUFJPRElEOk1pY3Jvc29mdCBFeGNoYW5n


--_000_CY4PR2201MB1046E9C83FC42478EF4EE283C9750CY4PR2201MB1046_--
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
