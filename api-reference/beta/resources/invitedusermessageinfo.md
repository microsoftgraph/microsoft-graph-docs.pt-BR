---
title: Configurando a mensagem de convite
description: O objeto invitedUserMessageInfo permite que você configure a mensagem de convite.
localization_priority: Normal
ms.openlocfilehash: fa7ead6938ddfaca78322f56f4638c45d3f2df14
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643787"
---
# <a name="configuring-the-invitation-message"></a><span data-ttu-id="3e5d0-103">Configurando a mensagem de convite</span><span class="sxs-lookup"><span data-stu-id="3e5d0-103">Configuring the invitation message</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3e5d0-104">O objeto invitedUserMessageInfo permite que você configure a mensagem de [convite](invitation.md).</span><span class="sxs-lookup"><span data-stu-id="3e5d0-104">The invitedUserMessageInfo object allows you to configure the [invitation](invitation.md) message.</span></span>


## <a name="properties"></a><span data-ttu-id="3e5d0-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3e5d0-105">Properties</span></span>
| <span data-ttu-id="3e5d0-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3e5d0-106">Property</span></span>     | <span data-ttu-id="3e5d0-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="3e5d0-107">Type</span></span>   |<span data-ttu-id="3e5d0-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="3e5d0-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3e5d0-109">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="3e5d0-109">ccRecipients</span></span>|[<span data-ttu-id="3e5d0-110">Destinatários</span><span class="sxs-lookup"><span data-stu-id="3e5d0-110">Recipients</span></span>](recipient.md)|<span data-ttu-id="3e5d0-p101">Outros destinatários aos quais a mensagem de convite deve ser enviada. No momento, só é possível adicionar mais um destinatário.</span><span class="sxs-lookup"><span data-stu-id="3e5d0-p101">Additional recipients the invitation message should be sent to. Currently only 1 additional recipient is supported.</span></span>|
|<span data-ttu-id="3e5d0-113">customizedMessageBody</span><span class="sxs-lookup"><span data-stu-id="3e5d0-113">customizedMessageBody</span></span>|<span data-ttu-id="3e5d0-114">String</span><span class="sxs-lookup"><span data-stu-id="3e5d0-114">String</span></span>|<span data-ttu-id="3e5d0-115">Corpo da mensagem personalizada a ser enviada caso você não queira a mensagem padrão.</span><span class="sxs-lookup"><span data-stu-id="3e5d0-115">Customized message body you want to send if you don't want the default message.</span></span>|
|<span data-ttu-id="3e5d0-116">messageLanguage</span><span class="sxs-lookup"><span data-stu-id="3e5d0-116">messageLanguage</span></span>|<span data-ttu-id="3e5d0-117">String</span><span class="sxs-lookup"><span data-stu-id="3e5d0-117">String</span></span>|<span data-ttu-id="3e5d0-p102">O idioma no qual você deseja enviar a mensagem padrão. Se customizedMessageBody for especificada, essa propriedade será ignorada, e a mensagem será enviada usando-se customizedMessageBody. O formato do idioma deve estar no ISO 639. O padrão é en-US.</span><span class="sxs-lookup"><span data-stu-id="3e5d0-p102">The language you want to send the default message in. If the customizedMessageBody is specified, this property is ignored, and the message is sent using the customizedMessageBody. The language format should be in ISO 639. The default is en-US.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3e5d0-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3e5d0-122">JSON representation</span></span>
<span data-ttu-id="3e5d0-123">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="3e5d0-123">Here is a JSON representation of the resource</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/invitedusermessageinfo.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
