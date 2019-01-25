---
title: Tipo de recurso followupFlag
description: Permite definir um sinalizador para que o usuário possa acompanhar um item posteriormente. Os itens com suporte incluem message e contact.
localization_priority: Normal
ms.openlocfilehash: f8ae4cdc04b48fe0b6dede437684215cefb75969
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509543"
---
# <a name="followupflag-resource-type"></a><span data-ttu-id="d3503-104">Tipo de recurso followupFlag</span><span class="sxs-lookup"><span data-stu-id="d3503-104">followupFlag resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d3503-105">Permite definir um sinalizador para que o usuário possa acompanhar um item posteriormente.</span><span class="sxs-lookup"><span data-stu-id="d3503-105">Allows setting a flag for the user to follow up on an item later.</span></span> <span data-ttu-id="d3503-106">Os itens com suporte incluem [message](message.md) e [contact](contact.md).</span><span class="sxs-lookup"><span data-stu-id="d3503-106">Supported items include [message](message.md) and [contact](contact.md).</span></span>

## <a name="properties"></a><span data-ttu-id="d3503-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d3503-107">Properties</span></span>
| <span data-ttu-id="d3503-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d3503-108">Property</span></span>     | <span data-ttu-id="d3503-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="d3503-109">Type</span></span>   |<span data-ttu-id="d3503-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="d3503-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d3503-111">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="d3503-111">completedDateTime</span></span>|[<span data-ttu-id="d3503-112">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="d3503-112">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="d3503-113">Data e hora em que o acompanhamento foi concluído.</span><span class="sxs-lookup"><span data-stu-id="d3503-113">The date and time that the follow-up was finished.</span></span>|
|<span data-ttu-id="d3503-114">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="d3503-114">dueDateTime</span></span>|<span data-ttu-id="d3503-115">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="d3503-115">**dateTimeTimeZone**</span></span>|<span data-ttu-id="d3503-116">Data e hora em que o acompanhamento deve ser concluído.</span><span class="sxs-lookup"><span data-stu-id="d3503-116">The date and time that the follow-up is to be finished.</span></span>|
|<span data-ttu-id="d3503-117">flagStatus</span><span class="sxs-lookup"><span data-stu-id="d3503-117">flagStatus</span></span>|<span data-ttu-id="d3503-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d3503-118">String</span></span>|<span data-ttu-id="d3503-119">O status de acompanhamento de um item.</span><span class="sxs-lookup"><span data-stu-id="d3503-119">The status for follow-up for an item.</span></span> <span data-ttu-id="d3503-120">Os valores possíveis são: `notFlagged`, `complete` e `flagged`.</span><span class="sxs-lookup"><span data-stu-id="d3503-120">Possible values are `notFlagged`, `complete`, and `flagged`.</span></span>|
|<span data-ttu-id="d3503-121">startDateTime</span><span class="sxs-lookup"><span data-stu-id="d3503-121">startDateTime</span></span>|<span data-ttu-id="d3503-122">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="d3503-122">**dateTimeTimeZone**</span></span>|<span data-ttu-id="d3503-123">Data e hora em que o acompanhamento deve começar.</span><span class="sxs-lookup"><span data-stu-id="d3503-123">The date and time that the follow-up is to begin.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d3503-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d3503-124">JSON representation</span></span>

<span data-ttu-id="d3503-125">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="d3503-125">Here is a JSON representation of the resource</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/followupflag.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
