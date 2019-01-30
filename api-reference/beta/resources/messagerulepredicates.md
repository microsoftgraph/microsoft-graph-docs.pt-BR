---
title: Tipo de recurso messageRulePredicates
description: Representa o conjunto de condições e exceções disponíveis para uma regra.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: fda6a160d30dc0d822f2e0aeb5642250d6b69658
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29644032"
---
# <a name="messagerulepredicates-resource-type"></a>Tipo de recurso messageRulePredicates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o conjunto de condições e exceções disponíveis para uma regra.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
| bodyContains | Coleção (String) | Representa as cadeias de caracteres que devem aparecer no corpo de uma mensagem de entrada para que a exceção ou condição seja aplicada. |
| bodyOrSubjectContains | Coleção (String) | Representa as cadeias de caracteres que devem aparecer no corpo ou assunto de uma mensagem de entrada para que a exceção ou condição seja aplicada. |
| categories | Coleção (String) | Representa as categorias com as quais a mensagem de entrada deve ser rotulada para que a exceção ou condição seja aplicada. |
| fromAddresses | Coleção ([recipient](recipient.md)) | Representa os endereços de email específicos do remetente de uma mensagem de entrada para que a condição ou exceção seja aplicada. |
| hasAttachments | Boolean | Indica se uma mensagem de entrada deve ter anexos para que a exceção ou condição seja aplicada. |
| headerContains | Coleção (String) | Representa as cadeias de caracteres que são exibidas nos cabeçalhos de uma mensagem de entrada para que a exceção ou condição seja aplicada. |
| importance | Cadeia de caracteres | A importância que é marcada em uma mensagem de entrada para que a exceção ou condição seja aplicada: `low`, `normal`, `high`. |
| isApprovalRequest | Boolean | Indica se uma mensagem de entrada deve ter uma solicitação de aprovação para que a exceção ou condição seja aplicada. |
| isAutomaticForward | Boolean | Indica se uma mensagem de entrada deve ser encaminhada automaticamente para que a exceção ou condição seja aplicada. |
| isAutomaticReply | Boolean | Indica se uma mensagem de entrada deve ser uma resposta automática para que a exceção ou condição seja aplicada. |
| isEncrypted | Boolean | Indica se uma mensagem de entrada deve estar criptografada para que a exceção ou condição seja aplicada. |
| isMeetingRequest | Boolean | Indica se uma mensagem de entrada deve ser uma solicitação de reunião para que a exceção ou condição seja aplicada. |
| isMeetingResponse | Boolean | Indica se uma mensagem de entrada deve ser uma resposta à solicitação de reunião para que a exceção ou condição seja aplicada. |
| isNonDeliveryReport | Boolean | Indica se uma mensagem de entrada deve ser uma notificação de falha na entrega para que a exceção ou condição seja aplicada. |
| isPermissionControlled | Boolean | Indica se uma mensagem de entrada deve ser uma permissão controlada (protegida por RMS) para que a exceção ou condição seja aplicada. |
| isReadReceipt | Boolean | Indica se uma mensagem de entrada deve ser uma confirmação de leitura para que a exceção ou condição seja aplicada. |
| isSigned | Boolean | Indica se uma mensagem de entrada deve ser assinada por S/MIME para que a exceção ou condição seja aplicada. |
| isVoicemail | Boolean | Indica se uma mensagem de entrada deve ser uma caixa postal para que a exceção ou condição seja aplicada. |
| messageActionFlag | Cadeia de caracteres  | Representa o valor do sinalizador de ações que é exibido em uma mensagem de entrada para que a exceção ou condição seja aplicada. Os valores possíveis são: `any`, `call`, `doNotForward`, `followUp`, `fyi`, `forward`, `noResponseNecessary`, `read`, `reply`, `replyToAll`, `review`. |
| notSentToMe | Boolean | Indica se o proprietário da caixa de correio não deve ser um destinatário de uma mensagem de entrada para que a condição ou exceção seja aplicada. |
| recipientContains | Coleção (String) | Representa as cadeias de caracteres que são exibidas nas propriedades **toRecipients** ou **ccRecipients** de uma mensagem de entrada para que a exceção ou condição seja aplicada. |
| senderContains | Coleção (String) | Representa as cadeias de caracteres que são exibidas na propriedade **from** de uma mensagem de entrada para que a exceção ou condição seja aplicada. |
| sensitivity | Cadeia de caracteres | Representa o nível de sensibilidade que deve ser marcado em uma mensagem de entrada para que a condição ou exceção seja aplicada. Os valores possíveis são: `normal`, `personal`, `private`, `confidential`. |
| sentCcMe | Boolean | Indica se o proprietário da caixa de correio deve estar na propriedade **ccRecipients** de uma mensagem de entrada para que a condição ou exceção seja aplicada. |
| sentOnlyToMe | Boolean | Indica se o proprietário da caixa de correio deve ser o único destinatário em uma mensagem de entrada para que a condição ou exceção seja aplicada. |
| sentToAddresses | Coleção ([recipient](recipient.md)) | Representa os endereços de email para os quais uma mensagem de entrada deve ter sido enviada para que a condição ou exceção seja aplicada. |
| sentToMe | Boolean | Indica se o proprietário da caixa de correio deve estar na propriedade **toRecipients** de uma mensagem de entrada para que a condição ou exceção seja aplicada. |
| sentToOrCcMe | Boolean | Indica se o proprietário da caixa de correio deve estar na propriedade **toRecipients** ou **ccRecipients** de uma mensagem de entrada para que a condição ou exceção seja aplicada. |
| subjectContains | Coleção (String) | Representa as cadeias de caracteres que são exibidas no assunto de uma mensagem de entrada para que a exceção ou condição seja aplicada. |
| withinSizeRange | [sizeRange](sizerange.md) | Representa os tamanhos mínimo e máximo (em kilobytes) nos quais uma mensagem de entrada deve se enquadrar para que a condição ou exceção seja aplicada. |



## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
   ],
  "@odata.type": "microsoft.graph.messageRulePredicates"
}-->

```json
{
  "bodyContains": ["String"],
  "bodyOrSubjectContains": ["String"],
  "categories": ["String"],
  "fromAddresses": [{"@odata.type": "microsoft.graph.recipient"}],
  "hasAttachments": "Boolean",
  "headerContains": ["String"],
  "importance": "String",
  "isApprovalRequest": "Boolean",
  "isAutomaticForward": "Boolean",
  "isAutomaticReply": "Boolean",
  "isEncrypted": "Boolean",
  "isMeetingRequest": "Boolean",
  "isMeetingResponse": "Boolean",
  "isNonDeliveryReport": "Boolean",
  "isPermissionControlled": "Boolean",
  "isReadReceipt": "Boolean",
  "isSigned": "Boolean",
  "isVoicemail": "Boolean",
  "messageActionFlag": "String",
  "notSentToMe": "Boolean",
  "recipientContains": ["String"],
  "senderContains": ["String"],
  "sensitivity": "String",
  "sentCcMe": "Boolean",
  "sentOnlyToMe": "Boolean",
  "sentToAddresses": [{"@odata.type": "microsoft.graph.recipient"}],
  "sentToMe": "Boolean",
  "sentToOrCcMe": "Boolean",
  "subjectContains": ["String"],
  "withinSizeRange": {"@odata.type": "microsoft.graph.sizeRange"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "messageRulePredicates resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/messagerulepredicates.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
