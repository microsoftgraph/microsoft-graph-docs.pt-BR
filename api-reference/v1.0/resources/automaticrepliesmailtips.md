---
title: tipo de recurso de automaticRepliesMailTips
description: Dicas de email sobre qualquer respostas automáticas que foram configuradas em uma caixa de correio.
localization_priority: Normal
ms.openlocfilehash: bb477979b975996f70e4b8ac624befab7f254f46
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27816272"
---
# <a name="automaticrepliesmailtips-resource-type"></a><span data-ttu-id="f4b5d-103">tipo de recurso de automaticRepliesMailTips</span><span class="sxs-lookup"><span data-stu-id="f4b5d-103">automaticRepliesMailTips resource type</span></span>


<span data-ttu-id="f4b5d-104">[Dicas de email](../resources/mailtips.md) sobre qualquer respostas automáticas que foram configurados em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="f4b5d-104">[MailTips](../resources/mailtips.md) about any automatic replies that have been set up on a mailbox.</span></span>

## <a name="properties"></a><span data-ttu-id="f4b5d-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f4b5d-105">Properties</span></span>
| <span data-ttu-id="f4b5d-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f4b5d-106">Property</span></span>     | <span data-ttu-id="f4b5d-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="f4b5d-107">Type</span></span>   |<span data-ttu-id="f4b5d-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="f4b5d-108">Description</span></span>|
|:-----|:-----|:-----|
| <span data-ttu-id="f4b5d-109">mensagem</span><span class="sxs-lookup"><span data-stu-id="f4b5d-109">message</span></span> | <span data-ttu-id="f4b5d-110">String</span><span class="sxs-lookup"><span data-stu-id="f4b5d-110">String</span></span> | <span data-ttu-id="f4b5d-111">A mensagem de resposta automática.</span><span class="sxs-lookup"><span data-stu-id="f4b5d-111">The automatic reply message.</span></span> |
| <span data-ttu-id="f4b5d-112">messageLanguage</span><span class="sxs-lookup"><span data-stu-id="f4b5d-112">messageLanguage</span></span> | [<span data-ttu-id="f4b5d-113">localeInfo</span><span class="sxs-lookup"><span data-stu-id="f4b5d-113">localeInfo</span></span>](../resources/localeinfo.md) | <span data-ttu-id="f4b5d-114">O idioma em que a mensagem de resposta automática está em.</span><span class="sxs-lookup"><span data-stu-id="f4b5d-114">The language that the automatic reply message is in.</span></span> |
| <span data-ttu-id="f4b5d-115">scheduledEndTime</span><span class="sxs-lookup"><span data-stu-id="f4b5d-115">scheduledEndTime</span></span> | [<span data-ttu-id="f4b5d-116">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="f4b5d-116">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md) | <span data-ttu-id="f4b5d-117">A data e hora em que as respostas automáticas estão definidas para encerrar.</span><span class="sxs-lookup"><span data-stu-id="f4b5d-117">The date and time that automatic replies are set to end.</span></span> |
| <span data-ttu-id="f4b5d-118">scheduledStartTime</span><span class="sxs-lookup"><span data-stu-id="f4b5d-118">scheduledStartTime</span></span> | [<span data-ttu-id="f4b5d-119">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="f4b5d-119">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md) | <span data-ttu-id="f4b5d-120">A data e hora em que as respostas automáticas estão definidas para começar.</span><span class="sxs-lookup"><span data-stu-id="f4b5d-120">The date and time that automatic replies are set to begin.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f4b5d-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f4b5d-121">JSON representation</span></span>

<span data-ttu-id="f4b5d-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f4b5d-122">Here is a JSON representation of the resource.</span></span>

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
