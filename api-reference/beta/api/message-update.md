---
title: Atualizar mensagem
description: Atualizar as propriedades do objeto mensagem.
author: abheek-das
ms.localizationpriority: medium
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 705134b7e85e27b7a36ce30f8d76972b2338cdb6
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61020674"
---
# <a name="update-message"></a>Atualizar mensagem

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualizar as propriedades de um objeto mensagem.
## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Mail.ReadWrite    |
|Delegado (conta pessoal da Microsoft) | Mail.ReadWrite    |
|Aplicativo | Mail.ReadWrite |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/messages/{id}
PATCH /users/{id | userPrincipalName}/messages/{id}
PATCH /me/mailFolders/{id}/messages/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome       | Tipo | Descrição|
|:-----------|:------|:----------|
| Autorização  | string  | {token} de portador. Obrigatório. |
| Content-Type | string  | Natureza dos dados no corpo de uma entidade. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação
No corpo de solicitação, forneça os valores para os campos relevantes que devem ser atualizados. As propriedades existentes que não estão incluídas no corpo da solicitação manterão seus valores anteriores ou serão recalculadas com base nas mudanças de outros valores de propriedade. Para obter o melhor desempenho, você não deve incluir valores existentes que não tenham sido alterados. As seguintes propriedades podem ser atualizadas.

| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|bccRecipients|Destinatário|Os destinatários Cco da mensagem. |
|corpo|ItemBody|O corpo da mensagem. Atualizável somente se isDraft = true.|
|Categorias|String collection|As categorias associadas à mensagem.|
|ccRecipients|Coleção Recipient|Os destinatários Cc da mensagem. |
|sinalizador|[followupFlag](../resources/followupflag.md)|O valor do sinalizador que indica o status, a data de início, a data de conclusão ou a data de finalização da mensagem.|
|from|Destinatário|O proprietário da caixa de correio e o remetente da mensagem. Devem corresponder à caixa de correio real que foi usada. |
|importância|Cadeia de caracteres|A importância da mensagem. Os valores possíveis são: `Low`, `Normal`, `High`.|
|inferenceClassification | String | A classificação da mensagem para o usuário, com base na relevância deduzida ou na importância, ou em uma substituição explícita. Os valores possíveis são: `focused` ou `other`. |
|internetMessageId |String |O ID da mensagem no formato especificado por [RFC2822](https://www.ietf.org/rfc/rfc2822.txt). Atualizável apenas se isDraft = true.|
|isDeliveryReceiptRequested|Boolean|Indica se uma confirmação de leitura foi solicitada para a mensagem.|
|isRead|Boolean|Indica se a mensagem foi lida.|
|isReadReceiptRequested|Boolean|Indica se uma confirmação de leitura foi solicitada para a mensagem.|
|multiValueExtendedProperties|Coleção [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md)| A coleção de propriedades estendidas de vários valores definidas para a mensagem. Anulável.|
|replyTo|Coleção Recipient|Os endereços de email para usar ao responder. Atualizável somente se isDraft = true.|
|remetente|Destinatário|A conta que é realmente usada para gerar a mensagem. Atualizável ao enviar uma mensagem de uma [caixa de correio compartilhada](/exchange/collaboration/shared-mailboxes/shared-mailboxes), ou enviar uma mensagem como um [delegado](https://support.office.com/article/allow-someone-else-to-manage-your-mail-and-calendar-41c40c04-3bd1-4d22-963a-28eafec25926). De qualquer forma, o valor deve corresponder à caixa de correio real que foi usada.|
|singleValueExtendedProperties|Coleção [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md)| A coleção de propriedades estendidas de valor único definidas para a mensagem. Anulável.|
|Assunto|String|O assunto da mensagem. Atualizável somente se isDraft = true.|
|toRecipients|Coleção Recipient|Os destinatários Para da mensagem. |

Como o recurso **message** dá suporte a [extensions](/graph/extensibility-overview), você pode usar a operação `PATCH` para adicionar, atualizar ou excluir seus próprios dados específicos do aplicativo nas propriedades personalizadas de uma extensão em uma instância de **message** existente.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta `200 OK` e o objeto [message](../resources/message.md) atualizado no corpo da resposta.
## <a name="example"></a>Exemplo
##### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_message"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/messages/{id}
Content-type: application/json

{
  "subject": "subject-value",
  "body": {
    "contentType": "",
    "content": "content-value"
  },
  "inferenceClassification": "other"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-message-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-message-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a>Resposta
Aqui está um exemplo da resposta. Observação: o objeto de resposta mostrado aqui pode ser reduzido para facilitar a leitura.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "receivedDateTime": "2016-10-19T10:37:00Z",
  "sentDateTime": "2016-10-19T10:37:00Z",
  "hasAttachments": true,
  "subject": "subject-value",
  "body": {
    "contentType": "",
    "content": "content-value"
  },
  "bodyPreview": "bodyPreview-value",
  "inferenceClassification": "other"
}
```

## <a name="see-also"></a>Confira também

- [Adicionar dados personalizados a recursos usando extensões](/graph/extensibility-overview)
- [Adicionar dados personalizados aos usuários usando extensões abertas (visualização)](/graph/extensibility-open-users)
- [Adicionar dados personalizados a grupos usando extensões do esquema (visualização)](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update message",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


