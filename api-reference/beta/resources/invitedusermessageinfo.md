---
title: ConFigurando a mensagem de convite
description: O objeto invitedUserMessageInfo permite que você configure a mensagem de convite.
localization_priority: Normal
ms.openlocfilehash: fa7ead6938ddfaca78322f56f4638c45d3f2df14
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32569965"
---
# <a name="configuring-the-invitation-message"></a><span data-ttu-id="7bfff-103">ConFigurando a mensagem de convite</span><span class="sxs-lookup"><span data-stu-id="7bfff-103">Configuring the invitation message</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7bfff-104">O objeto invitedUserMessageInfo permite que você configure a mensagem de [convite](invitation.md) .</span><span class="sxs-lookup"><span data-stu-id="7bfff-104">The invitedUserMessageInfo object allows you to configure the [invitation](invitation.md) message.</span></span>


## <a name="properties"></a><span data-ttu-id="7bfff-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7bfff-105">Properties</span></span>
| <span data-ttu-id="7bfff-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7bfff-106">Property</span></span>     | <span data-ttu-id="7bfff-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="7bfff-107">Type</span></span>   |<span data-ttu-id="7bfff-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="7bfff-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7bfff-109">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="7bfff-109">ccRecipients</span></span>|[<span data-ttu-id="7bfff-110">Destinatários</span><span class="sxs-lookup"><span data-stu-id="7bfff-110">Recipients</span></span>](recipient.md)|<span data-ttu-id="7bfff-111">Destinatários adicionais para os quais a mensagem de convite deve ser enviada.</span><span class="sxs-lookup"><span data-stu-id="7bfff-111">Additional recipients the invitation message should be sent to.</span></span> <span data-ttu-id="7bfff-112">Atualmente, apenas 1 destinatário adicional é suportado.</span><span class="sxs-lookup"><span data-stu-id="7bfff-112">Currently only 1 additional recipient is supported.</span></span>|
|<span data-ttu-id="7bfff-113">customizedMessageBody</span><span class="sxs-lookup"><span data-stu-id="7bfff-113">customizedMessageBody</span></span>|<span data-ttu-id="7bfff-114">String</span><span class="sxs-lookup"><span data-stu-id="7bfff-114">String</span></span>|<span data-ttu-id="7bfff-115">O corpo da mensagem personalizada que você deseja enviar se não quiser a mensagem padrão.</span><span class="sxs-lookup"><span data-stu-id="7bfff-115">Customized message body you want to send if you don't want the default message.</span></span>|
|<span data-ttu-id="7bfff-116">messageLanguage</span><span class="sxs-lookup"><span data-stu-id="7bfff-116">messageLanguage</span></span>|<span data-ttu-id="7bfff-117">String</span><span class="sxs-lookup"><span data-stu-id="7bfff-117">String</span></span>|<span data-ttu-id="7bfff-118">O idioma no qual você deseja enviar a mensagem padrão.</span><span class="sxs-lookup"><span data-stu-id="7bfff-118">The language you want to send the default message in.</span></span> <span data-ttu-id="7bfff-119">Se customizedMessageBody for especificado, essa propriedade será ignorada e a mensagem será enviada usando o customizedMessageBody.</span><span class="sxs-lookup"><span data-stu-id="7bfff-119">If the customizedMessageBody is specified, this property is ignored, and the message is sent using the customizedMessageBody.</span></span> <span data-ttu-id="7bfff-120">O formato de idioma deve estar no ISO 639.</span><span class="sxs-lookup"><span data-stu-id="7bfff-120">The language format should be in ISO 639.</span></span> <span data-ttu-id="7bfff-121">O padrão é en-US.</span><span class="sxs-lookup"><span data-stu-id="7bfff-121">The default is en-US.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7bfff-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7bfff-122">JSON representation</span></span>
<span data-ttu-id="7bfff-123">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="7bfff-123">Here is a JSON representation of the resource</span></span>

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
