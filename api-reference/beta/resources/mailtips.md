---
title: tipo de recurso de dicas de email
description: 'Mensagens informativas sobre um destinatário, que são exibidas aos usuários enquanto eles estão redigindo uma mensagem. Por exemplo, uma mensagem de ausência temporária '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 11e64c09a90d130b7656d4e87770e6df3fb67408
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508409"
---
# <a name="mailtips-resource-type"></a>tipo de recurso de dicas de email

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Mensagens informativas sobre um destinatário, que são exibidas aos usuários enquanto eles estão redigindo uma mensagem. Por exemplo, uma mensagem de ausência temporária como uma resposta automática para um destinatário de mensagem.


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
| automaticReplies | [automaticRepliesMailTips](../resources/automaticrepliesmailtips.md) | Dicas para a resposta automática de email se ele foi configurado pelo destinatário. |
| CustomMailTip | String | Uma dica de email personalizado que pode ser definida na caixa de correio do destinatário. |
| DeliveryRestricted| Booliano | Se caixa de correio do destinatário é restrita, por exemplo, aceitar mensagens de apenas uma lista de remetentes confiáveis, predefinida rejeitar mensagens de uma lista de remetentes predefinida, ou aceitar mensagens de apenas os remetentes autenticados. |
| emailAddress | [emailAddress](../resources/emailaddress.md) | O endereço de email do destinatário para obter dicas de email para. |
| erro | [mailTipsError](../resources/mailtipserror.md) | Erros que ocorrem durante a ação [getMailTips](../api/user-getmailtips.md) . |
| ExternalMemberCount | Int32 | O número de membros externos se o destinatário é uma lista de distribuição. |
| IsModerated |Booliano  | Se o envio de mensagens para o destinatário requer aprovação. Por exemplo, se o destinatário é uma lista de distribuição grandes e um moderador tiver sido definido até aprovar as mensagens enviadas para essa lista de distribuição ou se o envio de mensagens para um destinatário requer aprovação do gerente do destinatário. |
| MailboxFull | Booliano | O status completo da caixa de correio do destinatário. |
| MaxMessageSize | Int32 | O tamanho máximo da mensagem que tenha sido configurado para a organização ou a caixa de correio do destinatário. |
| recipientScope | String | O escopo do destinatário. Os valores possíveis são: `none`, `internal`, `external`, `externalPartner`, `externalNonParther`. Por exemplo, um administrador pode definir outra organização seja seu parceiro de"". O escopo é útil quando um administrador deseja que seja acessível a determinados escopos determinadas dicas de email. Também é útil para remetentes para informar a eles que seus mensagem pode deixar a organização, ajudando-os a tomar as decisões corretas sobre palavras, o tom e o conteúdo.|
| recipientSuggestions | Coleção [recipient](../resources/recipient.md) | Destinatários sugerido contextos de anteriores com base em onde eles aparecem na mesma mensagem. |
| TotalMemberCount | Int32 | O número de membros se o destinatário é uma lista de distribuição. |

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
