---
title: tipo de recurso automaticRepliesMailTips
description: Dicas de correio sobre as respostas automáticas que foram configuradas em uma caixa de correio.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 74fda9db7de1a97ce2b7e44ca9d56020b87ab6f9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974245"
---
# <a name="automaticrepliesmailtips-resource-type"></a><span data-ttu-id="867d4-103">tipo de recurso automaticRepliesMailTips</span><span class="sxs-lookup"><span data-stu-id="867d4-103">automaticRepliesMailTips resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="867d4-104">[Dicas](../resources/mailtips.md) de correio sobre as respostas automáticas que foram configuradas em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="867d4-104">[MailTips](../resources/mailtips.md) about any automatic replies that have been set up on a mailbox.</span></span>

## <a name="properties"></a><span data-ttu-id="867d4-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="867d4-105">Properties</span></span>
| <span data-ttu-id="867d4-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="867d4-106">Property</span></span>     | <span data-ttu-id="867d4-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="867d4-107">Type</span></span>   |<span data-ttu-id="867d4-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="867d4-108">Description</span></span>|
|:-----|:-----|:-----|
| <span data-ttu-id="867d4-109">mensagem</span><span class="sxs-lookup"><span data-stu-id="867d4-109">message</span></span> | <span data-ttu-id="867d4-110">String</span><span class="sxs-lookup"><span data-stu-id="867d4-110">String</span></span> | <span data-ttu-id="867d4-111">A mensagem de resposta automática.</span><span class="sxs-lookup"><span data-stu-id="867d4-111">The automatic reply message.</span></span> |
| <span data-ttu-id="867d4-112">messageLanguage</span><span class="sxs-lookup"><span data-stu-id="867d4-112">messageLanguage</span></span> | [<span data-ttu-id="867d4-113">localeInfo</span><span class="sxs-lookup"><span data-stu-id="867d4-113">localeInfo</span></span>](../resources/localeinfo.md) | <span data-ttu-id="867d4-114">O idioma em que a mensagem de resposta automática está.</span><span class="sxs-lookup"><span data-stu-id="867d4-114">The language that the automatic reply message is in.</span></span> |
| <span data-ttu-id="867d4-115">scheduledEndTime</span><span class="sxs-lookup"><span data-stu-id="867d4-115">scheduledEndTime</span></span> | [<span data-ttu-id="867d4-116">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="867d4-116">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md) | <span data-ttu-id="867d4-117">A data e a hora em que as respostas automáticas estão definidas para terminar.</span><span class="sxs-lookup"><span data-stu-id="867d4-117">The date and time that automatic replies are set to end.</span></span> |
| <span data-ttu-id="867d4-118">scheduledStartTime</span><span class="sxs-lookup"><span data-stu-id="867d4-118">scheduledStartTime</span></span> | [<span data-ttu-id="867d4-119">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="867d4-119">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md) | <span data-ttu-id="867d4-120">A data e a hora em que as respostas automáticas estão definidas para começar.</span><span class="sxs-lookup"><span data-stu-id="867d4-120">The date and time that automatic replies are set to begin.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="867d4-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="867d4-121">JSON representation</span></span>

<span data-ttu-id="867d4-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="867d4-122">Here is a JSON representation of the resource.</span></span>

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
