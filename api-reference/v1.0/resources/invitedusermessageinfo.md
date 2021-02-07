---
title: Configurando a mensagem de convite
description: O objeto invitedUserMessageInfo permite configurar a mensagem de convite.
localization_priority: Normal
author: elisolMS
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: d44542b26fd1c1ffb7b70dcfc019ada6f0cc02f5
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50129720"
---
# <a name="configuring-the-invitation-message"></a>Configurando a mensagem de convite

Namespace: microsoft.graph

O objeto invitedUserMessageInfo permite configurar a mensagem [de](invitation.md) convite.


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|ccRecipients|Coleção [Recipient](recipient.md)|Destinatários adicionais para os que a mensagem de convite deve ser enviada. Atualmente, apenas 1 destinatário adicional é suportado.|
|customizedMessageBody|String|Corpo de mensagem personalizado que você deseja enviar se não quiser a mensagem padrão.|
|messageLanguage|String|O idioma em que você deseja enviar a mensagem padrão. Se customizedMessageBody for especificado, essa propriedade será ignorada e a mensagem será enviada usando customizedMessageBody. O formato de idioma deve estar na ISO 639. O padrão é en-US.|

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

