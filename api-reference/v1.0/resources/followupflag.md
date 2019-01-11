---
title: Tipo de recurso followupFlag
description: 'Permite a definição de um sinalizador em um item para o usuário acompanhar posteriormente. '
localization_priority: Normal
ms.openlocfilehash: 60d2e40a10c3ba5b2af9aa798b84aadaebedd57a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27885495"
---
# <a name="followupflag-resource-type"></a><span data-ttu-id="a3ade-103">Tipo de recurso followupFlag</span><span class="sxs-lookup"><span data-stu-id="a3ade-103">followupFlag resource type</span></span>


<span data-ttu-id="a3ade-104">Permite a definição de um sinalizador em um item para o usuário acompanhar posteriormente.</span><span class="sxs-lookup"><span data-stu-id="a3ade-104">Allows setting a flag in an item for the user to follow up on later.</span></span> 

## <a name="properties"></a><span data-ttu-id="a3ade-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a3ade-105">Properties</span></span>
| <span data-ttu-id="a3ade-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a3ade-106">Property</span></span>     | <span data-ttu-id="a3ade-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="a3ade-107">Type</span></span>   |<span data-ttu-id="a3ade-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="a3ade-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a3ade-109">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="a3ade-109">completedDateTime</span></span>|[<span data-ttu-id="a3ade-110">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="a3ade-110">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="a3ade-111">Data e hora em que o acompanhamento foi concluído.</span><span class="sxs-lookup"><span data-stu-id="a3ade-111">The date and time that the follow-up was finished.</span></span>|
|<span data-ttu-id="a3ade-112">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="a3ade-112">dueDateTime</span></span>|<span data-ttu-id="a3ade-113">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="a3ade-113">**dateTimeTimeZone**</span></span>|<span data-ttu-id="a3ade-114">Data e hora em que o acompanhamento deve ser concluído.</span><span class="sxs-lookup"><span data-stu-id="a3ade-114">The date and time that the follow-up is to be finished.</span></span>|
|<span data-ttu-id="a3ade-115">flagStatus</span><span class="sxs-lookup"><span data-stu-id="a3ade-115">flagStatus</span></span>|<span data-ttu-id="a3ade-116">followupFlagStatus</span><span class="sxs-lookup"><span data-stu-id="a3ade-116">followupFlagStatus</span></span>|<span data-ttu-id="a3ade-117">O status de acompanhamento de um item.</span><span class="sxs-lookup"><span data-stu-id="a3ade-117">The status for follow-up for an item.</span></span> <span data-ttu-id="a3ade-118">Os valores possíveis são: `notFlagged`, `complete` e `flagged`.</span><span class="sxs-lookup"><span data-stu-id="a3ade-118">Possible values are `notFlagged`, `complete`, and `flagged`.</span></span>|
|<span data-ttu-id="a3ade-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="a3ade-119">startDateTime</span></span>|<span data-ttu-id="a3ade-120">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="a3ade-120">**dateTimeTimeZone**</span></span>|<span data-ttu-id="a3ade-121">Data e hora em que o acompanhamento deve começar.</span><span class="sxs-lookup"><span data-stu-id="a3ade-121">The date and time that the follow-up is to begin.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a3ade-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a3ade-122">JSON representation</span></span>

<span data-ttu-id="a3ade-123">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="a3ade-123">Here is a JSON representation of the resource</span></span>

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
