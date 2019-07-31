---
title: Configurando a mensagem de convite
description: O objeto invitedUserMessageInfo permite que você configure a mensagem de convite.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 1c9fffd2edec48fb528dcb2f6c5a751dd4f32d30
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36010102"
---
# <a name="configuring-the-invitation-message"></a><span data-ttu-id="fbe38-103">Configurando a mensagem de convite</span><span class="sxs-lookup"><span data-stu-id="fbe38-103">Configuring the invitation message</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fbe38-104">O objeto invitedUserMessageInfo permite que você configure a mensagem de [convite](invitation.md) .</span><span class="sxs-lookup"><span data-stu-id="fbe38-104">The invitedUserMessageInfo object allows you to configure the [invitation](invitation.md) message.</span></span>


## <a name="properties"></a><span data-ttu-id="fbe38-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fbe38-105">Properties</span></span>
| <span data-ttu-id="fbe38-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fbe38-106">Property</span></span>     | <span data-ttu-id="fbe38-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="fbe38-107">Type</span></span>   |<span data-ttu-id="fbe38-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="fbe38-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fbe38-109">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="fbe38-109">ccRecipients</span></span>|<span data-ttu-id="fbe38-110">Coleção [recipient](recipient.md)</span><span class="sxs-lookup"><span data-stu-id="fbe38-110">[recipient](recipient.md) collection</span></span>|<span data-ttu-id="fbe38-111">Destinatários adicionais para os quais a mensagem de convite deve ser enviada.</span><span class="sxs-lookup"><span data-stu-id="fbe38-111">Additional recipients the invitation message should be sent to.</span></span> <span data-ttu-id="fbe38-112">Atualmente, apenas 1 destinatário adicional é suportado.</span><span class="sxs-lookup"><span data-stu-id="fbe38-112">Currently only 1 additional recipient is supported.</span></span>|
|<span data-ttu-id="fbe38-113">customizedMessageBody</span><span class="sxs-lookup"><span data-stu-id="fbe38-113">customizedMessageBody</span></span>|<span data-ttu-id="fbe38-114">String</span><span class="sxs-lookup"><span data-stu-id="fbe38-114">String</span></span>|<span data-ttu-id="fbe38-115">O corpo da mensagem personalizada que você deseja enviar se não quiser a mensagem padrão.</span><span class="sxs-lookup"><span data-stu-id="fbe38-115">Customized message body you want to send if you don't want the default message.</span></span>|
|<span data-ttu-id="fbe38-116">messageLanguage</span><span class="sxs-lookup"><span data-stu-id="fbe38-116">messageLanguage</span></span>|<span data-ttu-id="fbe38-117">String</span><span class="sxs-lookup"><span data-stu-id="fbe38-117">String</span></span>|<span data-ttu-id="fbe38-118">O idioma no qual você deseja enviar a mensagem padrão.</span><span class="sxs-lookup"><span data-stu-id="fbe38-118">The language you want to send the default message in.</span></span> <span data-ttu-id="fbe38-119">Se customizedMessageBody for especificado, essa propriedade será ignorada e a mensagem será enviada usando o customizedMessageBody.</span><span class="sxs-lookup"><span data-stu-id="fbe38-119">If the customizedMessageBody is specified, this property is ignored, and the message is sent using the customizedMessageBody.</span></span> <span data-ttu-id="fbe38-120">O formato de idioma deve estar no ISO 639.</span><span class="sxs-lookup"><span data-stu-id="fbe38-120">The language format should be in ISO 639.</span></span> <span data-ttu-id="fbe38-121">O padrão é en-US.</span><span class="sxs-lookup"><span data-stu-id="fbe38-121">The default is en-US.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fbe38-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fbe38-122">JSON representation</span></span>
<span data-ttu-id="fbe38-123">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="fbe38-123">Here is a JSON representation of the resource</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "invitedUserMessageInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
