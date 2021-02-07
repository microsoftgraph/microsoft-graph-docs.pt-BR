---
title: tipo de recurso mailTips
description: 'Mensagens informativas sobre um destinatário, que são exibidas aos usuários enquanto eles compõem uma mensagem. Por exemplo, uma mensagem de fora do escritório '
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 3c72e7a81e06b267f4a212e3d56ae8607866eed2
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131530"
---
# <a name="mailtips-resource-type"></a>tipo de recurso mailTips

Namespace: microsoft.graph

Mensagens informativas sobre um destinatário, que são exibidas aos usuários enquanto eles compõem uma mensagem. Por exemplo, uma mensagem de fora do escritório como uma resposta automática para um destinatário da mensagem.


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
| automaticReplies | [automaticRepliesMailTips](../resources/automaticrepliesmailtips.md) | Dicas de email para resposta automática se ela tiver sido configurada pelo destinatário. |
| customMailTip | String | Uma dica de email personalizada que pode ser definida na caixa de correio do destinatário. |
| deliveryRestricted| Booliano | Se a caixa de correio do destinatário é restrita, por exemplo, aceitando mensagens de apenas uma lista predefinida de destinatários, rejeitando mensagens de uma lista predefinida de destinatários ou aceitando mensagens apenas de destinatários autenticados. |
| emailAddress | [emailAddress](../resources/emailaddress.md) | O endereço de email do destinatário para o que obter dicas de email. |
| erro | [mailTipsError](../resources/mailtipserror.md) | Erros que ocorrem durante a [ação getMailTips.](../api/user-getmailtips.md) |
| externalMemberCount | Int32 | O número de membros externos se o destinatário for uma lista de distribuição. |
| isModerated |Booliano  | Se o envio de mensagens para o destinatário requer aprovação. Por exemplo, se o destinatário for uma lista de distribuição grande e um moderador tiver sido definido para aprovar mensagens enviadas a essa lista de distribuição, ou se o envio de mensagens para um destinatário exigir aprovação do gerente do destinatário. |
| mailboxFull | Booliano | O status completo da caixa de correio do destinatário. |
| maxMessageSize | Int32 | O tamanho máximo da mensagem que foi configurado para a organização ou a caixa de correio do destinatário. |
| recipientScope | recipientScopeType | O escopo do destinatário. Os valores possíveis são: `none`, `internal`, `external`, `externalPartner`, `externalNonParther`. Por exemplo, um administrador pode definir outra organização como seu "parceiro". O escopo é útil se um administrador quiser que determinadas dicas de email sejam acessíveis a determinados escopos. Também é útil para os envios informá-los de que suas mensagens podem sair da organização, ajudando-os a tomar as decisões corretas sobre texto, tom e conteúdo.|
| recipientSuggestions | Coleção [recipient](../resources/recipient.md) | Destinatários sugeridos com base em contextos anteriores em que aparecem na mesma mensagem. |
| totalMemberCount | Int32 | O número de membros se o destinatário for uma lista de distribuição. |

### <a name="recipientscopetype-values"></a>Valores de recipientScopeType

| Valor
|:-------------------------
| nenhum
| interno
| externo
| externalPartner
| externalNonPartner


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "automaticReplies",
    "customMailTip",
    "deliveryRestricted",
    "emailAddress",
    "error",
    "externalMemberCount",
    "isModerated",
    "mailboxFull",
    "maxMessageSize",
    "recipientScope",
    "recipientSuggestions",
    "totalMemberCount"
  ],
  "@odata.type": "microsoft.graph.mailTips"
}-->

```json
{
  "automaticReplies": {"@odata.type": "microsoft.graph.automaticRepliesMailTips"},
  "customMailTip": "string",
  "deliveryRestricted": "boolean",
  "emailAddress": {"@odata.type": "microsoft.graph.emailAddress"},
  "error": {"@odata.type": "microsoft.graph.mailTipsError"},
  "externalMemberCount": 1024,
  "isModerated": "boolean",
  "mailboxFull": "boolean",
  "maxMessageSize": 1024,
  "recipientScope": "string",
  "recipientSuggestions": [{"@odata.type": "microsoft.graph.recipient"}],
  "totalMemberCount": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mailtips resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

