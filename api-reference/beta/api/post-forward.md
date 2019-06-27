---
title: 'post: forward'
description: 'Encaminhe uma postagem para um destinatário. Você pode especificar a conversa primária e o thread na solicitação, '
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: cf8d8c7759eec6f2429d16b791480ebcf531145c
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35264250"
---
# <a name="post-forward"></a>post: forward

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Encaminhe uma postagem para um destinatário. Você pode especificar a conversa pai e o thread na solicitação ou pode especificar apenas o thread pai, sem a conversa pai. 

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Group.ReadWrite.All    |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | Group.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads/{id}/posts/{id}/forward
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/forward

```
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Cabeçalho       | Valor |
|:---------------|:--------|
| Autorização  | {token} de portador. Obrigatório.  |

## <a name="request-body"></a>Corpo da solicitação
Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.

| Parâmetro    | Tipo   |Descrição|
|:---------------|:--------|:----------|
|comment|Cadeia de caracteres|Comentário opcional que é encaminhado com a postagem.|
|toRecipients|Coleção [recipient](../resources/recipient.md)|Os destinatários aos quais os threads são encaminhados.|

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.

## <a name="example"></a>Exemplo
Eis um exemplo de como chamar esta API.
##### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
<!-- {
  "blockType": "request",
  "name": "post_forward"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/threads/{id}/posts/{id}/forward
Content-type: application/json
Content-length: 166

{
  "comment": "comment-value",
  "toRecipients": [
    {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    }
  ]
}
```

##### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta.
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```
#### <a name="sdk-sample-code"></a>Código de exemplo do SDK
# <a name="ctabcs"></a>[C#](#tab/cs)
[!INCLUDE [sample-code](../includes/post_forward-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/post_forward-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[Objetivo-C](#tab/objective-c)
[!INCLUDE [sample-code](../includes/post_forward-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "post: forward",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/post-forward.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/post-forward.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/post-forward.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
