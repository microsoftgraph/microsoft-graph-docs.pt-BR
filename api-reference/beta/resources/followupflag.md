---
title: Tipo de recurso followupFlag
description: Permite definir um sinalizador para que o usuário possa acompanhar um item posteriormente. Os itens com suporte incluem message e contact.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: abheek-das
ms.openlocfilehash: 4d075b36cf06db3d4c470ece46229c05c44949af
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50129452"
---
# <a name="followupflag-resource-type"></a><span data-ttu-id="07a35-104">Tipo de recurso followupFlag</span><span class="sxs-lookup"><span data-stu-id="07a35-104">followupFlag resource type</span></span>

<span data-ttu-id="07a35-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="07a35-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="07a35-106">Permite definir um sinalizador para que o usuário possa acompanhar um item posteriormente.</span><span class="sxs-lookup"><span data-stu-id="07a35-106">Allows setting a flag for the user to follow up on an item later.</span></span> <span data-ttu-id="07a35-107">Os itens com suporte incluem [message](message.md) e [contact](contact.md).</span><span class="sxs-lookup"><span data-stu-id="07a35-107">Supported items include [message](message.md) and [contact](contact.md).</span></span>

## <a name="properties"></a><span data-ttu-id="07a35-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="07a35-108">Properties</span></span>
| <span data-ttu-id="07a35-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="07a35-109">Property</span></span>     | <span data-ttu-id="07a35-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="07a35-110">Type</span></span>   |<span data-ttu-id="07a35-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="07a35-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="07a35-112">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="07a35-112">completedDateTime</span></span>|[<span data-ttu-id="07a35-113">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="07a35-113">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="07a35-114">Data e hora em que o acompanhamento foi concluído.</span><span class="sxs-lookup"><span data-stu-id="07a35-114">The date and time that the follow-up was finished.</span></span>|
|<span data-ttu-id="07a35-115">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="07a35-115">dueDateTime</span></span>|<span data-ttu-id="07a35-116">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="07a35-116">**dateTimeTimeZone**</span></span>|<span data-ttu-id="07a35-117">A data e a hora em que o acompanhamento deve ser concluído.</span><span class="sxs-lookup"><span data-stu-id="07a35-117">The date and time that the follow up is to be finished.</span></span> <span data-ttu-id="07a35-118">**Observação:** para definir a data de vencimento, você também deve especificar o ; `startDateTime` caso contrário, você receberá uma `400 Bad Request` resposta.</span><span class="sxs-lookup"><span data-stu-id="07a35-118">**Note**: To set the due date, you must also specify the `startDateTime`; otherwise, you will get a `400 Bad Request` response.</span></span>|
|<span data-ttu-id="07a35-119">flagStatus</span><span class="sxs-lookup"><span data-stu-id="07a35-119">flagStatus</span></span>|<span data-ttu-id="07a35-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="07a35-120">String</span></span>|<span data-ttu-id="07a35-121">O status de acompanhamento de um item.</span><span class="sxs-lookup"><span data-stu-id="07a35-121">The status for follow-up for an item.</span></span> <span data-ttu-id="07a35-122">Os valores possíveis são: `notFlagged`, `complete` e `flagged`.</span><span class="sxs-lookup"><span data-stu-id="07a35-122">Possible values are `notFlagged`, `complete`, and `flagged`.</span></span>|
|<span data-ttu-id="07a35-123">startDateTime</span><span class="sxs-lookup"><span data-stu-id="07a35-123">startDateTime</span></span>|<span data-ttu-id="07a35-124">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="07a35-124">**dateTimeTimeZone**</span></span>|<span data-ttu-id="07a35-125">Data e hora em que o acompanhamento deve começar.</span><span class="sxs-lookup"><span data-stu-id="07a35-125">The date and time that the follow-up is to begin.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="07a35-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="07a35-126">JSON representation</span></span>

<span data-ttu-id="07a35-127">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="07a35-127">Here is a JSON representation of the resource</span></span>

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


