---
title: 'message: send'
description: Envie uma mensagem de rascunho existente.
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: ea24ae69c3888e31124df758bc22199bde1048ea
ms.sourcegitcommit: cec76c5a58b359d79df764c849c8b459349b3b52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2021
ms.locfileid: "52645518"
---
# <a name="message-send"></a>message: send

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Envie uma mensagem de rascunho existente. 

A mensagem de rascunho pode ser um novo rascunho de [mensagem,](../api/user-post-messages.md)rascunho de [resposta,](../api/message-createreply.md)rascunho de [resposta-tudo](../api/message-createreplyall.md)ou um [rascunho de encaminhamento.](../api/message-createforward.md) 

Este método salva a mensagem na pasta **Itens** Enviados.

Como alternativa, [envie uma nova mensagem](../api/user-sendmail.md) em uma única operação.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é necessária para chamar essa API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Mail.Send    |
|Delegado (conta pessoal da Microsoft) | Mail.Send    |
|Aplicativo | Mail.Send |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/send
POST /users/{id | userPrincipalName}/messages/{id}/send
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome       | Tipo | Descrição|
|:---------------|:--------|:----------|
| Autorização  | string  | {token} de portador. Obrigatório. |
| Content-Length | number | 0. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação
Como esse método envia uma mensagem de rascunho já existente, não é necessário especificar um corpo de solicitação.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.

## <a name="examples"></a>Exemplos
### <a name="example-1-send-an-existing-draft-message"></a>Exemplo 1: Enviar uma mensagem de rascunho existente

Eis um exemplo de como chamar esta API.

##### <a name="request"></a>Solicitação

Este é um exemplo da solicitação.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "message_send"
}-->

```http
POST https://graph.microsoft.com/beta/me/messages/{id}/send
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-send-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-send-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-send-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-send-java-snippets.md)]
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "message: send",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
