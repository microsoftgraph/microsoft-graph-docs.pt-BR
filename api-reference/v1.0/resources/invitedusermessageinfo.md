---
title: ConFigurando a mensagem de convite
description: O objeto invitedUserMessageInfo permite que você configure a mensagem de convite.
localization_priority: Normal
ms.openlocfilehash: 06be157e61fd6d466cc2b18546bb29762d0133a8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32585115"
---
# <a name="configuring-the-invitation-message"></a>ConFigurando a mensagem de convite

O objeto invitedUserMessageInfo permite que você configure a mensagem de [convite](invitation.md) .


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|ccRecipients|Coleção [Recipient](recipient.md)|Destinatários adicionais para os quais a mensagem de convite deve ser enviada. Atualmente, apenas 1 destinatário adicional é suportado.|
|customizedMessageBody|String|O corpo da mensagem personalizada que você deseja enviar se não quiser a mensagem padrão.|
|messageLanguage|String|O idioma no qual você deseja enviar a mensagem padrão. Se customizedMessageBody for especificado, essa propriedade será ignorada e a mensagem será enviada usando o customizedMessageBody. O formato de idioma deve estar no ISO 639. O padrão é en-US.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso

<!-- {"blockType": "resource", "@odata.type": "microsoft.graph.invitedUserMessageInfo"} -->
```json
{
  "ccRecipients": [ {"@odata.type": "microsoft.graph.recipient"} ],
  "customizedMessageBody": "string",
  "messageLanguage": "string"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2016-22-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "invitedUserMessageInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
