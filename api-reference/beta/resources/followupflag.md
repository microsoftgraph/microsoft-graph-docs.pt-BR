---
title: Tipo de recurso followupFlag
description: Permite definir um sinalizador para que o usuário possa acompanhar um item posteriormente. Os itens com suporte incluem message e contact.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: svpsiva
ms.openlocfilehash: d8ad74c843cc3115034ff89b9711de067c0c482e
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46809819"
---
# <a name="followupflag-resource-type"></a><span data-ttu-id="921c5-104">Tipo de recurso followupFlag</span><span class="sxs-lookup"><span data-stu-id="921c5-104">followupFlag resource type</span></span>

<span data-ttu-id="921c5-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="921c5-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="921c5-106">Permite definir um sinalizador para que o usuário possa acompanhar um item posteriormente.</span><span class="sxs-lookup"><span data-stu-id="921c5-106">Allows setting a flag for the user to follow up on an item later.</span></span> <span data-ttu-id="921c5-107">Os itens com suporte incluem [message](message.md) e [contact](contact.md).</span><span class="sxs-lookup"><span data-stu-id="921c5-107">Supported items include [message](message.md) and [contact](contact.md).</span></span>

## <a name="properties"></a><span data-ttu-id="921c5-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="921c5-108">Properties</span></span>
| <span data-ttu-id="921c5-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="921c5-109">Property</span></span>     | <span data-ttu-id="921c5-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="921c5-110">Type</span></span>   |<span data-ttu-id="921c5-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="921c5-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="921c5-112">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="921c5-112">completedDateTime</span></span>|[<span data-ttu-id="921c5-113">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="921c5-113">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="921c5-114">Data e hora em que o acompanhamento foi concluído.</span><span class="sxs-lookup"><span data-stu-id="921c5-114">The date and time that the follow-up was finished.</span></span>|
|<span data-ttu-id="921c5-115">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="921c5-115">dueDateTime</span></span>|<span data-ttu-id="921c5-116">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="921c5-116">**dateTimeTimeZone**</span></span>|<span data-ttu-id="921c5-117">A data e a hora em que o acompanhamento deve ser concluído.</span><span class="sxs-lookup"><span data-stu-id="921c5-117">The date and time that the follow up is to be finished.</span></span> <span data-ttu-id="921c5-118">**Observação**: para definir a data de conclusão, você também deve especificar o `startDateTime` ; caso contrário, você receberá uma `400 Bad Request` resposta.</span><span class="sxs-lookup"><span data-stu-id="921c5-118">**Note**: To set the due date, you must also specify the `startDateTime`; otherwise, you will get a `400 Bad Request` response.</span></span>|
|<span data-ttu-id="921c5-119">flagStatus</span><span class="sxs-lookup"><span data-stu-id="921c5-119">flagStatus</span></span>|<span data-ttu-id="921c5-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="921c5-120">String</span></span>|<span data-ttu-id="921c5-121">O status de acompanhamento de um item.</span><span class="sxs-lookup"><span data-stu-id="921c5-121">The status for follow-up for an item.</span></span> <span data-ttu-id="921c5-122">Os valores possíveis são: `notFlagged`, `complete` e `flagged`.</span><span class="sxs-lookup"><span data-stu-id="921c5-122">Possible values are `notFlagged`, `complete`, and `flagged`.</span></span>|
|<span data-ttu-id="921c5-123">startDateTime</span><span class="sxs-lookup"><span data-stu-id="921c5-123">startDateTime</span></span>|<span data-ttu-id="921c5-124">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="921c5-124">**dateTimeTimeZone**</span></span>|<span data-ttu-id="921c5-125">Data e hora em que o acompanhamento deve começar.</span><span class="sxs-lookup"><span data-stu-id="921c5-125">The date and time that the follow-up is to begin.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="921c5-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="921c5-126">JSON representation</span></span>

<span data-ttu-id="921c5-127">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="921c5-127">Here is a JSON representation of the resource</span></span>

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
