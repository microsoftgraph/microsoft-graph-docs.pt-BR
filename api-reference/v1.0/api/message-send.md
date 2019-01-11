---
title: 'message: send'
description: Envie uma mensagem na pasta rascunho. A mensagem de rascunho pode ser um rascunho da nova mensagem, rascunho de responder, responder a todos com rascunho, ou
localization_priority: Priority
ms.openlocfilehash: cd98c4965f7eee3e53fc24bad551a1b14e8c7521
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27867442"
---
# <a name="message-send"></a>message: send

Envie uma mensagem na pasta de rascunho. A mensagem de rascunho pode ser um rascunho de mensagem nova, rascunho de resposta, rascunho de resposta a todos ou rascunho de encaminhamento. A mensagem é salva na pasta Itens Enviados.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

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
| Tamanho do conteúdo | number | 0. necessária. |

## <a name="request-body"></a>Corpo da solicitação

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.

## <a name="example"></a>Exemplo

O exemplo a seguir mostra como chamar essa API.

##### <a name="request"></a>Solicitação

Este é um exemplo da solicitação.
<!-- {
  "blockType": "request",
  "name": "message_send"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/send
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message: send",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
