---
title: tipo de recurso dicas de texto
description: 'Mensagens inFormativas sobre um destinatário, que são exibidas aos usuários enquanto eles compõem uma mensagem. Por exemplo, uma mensagem de ausência temporária '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 11e64c09a90d130b7656d4e87770e6df3fb67408
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562599"
---
# <a name="mailtips-resource-type"></a>tipo de recurso dicas de texto

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Mensagens inFormativas sobre um destinatário, que são exibidas aos usuários enquanto eles compõem uma mensagem. Por exemplo, uma mensagem de ausência temporária como uma resposta automática para um destinatário de mensagem.


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
| automaticReplies | [automaticRepliesMailTips](../resources/automaticrepliesmailtips.md) | Dicas de email para resposta automática se tiver sido configurada pelo destinatário. |
| customMailTip | String | Uma dica de email personalizada que pode ser definida na caixa de correio do destinatário. |
| deliveryRestricted| Booliano | Se a caixa de correio do destinatário é restrita, por exemplo, aceitando mensagens de apenas uma lista predefinida de remetentes, rejeitando mensagens de uma lista predefinida de remetentes ou aceitando mensagens de somente remetentes autenticados. |
| emailAddress | [emailAddress](../resources/emailaddress.md) | O endereço de email do destinatário para o qual obter dicas de email. |
| erro | [mailTipsError](../resources/mailtipserror.md) | Erros que ocorrem durante a [](../api/user-getmailtips.md) ação comdicas de as. |
| externalMemberCount | Int32 | O número de membros externos se o destinatário for uma lista de distribuição. |
| isModeradod |Booliano  | Se o envio de mensagens para o destinatário requer aprovação. Por exemplo, se o destinatário for uma lista de distribuição grande e um moderador tiver sido configurado para aprovar as mensagens enviadas para essa lista de distribuição ou se o envio de mensagens a um destinatário exigir a aprovação do gerente do destinatário. |
| mailboxFull | Booliano | O status completo da caixa de correio do destinatário. |
| maxMessageSize | Int32 | O tamanho máximo da mensagem que foi configurada para a organização ou caixa de correio do destinatário. |
| recipientScope | String | O escopo do destinatário. Os valores possíveis são: `none`, `internal`, `external`, `externalPartner`, `externalNonParther`. Por exemplo, um administrador pode definir outra organização como "parceiro". O escopo será útil se um administrador quiser que determinadas dicas de usuários fiquem acessíveis para determinados escopos. Também é útil para os remetentes informar que a mensagem pode sair da organização, ajudando-os a tomar as decisões corretas sobre o texto, o Tom e o conteúdo.|
| recipientSuggestions | Coleção [recipient](../resources/recipient.md) | Os destinatários sugeridos com base em contextos anteriores, onde aparecem na mesma mensagem. |
| totalMemberCount | Int32 | O número de membros se o destinatário for uma lista de distribuição. |

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
<!--
{
  "type": "#page.annotation",
  "description": "mailtips resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/mailtips.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
