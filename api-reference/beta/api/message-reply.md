---
title: 'message: reply'
description: Responder ao remetente de uma mensagem usando o formato JSON ou MIME.
ms.localizationpriority: medium
author: abheek-das
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: a408b1309392520ba5be6b2d0040ed3e2d5b0a6d
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61004756"
---
# <a name="message-reply"></a>message: reply

Namespace: microsoft.graph.

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Responder ao remetente de uma mensagem [usando](../resources/message.md) o formato JSON ou MIME.

Ao usar o formato JSON:
- Especifique um comentário ou **a propriedade body** do `message` parâmetro. Especificar ambos retornará um erro HTTP 400 - Solicitação incorreta.
- Se a mensagem original especificar um destinatário na propriedade **replyTo,** por Formato de Mensagem da Internet ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), envie a resposta aos destinatários em **replyTo** e não ao destinatário na propriedade **from.**

Ao utilizar o formato MIME:
- Fornecer os [cabeçalhos de mensagem da Internet](https://tools.ietf.org/html/rfc2076) e o [conteúdo MIME](https://tools.ietf.org/html/rfc2045) aplicáveis, todos codificados no formato **base64** no corpo da solicitação.
- Adicionar quaisquer anexos e propriedades S/MIME ao conteúdo MIME.

Este método salva a mensagem na pasta **Itens Enviados**.

Como alternativa, [crie um rascunho para responder a uma mensagem](../api/message-createreply.md)e [envie-a](../api/message-send.md) mais tarde.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, consulte [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Mail.Send    |
|Delegado (conta pessoal da Microsoft) | Mail.Send    |
|Aplicativo | Mail.Send |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/reply
POST /users/{id | userPrincipalName}/messages/{id}/reply
POST /me/mailFolders/{id}/messages/{id}/reply
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/reply
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome       | Tipo | Descrição|
|:---------------|:--------|:----------|
| Autorização  | string  | Portador {token}. Obrigatório |
| Content-Type | string  | Natureza dos dados no corpo de uma entidade. Obrigatório <br/> Usar `application/json` para um objeto JSON e para conteúdo `text/plain` MIME |

## <a name="request-body"></a>Corpo da solicitação
Ao usar o formato JSON, inclua um objeto JSON com os seguintes parâmetros.

| Parâmetro    | Tipo   |Descrição|
|:---------------|:--------|:----------|
|comment|String|Um comentário a incluir. Não pode ficar vazio.|
|mensagem|[message](../resources/message.md) | Quaisquer propriedades graváveis ​​a serem atualizadas na mensagem de resposta.|

Ao especificar o corpo no formato MIME, forneça o conteúdo MIME com os headers de mensagem da Internet aplicáveis, todos codificados no **formato base64** no corpo da solicitação. Este método usa o remetente da mensagem original como destinatário.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.

Se o corpo da solicitação incluir conteúdo MIME malformado, este método retornará `400 Bad request` e a seguinte mensagem de erro: "Cadeia de caracteres base64 inválida para o conteúdo MIME".

## <a name="examples"></a>Exemplos
### <a name="example-1-reply-to-a-message-in-json-format"></a>Exemplo 1: Responder a uma mensagem no formato JSON
O exemplo a seguir inclui um comentário e adiciona um destinatário à mensagem de resposta.
##### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.

# <a name="http"></a>[HTTP](#tab/http)

<!-- {
  "blockType": "request",
  "name": "message_reply_beta",
  "sampleKeys": ["AAMkADA1MTAAAAqldOAAA="]
}-->

```http
POST https://graph.microsoft.com/beta/me/messages/AAMkADA1MTAAAAqldOAAA=/reply
Content-Type: application/json

{
  "message":{  
    "toRecipients":[
      {
        "emailAddress": {
          "address":"samanthab@contoso.onmicrosoft.com",
          "name":"Samantha Booth"
        }
      },
      {
        "emailAddress":{
          "address":"randiw@contoso.onmicrosoft.com",
          "name":"Randi Welch"
        }
      }
     ]
  },
  "comment": "Samantha, Randi, would you name the group please?" 
}

```

# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-reply-beta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-reply-beta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-reply-beta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-reply-beta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/message-reply-beta-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta.

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 202 Accepted
```

### <a name="example-2-reply-to-a-message-in-mime-format"></a>Exemplo 2: Responder a uma mensagem no formato MIME
##### <a name="request"></a>Solicitação

<!-- {
  "blockType": "ignored",
  "name": "message_reply_mime_beta"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/messages/AAMkADA1MTAAAAqldOAAA=/reply
Content-Type: text/plain

UmVjZWl2ZWQ6IGZyb20gY29udG9zby5jb20gKDEwLjE5NC4yNDEuMTk3KSBieSAKY29udG9zby5jb20gKDEwLjE5NC4yNDEuMTk3KSB3aXRoIE1pY3Jvc29mdCAKU01UUCBTZXJ2ZXIgKHZlcnNpb249VExTMV8yLCAKY2lwaGVyPVRMU19FQ0RIRV9SU0FfV0lUSF9BRVNfMjU2X0NCQ19TSEEzODRfUDI1NikgaW

```

##### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta.

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 202 Accepted
```

Se o corpo da solicitação incluir conteúdo MIME malformado, este método retornará a seguinte mensagem de erro.

<!-- { "blockType": "ignored" } -->

```http
HTTP/1.1 400 Bad Request
Content-type: application/json

{
    "error": {
        "code": "ErrorMimeContentInvalidBase64String",
        "message": "Invalid base64 string for MIME content."
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "message: reply",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
