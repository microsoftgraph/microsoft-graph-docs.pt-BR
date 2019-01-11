---
title: Configurando a mensagem de convite
description: O objeto invitedUserMessageInfo permite que você configure a mensagem de convite.
localization_priority: Normal
ms.openlocfilehash: f8a6dd118f1774320e3fe8327d284dac1141fc55
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27874120"
---
# <a name="configuring-the-invitation-message"></a><span data-ttu-id="44f94-103">Configurando a mensagem de convite</span><span class="sxs-lookup"><span data-stu-id="44f94-103">Configuring the invitation message</span></span>

> <span data-ttu-id="44f94-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="44f94-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="44f94-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="44f94-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="44f94-106">O objeto invitedUserMessageInfo permite que você configure a mensagem de [convite](invitation.md).</span><span class="sxs-lookup"><span data-stu-id="44f94-106">The invitedUserMessageInfo object allows you to configure the [invitation](invitation.md) message.</span></span>


## <a name="properties"></a><span data-ttu-id="44f94-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="44f94-107">Properties</span></span>
| <span data-ttu-id="44f94-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="44f94-108">Property</span></span>     | <span data-ttu-id="44f94-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="44f94-109">Type</span></span>   |<span data-ttu-id="44f94-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="44f94-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="44f94-111">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="44f94-111">ccRecipients</span></span>|[<span data-ttu-id="44f94-112">Destinatários</span><span class="sxs-lookup"><span data-stu-id="44f94-112">Recipients</span></span>](recipient.md)|<span data-ttu-id="44f94-p102">Outros destinatários aos quais a mensagem de convite deve ser enviada. No momento, só é possível adicionar mais um destinatário.</span><span class="sxs-lookup"><span data-stu-id="44f94-p102">Additional recipients the invitation message should be sent to. Currently only 1 additional recipient is supported.</span></span>|
|<span data-ttu-id="44f94-115">customizedMessageBody</span><span class="sxs-lookup"><span data-stu-id="44f94-115">customizedMessageBody</span></span>|<span data-ttu-id="44f94-116">String</span><span class="sxs-lookup"><span data-stu-id="44f94-116">String</span></span>|<span data-ttu-id="44f94-117">Corpo da mensagem personalizada a ser enviada caso você não queira a mensagem padrão.</span><span class="sxs-lookup"><span data-stu-id="44f94-117">Customized message body you want to send if you don't want the default message.</span></span>|
|<span data-ttu-id="44f94-118">messageLanguage</span><span class="sxs-lookup"><span data-stu-id="44f94-118">messageLanguage</span></span>|<span data-ttu-id="44f94-119">String</span><span class="sxs-lookup"><span data-stu-id="44f94-119">String</span></span>|<span data-ttu-id="44f94-p103">O idioma no qual você deseja enviar a mensagem padrão. Se customizedMessageBody for especificada, essa propriedade será ignorada, e a mensagem será enviada usando-se customizedMessageBody. O formato do idioma deve estar no ISO 639. O padrão é en-US.</span><span class="sxs-lookup"><span data-stu-id="44f94-p103">The language you want to send the default message in. If the customizedMessageBody is specified, this property is ignored, and the message is sent using the customizedMessageBody. The language format should be in ISO 639. The default is en-US.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="44f94-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="44f94-124">JSON representation</span></span>
<span data-ttu-id="44f94-125">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="44f94-125">Here is a JSON representation of the resource</span></span>

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
