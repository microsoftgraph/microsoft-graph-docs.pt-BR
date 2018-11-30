---
title: tipo de recurso de automaticRepliesMailTips
description: Dicas de email sobre qualquer respostas automáticas que foram configuradas em uma caixa de correio.
ms.openlocfilehash: 943a465671c777305e5623104c82f377ff9496dd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27005423"
---
# <a name="automaticrepliesmailtips-resource-type"></a><span data-ttu-id="962b2-103">tipo de recurso de automaticRepliesMailTips</span><span class="sxs-lookup"><span data-stu-id="962b2-103">automaticRepliesMailTips resource type</span></span>


<span data-ttu-id="962b2-104">[Dicas de email](../resources/mailtips.md) sobre qualquer respostas automáticas que foram configurados em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="962b2-104">[MailTips](../resources/mailtips.md) about any automatic replies that have been set up on a mailbox.</span></span>

## <a name="properties"></a><span data-ttu-id="962b2-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="962b2-105">Properties</span></span>
| <span data-ttu-id="962b2-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="962b2-106">Property</span></span>     | <span data-ttu-id="962b2-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="962b2-107">Type</span></span>   |<span data-ttu-id="962b2-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="962b2-108">Description</span></span>|
|:-----|:-----|:-----|
| <span data-ttu-id="962b2-109">mensagem</span><span class="sxs-lookup"><span data-stu-id="962b2-109">message</span></span> | <span data-ttu-id="962b2-110">String</span><span class="sxs-lookup"><span data-stu-id="962b2-110">String</span></span> | <span data-ttu-id="962b2-111">A mensagem de resposta automática.</span><span class="sxs-lookup"><span data-stu-id="962b2-111">The automatic reply message.</span></span> |
| <span data-ttu-id="962b2-112">messageLanguage</span><span class="sxs-lookup"><span data-stu-id="962b2-112">messageLanguage</span></span> | [<span data-ttu-id="962b2-113">localeInfo</span><span class="sxs-lookup"><span data-stu-id="962b2-113">localeInfo</span></span>](../resources/localeinfo.md) | <span data-ttu-id="962b2-114">O idioma em que a mensagem de resposta automática está em.</span><span class="sxs-lookup"><span data-stu-id="962b2-114">The language that the automatic reply message is in.</span></span> |
| <span data-ttu-id="962b2-115">scheduledEndTime</span><span class="sxs-lookup"><span data-stu-id="962b2-115">scheduledEndTime</span></span> | [<span data-ttu-id="962b2-116">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="962b2-116">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md) | <span data-ttu-id="962b2-117">A data e hora em que as respostas automáticas estão definidas para encerrar.</span><span class="sxs-lookup"><span data-stu-id="962b2-117">The date and time that automatic replies are set to end.</span></span> |
| <span data-ttu-id="962b2-118">scheduledStartTime</span><span class="sxs-lookup"><span data-stu-id="962b2-118">scheduledStartTime</span></span> | [<span data-ttu-id="962b2-119">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="962b2-119">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md) | <span data-ttu-id="962b2-120">A data e hora em que as respostas automáticas estão definidas para começar.</span><span class="sxs-lookup"><span data-stu-id="962b2-120">The date and time that automatic replies are set to begin.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="962b2-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="962b2-121">JSON representation</span></span>

<span data-ttu-id="962b2-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="962b2-122">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "messageLanguage",
    "scheduledEndTime",
    "scheduledStartTime"
  ],
  "@odata.type": "microsoft.graph.automaticRepliesMailTips"
}-->

```json
{
  "message": "string",
  "messageLanguage": {"@odata.type": "microsoft.graph.localeInfo"},
  "scheduledEndTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "scheduledStartTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "automaticRepliesMailTips resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->