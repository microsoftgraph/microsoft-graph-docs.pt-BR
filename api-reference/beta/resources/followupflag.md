---
title: Tipo de recurso followupFlag
description: Permite definir um sinalizador para que o usuário possa acompanhar um item posteriormente. Os itens com suporte incluem message e contact.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 9f69eca77fbeb7b9501c1f9186d0e00199a08658
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42497829"
---
# <a name="followupflag-resource-type"></a><span data-ttu-id="0bf76-104">Tipo de recurso followupFlag</span><span class="sxs-lookup"><span data-stu-id="0bf76-104">followupFlag resource type</span></span>

<span data-ttu-id="0bf76-105">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="0bf76-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0bf76-106">Permite definir um sinalizador para que o usuário possa acompanhar um item posteriormente.</span><span class="sxs-lookup"><span data-stu-id="0bf76-106">Allows setting a flag for the user to follow up on an item later.</span></span> <span data-ttu-id="0bf76-107">Os itens com suporte incluem [message](message.md) e [contact](contact.md).</span><span class="sxs-lookup"><span data-stu-id="0bf76-107">Supported items include [message](message.md) and [contact](contact.md).</span></span>

## <a name="properties"></a><span data-ttu-id="0bf76-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0bf76-108">Properties</span></span>
| <span data-ttu-id="0bf76-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0bf76-109">Property</span></span>     | <span data-ttu-id="0bf76-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="0bf76-110">Type</span></span>   |<span data-ttu-id="0bf76-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="0bf76-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0bf76-112">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="0bf76-112">completedDateTime</span></span>|[<span data-ttu-id="0bf76-113">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="0bf76-113">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="0bf76-114">Data e hora em que o acompanhamento foi concluído.</span><span class="sxs-lookup"><span data-stu-id="0bf76-114">The date and time that the follow-up was finished.</span></span>|
|<span data-ttu-id="0bf76-115">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="0bf76-115">dueDateTime</span></span>|<span data-ttu-id="0bf76-116">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="0bf76-116">**dateTimeTimeZone**</span></span>|<span data-ttu-id="0bf76-117">Data e hora em que o acompanhamento deve ser concluído.</span><span class="sxs-lookup"><span data-stu-id="0bf76-117">The date and time that the follow-up is to be finished.</span></span>|
|<span data-ttu-id="0bf76-118">flagStatus</span><span class="sxs-lookup"><span data-stu-id="0bf76-118">flagStatus</span></span>|<span data-ttu-id="0bf76-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0bf76-119">String</span></span>|<span data-ttu-id="0bf76-120">O status de acompanhamento de um item.</span><span class="sxs-lookup"><span data-stu-id="0bf76-120">The status for follow-up for an item.</span></span> <span data-ttu-id="0bf76-121">Os valores possíveis são: `notFlagged`, `complete` e `flagged`.</span><span class="sxs-lookup"><span data-stu-id="0bf76-121">Possible values are `notFlagged`, `complete`, and `flagged`.</span></span>|
|<span data-ttu-id="0bf76-122">startDateTime</span><span class="sxs-lookup"><span data-stu-id="0bf76-122">startDateTime</span></span>|<span data-ttu-id="0bf76-123">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="0bf76-123">**dateTimeTimeZone**</span></span>|<span data-ttu-id="0bf76-124">Data e hora em que o acompanhamento deve começar.</span><span class="sxs-lookup"><span data-stu-id="0bf76-124">The date and time that the follow-up is to begin.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0bf76-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0bf76-125">JSON representation</span></span>

<span data-ttu-id="0bf76-126">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="0bf76-126">Here is a JSON representation of the resource</span></span>

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
