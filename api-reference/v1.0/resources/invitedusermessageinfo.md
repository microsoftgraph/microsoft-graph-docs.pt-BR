---
title: Configurando a mensagem de convite
description: O objeto invitedUserMessageInfo permite configurar a mensagem de convite.
ms.localizationpriority: medium
author: Sammak
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 473e043da7669cc07e79fdf3a06edb0d36f657ba
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59084416"
---
# <a name="configuring-the-invitation-message"></a>Configurando a mensagem de convite

Namespace: microsoft.graph

O objeto invitedUserMessageInfo permite configurar a [mensagem de](invitation.md) convite.


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|ccRecipients|Coleção [Recipient](recipient.md)|Destinatários adicionais aos que a mensagem de convite deve ser enviada. Atualmente, apenas 1 destinatário adicional é suportado.|
|customizedMessageBody|Cadeia de caracteres|Corpo da mensagem personalizado que você deseja enviar se não quiser a mensagem padrão.|
|messageLanguage|String|O idioma em que você deseja enviar a mensagem padrão. Se o personaledMessageBody for especificado, essa propriedade será ignorada e a mensagem será enviada usando o CustomizedMessageBody. O formato de idioma deve estar na ISO 639. O padrão é en-US.|

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

