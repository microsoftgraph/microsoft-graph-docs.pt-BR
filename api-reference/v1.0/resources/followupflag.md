---
title: Tipo de recurso followupFlag
description: 'Permite a definição de um sinalizador em um item para o usuário acompanhar posteriormente. '
ms.openlocfilehash: 5aa9d82fc90d7142717ac5ef05f9d837bac371ba
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006991"
---
# <a name="followupflag-resource-type"></a><span data-ttu-id="45abf-103">Tipo de recurso followupFlag</span><span class="sxs-lookup"><span data-stu-id="45abf-103">followupFlag resource type</span></span>


<span data-ttu-id="45abf-104">Permite a definição de um sinalizador em um item para o usuário acompanhar posteriormente.</span><span class="sxs-lookup"><span data-stu-id="45abf-104">Allows setting a flag in an item for the user to follow up on later.</span></span> 

## <a name="properties"></a><span data-ttu-id="45abf-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="45abf-105">Properties</span></span>
| <span data-ttu-id="45abf-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="45abf-106">Property</span></span>     | <span data-ttu-id="45abf-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="45abf-107">Type</span></span>   |<span data-ttu-id="45abf-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="45abf-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="45abf-109">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="45abf-109">completedDateTime</span></span>|[<span data-ttu-id="45abf-110">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="45abf-110">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="45abf-111">Data e hora em que o acompanhamento foi concluído.</span><span class="sxs-lookup"><span data-stu-id="45abf-111">The date and time that the follow-up was finished.</span></span>|
|<span data-ttu-id="45abf-112">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="45abf-112">dueDateTime</span></span>|<span data-ttu-id="45abf-113">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="45abf-113">**dateTimeTimeZone**</span></span>|<span data-ttu-id="45abf-114">Data e hora em que o acompanhamento deve ser concluído.</span><span class="sxs-lookup"><span data-stu-id="45abf-114">The date and time that the follow-up is to be finished.</span></span>|
|<span data-ttu-id="45abf-115">flagStatus</span><span class="sxs-lookup"><span data-stu-id="45abf-115">flagStatus</span></span>|<span data-ttu-id="45abf-116">followupFlagStatus</span><span class="sxs-lookup"><span data-stu-id="45abf-116">followupFlagStatus</span></span>|<span data-ttu-id="45abf-117">O status de acompanhamento de um item.</span><span class="sxs-lookup"><span data-stu-id="45abf-117">The status for follow-up for an item.</span></span> <span data-ttu-id="45abf-118">Os valores possíveis são: `notFlagged`, `complete` e `flagged`.</span><span class="sxs-lookup"><span data-stu-id="45abf-118">Possible values are `notFlagged`, `complete`, and `flagged`.</span></span>|
|<span data-ttu-id="45abf-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="45abf-119">startDateTime</span></span>|<span data-ttu-id="45abf-120">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="45abf-120">**dateTimeTimeZone**</span></span>|<span data-ttu-id="45abf-121">Data e hora em que o acompanhamento deve começar.</span><span class="sxs-lookup"><span data-stu-id="45abf-121">The date and time that the follow-up is to begin.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="45abf-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="45abf-122">JSON representation</span></span>

<span data-ttu-id="45abf-123">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="45abf-123">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.followupFlag"
}-->

```json
{
  "completedDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "dueDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "flagStatus": "String",
  "startDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "followupFlag resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
