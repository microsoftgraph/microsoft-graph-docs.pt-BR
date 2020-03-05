---
title: Configurando a mensagem de convite
description: O objeto invitedUserMessageInfo permite que você configure a mensagem de convite.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 324ce713354fc8f27ef926ef1ee0bbf538ee4b0a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447700"
---
# <a name="configuring-the-invitation-message"></a><span data-ttu-id="b1f38-103">Configurando a mensagem de convite</span><span class="sxs-lookup"><span data-stu-id="b1f38-103">Configuring the invitation message</span></span>

<span data-ttu-id="b1f38-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="b1f38-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b1f38-105">O objeto invitedUserMessageInfo permite que você configure a mensagem de [convite](invitation.md) .</span><span class="sxs-lookup"><span data-stu-id="b1f38-105">The invitedUserMessageInfo object allows you to configure the [invitation](invitation.md) message.</span></span>


## <a name="properties"></a><span data-ttu-id="b1f38-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b1f38-106">Properties</span></span>
| <span data-ttu-id="b1f38-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b1f38-107">Property</span></span>     | <span data-ttu-id="b1f38-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="b1f38-108">Type</span></span>   |<span data-ttu-id="b1f38-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="b1f38-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b1f38-110">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="b1f38-110">ccRecipients</span></span>|<span data-ttu-id="b1f38-111">Coleção [Recipient](recipient.md)</span><span class="sxs-lookup"><span data-stu-id="b1f38-111">[Recipient](recipient.md) collection</span></span>|<span data-ttu-id="b1f38-112">Destinatários adicionais para os quais a mensagem de convite deve ser enviada.</span><span class="sxs-lookup"><span data-stu-id="b1f38-112">Additional recipients the invitation message should be sent to.</span></span> <span data-ttu-id="b1f38-113">Atualmente, apenas 1 destinatário adicional é suportado.</span><span class="sxs-lookup"><span data-stu-id="b1f38-113">Currently only 1 additional recipient is supported.</span></span>|
|<span data-ttu-id="b1f38-114">customizedMessageBody</span><span class="sxs-lookup"><span data-stu-id="b1f38-114">customizedMessageBody</span></span>|<span data-ttu-id="b1f38-115">String</span><span class="sxs-lookup"><span data-stu-id="b1f38-115">String</span></span>|<span data-ttu-id="b1f38-116">O corpo da mensagem personalizada que você deseja enviar se não quiser a mensagem padrão.</span><span class="sxs-lookup"><span data-stu-id="b1f38-116">Customized message body you want to send if you don't want the default message.</span></span>|
|<span data-ttu-id="b1f38-117">messageLanguage</span><span class="sxs-lookup"><span data-stu-id="b1f38-117">messageLanguage</span></span>|<span data-ttu-id="b1f38-118">String</span><span class="sxs-lookup"><span data-stu-id="b1f38-118">String</span></span>|<span data-ttu-id="b1f38-119">O idioma no qual você deseja enviar a mensagem padrão.</span><span class="sxs-lookup"><span data-stu-id="b1f38-119">The language you want to send the default message in.</span></span> <span data-ttu-id="b1f38-120">Se customizedMessageBody for especificado, essa propriedade será ignorada e a mensagem será enviada usando o customizedMessageBody.</span><span class="sxs-lookup"><span data-stu-id="b1f38-120">If the customizedMessageBody is specified, this property is ignored, and the message is sent using the customizedMessageBody.</span></span> <span data-ttu-id="b1f38-121">O formato de idioma deve estar no ISO 639.</span><span class="sxs-lookup"><span data-stu-id="b1f38-121">The language format should be in ISO 639.</span></span> <span data-ttu-id="b1f38-122">O padrão é en-US.</span><span class="sxs-lookup"><span data-stu-id="b1f38-122">The default is en-US.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b1f38-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b1f38-123">JSON representation</span></span>
<span data-ttu-id="b1f38-124">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="b1f38-124">Here is a JSON representation of the resource</span></span>

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
