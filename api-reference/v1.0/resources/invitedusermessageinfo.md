---
title: Configurando a mensagem de convite
description: O objeto invitedUserMessageInfo permite configurar a mensagem de convite.
localization_priority: Normal
author: Sammak
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 5b20eb15cfc8eb2ae248d87e5ae61ffa0d5ea08d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50941376"
---
# <a name="configuring-the-invitation-message"></a><span data-ttu-id="8a31d-103">Configurando a mensagem de convite</span><span class="sxs-lookup"><span data-stu-id="8a31d-103">Configuring the invitation message</span></span>

<span data-ttu-id="8a31d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8a31d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8a31d-105">O objeto invitedUserMessageInfo permite configurar a [mensagem de](invitation.md) convite.</span><span class="sxs-lookup"><span data-stu-id="8a31d-105">The invitedUserMessageInfo object allows you to configure the [invitation](invitation.md) message.</span></span>


## <a name="properties"></a><span data-ttu-id="8a31d-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8a31d-106">Properties</span></span>
| <span data-ttu-id="8a31d-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8a31d-107">Property</span></span>     | <span data-ttu-id="8a31d-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="8a31d-108">Type</span></span>   |<span data-ttu-id="8a31d-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="8a31d-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8a31d-110">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="8a31d-110">ccRecipients</span></span>|<span data-ttu-id="8a31d-111">Coleção [Recipient](recipient.md)</span><span class="sxs-lookup"><span data-stu-id="8a31d-111">[Recipient](recipient.md) collection</span></span>|<span data-ttu-id="8a31d-112">Destinatários adicionais aos que a mensagem de convite deve ser enviada.</span><span class="sxs-lookup"><span data-stu-id="8a31d-112">Additional recipients the invitation message should be sent to.</span></span> <span data-ttu-id="8a31d-113">Atualmente, apenas 1 destinatário adicional é suportado.</span><span class="sxs-lookup"><span data-stu-id="8a31d-113">Currently only 1 additional recipient is supported.</span></span>|
|<span data-ttu-id="8a31d-114">customizedMessageBody</span><span class="sxs-lookup"><span data-stu-id="8a31d-114">customizedMessageBody</span></span>|<span data-ttu-id="8a31d-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8a31d-115">String</span></span>|<span data-ttu-id="8a31d-116">Corpo da mensagem personalizado que você deseja enviar se não quiser a mensagem padrão.</span><span class="sxs-lookup"><span data-stu-id="8a31d-116">Customized message body you want to send if you don't want the default message.</span></span>|
|<span data-ttu-id="8a31d-117">messageLanguage</span><span class="sxs-lookup"><span data-stu-id="8a31d-117">messageLanguage</span></span>|<span data-ttu-id="8a31d-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8a31d-118">String</span></span>|<span data-ttu-id="8a31d-119">O idioma em que você deseja enviar a mensagem padrão.</span><span class="sxs-lookup"><span data-stu-id="8a31d-119">The language you want to send the default message in.</span></span> <span data-ttu-id="8a31d-120">Se o personaledMessageBody for especificado, essa propriedade será ignorada e a mensagem será enviada usando o CustomizedMessageBody.</span><span class="sxs-lookup"><span data-stu-id="8a31d-120">If the customizedMessageBody is specified, this property is ignored, and the message is sent using the customizedMessageBody.</span></span> <span data-ttu-id="8a31d-121">O formato de idioma deve estar na ISO 639.</span><span class="sxs-lookup"><span data-stu-id="8a31d-121">The language format should be in ISO 639.</span></span> <span data-ttu-id="8a31d-122">O padrão é en-US.</span><span class="sxs-lookup"><span data-stu-id="8a31d-122">The default is en-US.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8a31d-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8a31d-123">JSON representation</span></span>
<span data-ttu-id="8a31d-124">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="8a31d-124">Here is a JSON representation of the resource</span></span>

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

