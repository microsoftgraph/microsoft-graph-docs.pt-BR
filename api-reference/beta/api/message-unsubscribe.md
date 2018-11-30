---
title: 'mensagem: Cancelar a assinatura'
description: Envia uma solicitação de e-mail em nome do usuário conectado para cancelar a assinatura de uma lista de distribuição de e-mail. Usa as informações do cabeçalho `List-Unsubscribe`.
ms.openlocfilehash: b4f72a0b629fb59074acbbd58f09a3c16118cc8c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037365"
---
# <a name="message-unsubscribe"></a>mensagem: Cancelar a assinatura

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Envia uma solicitação de e-mail em nome do usuário conectado para cancelar a assinatura de uma lista de distribuição de e-mail. Usa as informações do cabeçalho `List-Unsubscribe`.

Remetentes de mensagens podem usar listas de endereçamento de forma amigável, incluindo uma opção para destinatários para rejeitar. Eles podem fazer isso, especificando o `List-Unsubscribe` cabeçalho em cada mensagem seguindo [RFC-2369](https://www.faqs.org/rfcs/rfc2369.html).

**Observação** Em particular, para a ação **Cancelar** funcione, o remetente deve especificar `mailto:` e não baseado em URL cancelar a assinatura de informações.

A definição desse cabeçalho seria também definir a propriedade de **unsubscribeEnabled** da instância da [mensagem](../resources/message.md) para `true`e a propriedade **unsubscribeData** para os dados de cabeçalho.

Se a propriedade **unsubscribeEnabled** de uma mensagem é `true`, você pode usar a ação **Cancelar** para cancelar o usuário de mensagens futuras semelhantes como gerenciado pelo remetente da mensagem.

Uma ação bem-sucedida **Cancelar** move a mensagem para a pasta **Itens excluídos** . A exclusão do usuário dos destinatários de futuros e-mails é gerenciada pelo remetente.

## <a name="permissions"></a>Permissions
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Mail.Send    |
|Delegado (conta pessoal da Microsoft) | Mail.Send    |
|Aplicativo | Mail.Send |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/messages/{id}/unsubscribe
```
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome       | Tipo | Descrição|
|:---------------|:--------|:----------|
| Autorização  | string  | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.

## <a name="example"></a>Exemplo
Eis um exemplo de como chamar esta API.
##### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
<!-- {
  "blockType": "request",
  "name": "message_unsubscribe"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages/{id}/unsubscribe
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
  "description": "message: unsubscribe",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
