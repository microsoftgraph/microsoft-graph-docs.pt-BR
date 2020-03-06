---
title: tipo de recurso automaticRepliesMailTips
description: Dicas de correio sobre as respostas automáticas que foram configuradas em uma caixa de correio.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: fc7d7c5c6a3560435c4e61a8953887f5b6b61324
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532045"
---
# <a name="automaticrepliesmailtips-resource-type"></a><span data-ttu-id="d6108-103">tipo de recurso automaticRepliesMailTips</span><span class="sxs-lookup"><span data-stu-id="d6108-103">automaticRepliesMailTips resource type</span></span>

<span data-ttu-id="d6108-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d6108-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="d6108-105">[Dicas](../resources/mailtips.md) de correio sobre as respostas automáticas que foram configuradas em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="d6108-105">[MailTips](../resources/mailtips.md) about any automatic replies that have been set up on a mailbox.</span></span>

## <a name="properties"></a><span data-ttu-id="d6108-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d6108-106">Properties</span></span>
| <span data-ttu-id="d6108-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d6108-107">Property</span></span>     | <span data-ttu-id="d6108-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="d6108-108">Type</span></span>   |<span data-ttu-id="d6108-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="d6108-109">Description</span></span>|
|:-----|:-----|:-----|
| <span data-ttu-id="d6108-110">mensagem</span><span class="sxs-lookup"><span data-stu-id="d6108-110">message</span></span> | <span data-ttu-id="d6108-111">String</span><span class="sxs-lookup"><span data-stu-id="d6108-111">String</span></span> | <span data-ttu-id="d6108-112">A mensagem de resposta automática.</span><span class="sxs-lookup"><span data-stu-id="d6108-112">The automatic reply message.</span></span> |
| <span data-ttu-id="d6108-113">messageLanguage</span><span class="sxs-lookup"><span data-stu-id="d6108-113">messageLanguage</span></span> | [<span data-ttu-id="d6108-114">localeInfo</span><span class="sxs-lookup"><span data-stu-id="d6108-114">localeInfo</span></span>](../resources/localeinfo.md) | <span data-ttu-id="d6108-115">O idioma em que a mensagem de resposta automática está.</span><span class="sxs-lookup"><span data-stu-id="d6108-115">The language that the automatic reply message is in.</span></span> |
| <span data-ttu-id="d6108-116">scheduledEndTime</span><span class="sxs-lookup"><span data-stu-id="d6108-116">scheduledEndTime</span></span> | [<span data-ttu-id="d6108-117">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="d6108-117">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md) | <span data-ttu-id="d6108-118">A data e a hora em que as respostas automáticas estão definidas para terminar.</span><span class="sxs-lookup"><span data-stu-id="d6108-118">The date and time that automatic replies are set to end.</span></span> |
| <span data-ttu-id="d6108-119">scheduledStartTime</span><span class="sxs-lookup"><span data-stu-id="d6108-119">scheduledStartTime</span></span> | [<span data-ttu-id="d6108-120">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="d6108-120">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md) | <span data-ttu-id="d6108-121">A data e a hora em que as respostas automáticas estão definidas para começar.</span><span class="sxs-lookup"><span data-stu-id="d6108-121">The date and time that automatic replies are set to begin.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d6108-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d6108-122">JSON representation</span></span>

<span data-ttu-id="d6108-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d6108-123">Here is a JSON representation of the resource.</span></span>

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
