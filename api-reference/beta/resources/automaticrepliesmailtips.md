---
title: tipo de recurso automaticRepliesMailTips
description: Dicas de correio sobre as respostas automáticas que foram configuradas em uma caixa de correio.
localization_priority: Normal
ms.openlocfilehash: faefc5997f724afeaf09ff4740aac5702be159fa
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339043"
---
# <a name="automaticrepliesmailtips-resource-type"></a><span data-ttu-id="c47c9-103">tipo de recurso automaticRepliesMailTips</span><span class="sxs-lookup"><span data-stu-id="c47c9-103">automaticRepliesMailTips resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c47c9-104">[Dicas](../resources/mailtips.md) de correio sobre as respostas automáticas que foram configuradas em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="c47c9-104">[MailTips](../resources/mailtips.md) about any automatic replies that have been set up on a mailbox.</span></span>

## <a name="properties"></a><span data-ttu-id="c47c9-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c47c9-105">Properties</span></span>
| <span data-ttu-id="c47c9-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c47c9-106">Property</span></span>     | <span data-ttu-id="c47c9-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="c47c9-107">Type</span></span>   |<span data-ttu-id="c47c9-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="c47c9-108">Description</span></span>|
|:-----|:-----|:-----|
| <span data-ttu-id="c47c9-109">mensagem</span><span class="sxs-lookup"><span data-stu-id="c47c9-109">message</span></span> | <span data-ttu-id="c47c9-110">String</span><span class="sxs-lookup"><span data-stu-id="c47c9-110">String</span></span> | <span data-ttu-id="c47c9-111">A mensagem de resposta automática.</span><span class="sxs-lookup"><span data-stu-id="c47c9-111">The automatic reply message.</span></span> |
| <span data-ttu-id="c47c9-112">messageLanguage</span><span class="sxs-lookup"><span data-stu-id="c47c9-112">messageLanguage</span></span> | [<span data-ttu-id="c47c9-113">localeInfo</span><span class="sxs-lookup"><span data-stu-id="c47c9-113">localeInfo</span></span>](../resources/localeinfo.md) | <span data-ttu-id="c47c9-114">O idioma em que a mensagem de resposta automática está.</span><span class="sxs-lookup"><span data-stu-id="c47c9-114">The language that the automatic reply message is in.</span></span> |
| <span data-ttu-id="c47c9-115">scheduledEndTime</span><span class="sxs-lookup"><span data-stu-id="c47c9-115">scheduledEndTime</span></span> | [<span data-ttu-id="c47c9-116">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="c47c9-116">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md) | <span data-ttu-id="c47c9-117">A data e a hora em que as respostas automáticas estão definidas para terminar.</span><span class="sxs-lookup"><span data-stu-id="c47c9-117">The date and time that automatic replies are set to end.</span></span> |
| <span data-ttu-id="c47c9-118">scheduledStartTime</span><span class="sxs-lookup"><span data-stu-id="c47c9-118">scheduledStartTime</span></span> | [<span data-ttu-id="c47c9-119">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="c47c9-119">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md) | <span data-ttu-id="c47c9-120">A data e a hora em que as respostas automáticas estão definidas para começar.</span><span class="sxs-lookup"><span data-stu-id="c47c9-120">The date and time that automatic replies are set to begin.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c47c9-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c47c9-121">JSON representation</span></span>

<span data-ttu-id="c47c9-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c47c9-122">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "automaticRepliesMailTips resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
