---
title: Tipo de recurso followupFlag
description: Permite definir um sinalizador para que o usuário possa acompanhar um item posteriormente. Os itens com suporte incluem message e contact.
localization_priority: Normal
ms.openlocfilehash: dff12190b984d87ced6a75f2562a6b79dee53b44
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340248"
---
# <a name="followupflag-resource-type"></a><span data-ttu-id="00080-104">Tipo de recurso followupFlag</span><span class="sxs-lookup"><span data-stu-id="00080-104">followupFlag resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="00080-105">Permite definir um sinalizador para que o usuário possa acompanhar um item posteriormente.</span><span class="sxs-lookup"><span data-stu-id="00080-105">Allows setting a flag for the user to follow up on an item later.</span></span> <span data-ttu-id="00080-106">Os itens com suporte incluem [message](message.md) e [contact](contact.md).</span><span class="sxs-lookup"><span data-stu-id="00080-106">Supported items include [message](message.md) and [contact](contact.md).</span></span>

## <a name="properties"></a><span data-ttu-id="00080-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="00080-107">Properties</span></span>
| <span data-ttu-id="00080-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="00080-108">Property</span></span>     | <span data-ttu-id="00080-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="00080-109">Type</span></span>   |<span data-ttu-id="00080-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="00080-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="00080-111">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="00080-111">completedDateTime</span></span>|[<span data-ttu-id="00080-112">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="00080-112">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="00080-113">Data e hora em que o acompanhamento foi concluído.</span><span class="sxs-lookup"><span data-stu-id="00080-113">The date and time that the follow-up was finished.</span></span>|
|<span data-ttu-id="00080-114">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="00080-114">dueDateTime</span></span>|<span data-ttu-id="00080-115">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="00080-115">**dateTimeTimeZone**</span></span>|<span data-ttu-id="00080-116">Data e hora em que o acompanhamento deve ser concluído.</span><span class="sxs-lookup"><span data-stu-id="00080-116">The date and time that the follow-up is to be finished.</span></span>|
|<span data-ttu-id="00080-117">flagStatus</span><span class="sxs-lookup"><span data-stu-id="00080-117">flagStatus</span></span>|<span data-ttu-id="00080-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="00080-118">String</span></span>|<span data-ttu-id="00080-119">O status de acompanhamento de um item.</span><span class="sxs-lookup"><span data-stu-id="00080-119">The status for follow-up for an item.</span></span> <span data-ttu-id="00080-120">Os valores possíveis são: `notFlagged`, `complete` e `flagged`.</span><span class="sxs-lookup"><span data-stu-id="00080-120">Possible values are `notFlagged`, `complete`, and `flagged`.</span></span>|
|<span data-ttu-id="00080-121">startDateTime</span><span class="sxs-lookup"><span data-stu-id="00080-121">startDateTime</span></span>|<span data-ttu-id="00080-122">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="00080-122">**dateTimeTimeZone**</span></span>|<span data-ttu-id="00080-123">Data e hora em que o acompanhamento deve começar.</span><span class="sxs-lookup"><span data-stu-id="00080-123">The date and time that the follow-up is to begin.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="00080-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="00080-124">JSON representation</span></span>

<span data-ttu-id="00080-125">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="00080-125">Here is a JSON representation of the resource</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "followupFlag resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
