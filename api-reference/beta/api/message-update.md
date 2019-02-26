---
title: Atualizar mensagem
description: Atualizar as propriedades do objeto message.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 4b3c54e85c96524305fdba32525e277dd15508ed
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30142816"
---
# <a name="update-message"></a>Atualizar mensagem

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualiza as propriedades de um objeto Message.
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
No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações em outros valores de propriedade. Para obter o melhor desempenho, não inclua valores existentes que não foram alterados. As propriedades a seguir podem ser atualizadas.

| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|bccRecipients|Recipient|Os destinatários Cco da mensagem. |
|corpo|ItemBody|O corpo da mensagem. Atualizável somente se isDraft = true.|
|categories|Coleção de cadeias de caracteres|As categorias associadas à mensagem.|
|ccRecipients|Coleção Recipient|Os destinatários CC da mensagem. |
|flag|[followupFlag](../resources/followupflag.md)|O valor do sinalizador que indica o status, a data de início, a data de conclusão ou a data de finalização da mensagem.|
|from|Recipient|O proprietário da caixa de correio e o remetente da mensagem. Deve corresponder à caixa de correio real usada. |
|importance|String|A importância da mensagem. Os valores possíveis são: `Low`, `Normal` e `High`.|
|inferenceClassification | String | A classificação da mensagem para o usuário, com base na relevância deduzida ou na importância, ou em uma substituição explícita. Os valores possíveis são: `focused` ou `other`. |
|internetMessageId |String |A ID da mensagem no formato especificado por [RFC2822](https://www.ietf.org/rfc/rfc2822.txt). Atualizável somente se isDraft = true.|
|isDeliveryReceiptRequested|Boolean|Indica se uma confirmação de leitura foi solicitada para a mensagem.|
|isRead|Boolean|Indica se a mensagem foi lida.|
|isReadReceiptRequested|Boolean|Indica se uma confirmação de leitura foi solicitada para a mensagem.|
|multiValueExtendedProperties|Coleção [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md)| A coleção de propriedades estendidas de vários valores definidas para a mensagem. Anulável.|
|replyTo|Coleção Recipient|Os endereços de email a serem usados ao responder. Atualizável somente se isDraft = true.|
|sender|Destinatário|A conta que é realmente usada para gerar a mensagem. Atualizável ao enviar uma mensagem de uma [caixa de correio compartilhada](https://docs.microsoft.com/en-us/exchange/collaboration/shared-mailboxes/shared-mailboxes)ou enviar uma mensagem como um [Representante](https://support.office.com/en-us/article/allow-someone-else-to-manage-your-mail-and-calendar-41c40c04-3bd1-4d22-963a-28eafec25926). De qualquer forma, o valor deve corresponder à caixa de correio real que foi usada.|
|singleValueExtendedProperties|Coleção [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md)| A coleção de propriedades estendidas de valor único definidas para a mensagem. Anulável.|
|subject|String|O assunto da mensagem. Atualizável somente se isDraft = true.|
|toRecipients|Coleção Recipient|Os destinatários para para a mensagem. |

Como o recurso **message** dá suporte a [extensions](/graph/extensibility-overview), você pode usar a operação `PATCH` para adicionar, atualizar ou excluir seus próprios dados específicos do aplicativo nas propriedades personalizadas de uma extensão em uma instância de **message** existente.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta `200 OK` e o objeto [message](../resources/message.md) atualizado no corpo da resposta.
## <a name="example"></a>Exemplo
##### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
<!-- {
  "blockType": "request",
  "name": "update_message"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/messages/{id}
Content-type: application/json
Content-length: 248

{
  "subject": "subject-value",
  "body": {
    "contentType": "",
    "content": "content-value"
  },
  "inferenceClassification": "other"
}
```
##### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 248

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
    "Error: /api-reference/beta/api/message-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
