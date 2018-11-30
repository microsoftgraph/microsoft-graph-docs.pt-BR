---
title: Configurando a mensagem de convite
description: O objeto invitedUserMessageInfo permite que você configure a mensagem de convite.
ms.openlocfilehash: c8258d2b90d1aa5f5081b271ccc70fcb7408b132
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006640"
---
# <a name="configuring-the-invitation-message"></a><span data-ttu-id="b1b82-103">Configurando a mensagem de convite</span><span class="sxs-lookup"><span data-stu-id="b1b82-103">Configuring the invitation message</span></span>

<span data-ttu-id="b1b82-104">O objeto invitedUserMessageInfo permite que você configure a mensagem de [convite](invitation.md).</span><span class="sxs-lookup"><span data-stu-id="b1b82-104">The invitedUserMessageInfo object allows you to configure the [invitation](invitation.md) message.</span></span>


## <a name="properties"></a><span data-ttu-id="b1b82-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b1b82-105">Properties</span></span>
| <span data-ttu-id="b1b82-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b1b82-106">Property</span></span>     | <span data-ttu-id="b1b82-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="b1b82-107">Type</span></span>   |<span data-ttu-id="b1b82-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="b1b82-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b1b82-109">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="b1b82-109">ccRecipients</span></span>|<span data-ttu-id="b1b82-110">Coleção [Recipient](recipient.md)</span><span class="sxs-lookup"><span data-stu-id="b1b82-110">[Recipient](recipient.md) collection</span></span>|<span data-ttu-id="b1b82-p101">Outros destinatários aos quais a mensagem de convite deve ser enviada. No momento, só é possível adicionar mais um destinatário.</span><span class="sxs-lookup"><span data-stu-id="b1b82-p101">Additional recipients the invitation message should be sent to. Currently only 1 additional recipient is supported.</span></span>|
|<span data-ttu-id="b1b82-113">customizedMessageBody</span><span class="sxs-lookup"><span data-stu-id="b1b82-113">customizedMessageBody</span></span>|<span data-ttu-id="b1b82-114">String</span><span class="sxs-lookup"><span data-stu-id="b1b82-114">String</span></span>|<span data-ttu-id="b1b82-115">Corpo da mensagem personalizada a ser enviada caso você não queira a mensagem padrão.</span><span class="sxs-lookup"><span data-stu-id="b1b82-115">Customized message body you want to send if you don't want the default message.</span></span>|
|<span data-ttu-id="b1b82-116">messageLanguage</span><span class="sxs-lookup"><span data-stu-id="b1b82-116">messageLanguage</span></span>|<span data-ttu-id="b1b82-117">String</span><span class="sxs-lookup"><span data-stu-id="b1b82-117">String</span></span>|<span data-ttu-id="b1b82-p102">O idioma no qual você deseja enviar a mensagem padrão. Se customizedMessageBody for especificada, essa propriedade será ignorada, e a mensagem será enviada usando-se customizedMessageBody. O formato do idioma deve estar no ISO 639. O padrão é en-US.</span><span class="sxs-lookup"><span data-stu-id="b1b82-p102">The language you want to send the default message in. If the customizedMessageBody is specified, this property is ignored, and the message is sent using the customizedMessageBody. The language format should be in ISO 639. The default is en-US.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b1b82-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b1b82-122">JSON representation</span></span>
<span data-ttu-id="b1b82-123">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="b1b82-123">Here is a JSON representation of the resource</span></span>

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
