---
title: Tipo de recurso automaticRepliesMailTips
description: Dicas de Email sobre as respostas automáticas que foram configuradas em uma caixa de correio.
localization_priority: Normal
author: abheek-das
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 1cc7f65a526d4550182f1e6dc0c5ea25a12ee182
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135748"
---
# <a name="automaticrepliesmailtips-resource-type"></a><span data-ttu-id="6f966-103">Tipo de recurso automaticRepliesMailTips</span><span class="sxs-lookup"><span data-stu-id="6f966-103">automaticRepliesMailTips resource type</span></span>

<span data-ttu-id="6f966-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6f966-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="6f966-105">[Dicas de Email](../resources/mailtips.md) sobre as respostas automáticas que foram configuradas em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="6f966-105">[MailTips](../resources/mailtips.md) about any automatic replies that have been set up on a mailbox.</span></span>

## <a name="properties"></a><span data-ttu-id="6f966-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6f966-106">Properties</span></span>
| <span data-ttu-id="6f966-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6f966-107">Property</span></span>     | <span data-ttu-id="6f966-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="6f966-108">Type</span></span>   |<span data-ttu-id="6f966-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="6f966-109">Description</span></span>|
|:-----|:-----|:-----|
| <span data-ttu-id="6f966-110">mensagem</span><span class="sxs-lookup"><span data-stu-id="6f966-110">message</span></span> | <span data-ttu-id="6f966-111">String</span><span class="sxs-lookup"><span data-stu-id="6f966-111">String</span></span> | <span data-ttu-id="6f966-112">A mensagem de resposta automática.</span><span class="sxs-lookup"><span data-stu-id="6f966-112">The automatic reply message.</span></span> |
| <span data-ttu-id="6f966-113">messageLanguage</span><span class="sxs-lookup"><span data-stu-id="6f966-113">messageLanguage</span></span> | [<span data-ttu-id="6f966-114">localeInfo</span><span class="sxs-lookup"><span data-stu-id="6f966-114">localeInfo</span></span>](../resources/localeinfo.md) | <span data-ttu-id="6f966-115">O idioma em que a mensagem de resposta automática está.</span><span class="sxs-lookup"><span data-stu-id="6f966-115">The language that the automatic reply message is in.</span></span> |
| <span data-ttu-id="6f966-116">scheduledEndTime</span><span class="sxs-lookup"><span data-stu-id="6f966-116">scheduledEndTime</span></span> | [<span data-ttu-id="6f966-117">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="6f966-117">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md) | <span data-ttu-id="6f966-118">A data e a hora em que as respostas automáticas são definidas para terminar.</span><span class="sxs-lookup"><span data-stu-id="6f966-118">The date and time that automatic replies are set to end.</span></span> |
| <span data-ttu-id="6f966-119">scheduledStartTime</span><span class="sxs-lookup"><span data-stu-id="6f966-119">scheduledStartTime</span></span> | [<span data-ttu-id="6f966-120">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="6f966-120">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md) | <span data-ttu-id="6f966-121">A data e a hora em que as respostas automáticas são definidas para começar.</span><span class="sxs-lookup"><span data-stu-id="6f966-121">The date and time that automatic replies are set to begin.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6f966-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6f966-122">JSON representation</span></span>

<span data-ttu-id="6f966-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6f966-123">Here is a JSON representation of the resource.</span></span>

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

