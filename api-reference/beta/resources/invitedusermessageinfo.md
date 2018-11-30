---
title: Configurando a mensagem de convite
description: O objeto invitedUserMessageInfo permite que você configure a mensagem de convite.
ms.openlocfilehash: 326ca6654fd30da9c36022424b48c4a8f7b82ffe
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034844"
---
# <a name="configuring-the-invitation-message"></a><span data-ttu-id="66ea9-103">Configurando a mensagem de convite</span><span class="sxs-lookup"><span data-stu-id="66ea9-103">Configuring the invitation message</span></span>

> <span data-ttu-id="66ea9-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="66ea9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="66ea9-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="66ea9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="66ea9-106">O objeto invitedUserMessageInfo permite que você configure a mensagem de [convite](invitation.md).</span><span class="sxs-lookup"><span data-stu-id="66ea9-106">The invitedUserMessageInfo object allows you to configure the [invitation](invitation.md) message.</span></span>


## <a name="properties"></a><span data-ttu-id="66ea9-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="66ea9-107">Properties</span></span>
| <span data-ttu-id="66ea9-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="66ea9-108">Property</span></span>     | <span data-ttu-id="66ea9-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="66ea9-109">Type</span></span>   |<span data-ttu-id="66ea9-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="66ea9-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="66ea9-111">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="66ea9-111">ccRecipients</span></span>|[<span data-ttu-id="66ea9-112">Destinatários</span><span class="sxs-lookup"><span data-stu-id="66ea9-112">Recipients</span></span>](recipient.md)|<span data-ttu-id="66ea9-p102">Outros destinatários aos quais a mensagem de convite deve ser enviada. No momento, só é possível adicionar mais um destinatário.</span><span class="sxs-lookup"><span data-stu-id="66ea9-p102">Additional recipients the invitation message should be sent to. Currently only 1 additional recipient is supported.</span></span>|
|<span data-ttu-id="66ea9-115">customizedMessageBody</span><span class="sxs-lookup"><span data-stu-id="66ea9-115">customizedMessageBody</span></span>|<span data-ttu-id="66ea9-116">String</span><span class="sxs-lookup"><span data-stu-id="66ea9-116">String</span></span>|<span data-ttu-id="66ea9-117">Corpo da mensagem personalizada a ser enviada caso você não queira a mensagem padrão.</span><span class="sxs-lookup"><span data-stu-id="66ea9-117">Customized message body you want to send if you don't want the default message.</span></span>|
|<span data-ttu-id="66ea9-118">messageLanguage</span><span class="sxs-lookup"><span data-stu-id="66ea9-118">messageLanguage</span></span>|<span data-ttu-id="66ea9-119">String</span><span class="sxs-lookup"><span data-stu-id="66ea9-119">String</span></span>|<span data-ttu-id="66ea9-p103">O idioma no qual você deseja enviar a mensagem padrão. Se customizedMessageBody for especificada, essa propriedade será ignorada, e a mensagem será enviada usando-se customizedMessageBody. O formato do idioma deve estar no ISO 639. O padrão é en-US.</span><span class="sxs-lookup"><span data-stu-id="66ea9-p103">The language you want to send the default message in. If the customizedMessageBody is specified, this property is ignored, and the message is sent using the customizedMessageBody. The language format should be in ISO 639. The default is en-US.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="66ea9-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="66ea9-124">JSON representation</span></span>
<span data-ttu-id="66ea9-125">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="66ea9-125">Here is a JSON representation of the resource</span></span>

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
