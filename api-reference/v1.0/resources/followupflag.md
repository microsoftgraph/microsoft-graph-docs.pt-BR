---
title: Tipo de recurso followupFlag
description: 'Permite definir um sinalizador em um item para que o usuário acompanhe posteriormente. '
localization_priority: Normal
author: abheek-das
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 9b690c86a6ccbef6f5c215e268f7b34243e3023e
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50130203"
---
# <a name="followupflag-resource-type"></a><span data-ttu-id="0ecd1-103">Tipo de recurso followupFlag</span><span class="sxs-lookup"><span data-stu-id="0ecd1-103">followupFlag resource type</span></span>

<span data-ttu-id="0ecd1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0ecd1-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="0ecd1-105">Permite definir um sinalizador em um item para que o usuário acompanhe posteriormente.</span><span class="sxs-lookup"><span data-stu-id="0ecd1-105">Allows setting a flag in an item for the user to follow up on later.</span></span>

## <a name="properties"></a><span data-ttu-id="0ecd1-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0ecd1-106">Properties</span></span>
| <span data-ttu-id="0ecd1-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0ecd1-107">Property</span></span>     | <span data-ttu-id="0ecd1-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="0ecd1-108">Type</span></span>   |<span data-ttu-id="0ecd1-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="0ecd1-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0ecd1-110">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="0ecd1-110">completedDateTime</span></span>|[<span data-ttu-id="0ecd1-111">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="0ecd1-111">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="0ecd1-112">Data e hora em que o acompanhamento foi concluído.</span><span class="sxs-lookup"><span data-stu-id="0ecd1-112">The date and time that the follow-up was finished.</span></span>|
|<span data-ttu-id="0ecd1-113">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="0ecd1-113">dueDateTime</span></span>|<span data-ttu-id="0ecd1-114">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="0ecd1-114">**dateTimeTimeZone**</span></span>|<span data-ttu-id="0ecd1-115">A data e a hora em que o acompanhamento deve ser concluído.</span><span class="sxs-lookup"><span data-stu-id="0ecd1-115">The date and time that the follow up is to be finished.</span></span> <span data-ttu-id="0ecd1-116">**Observação:** para definir a data de vencimento, você também deve especificar o ; `startDateTime` caso contrário, você receberá uma `400 Bad Request` resposta.</span><span class="sxs-lookup"><span data-stu-id="0ecd1-116">**Note**: To set the due date, you must also specify the `startDateTime`; otherwise, you will get a `400 Bad Request` response.</span></span>|
|<span data-ttu-id="0ecd1-117">flagStatus</span><span class="sxs-lookup"><span data-stu-id="0ecd1-117">flagStatus</span></span>|<span data-ttu-id="0ecd1-118">followupFlagStatus</span><span class="sxs-lookup"><span data-stu-id="0ecd1-118">followupFlagStatus</span></span>|<span data-ttu-id="0ecd1-119">O status de acompanhamento de um item.</span><span class="sxs-lookup"><span data-stu-id="0ecd1-119">The status for follow-up for an item.</span></span> <span data-ttu-id="0ecd1-120">Os valores possíveis são: `notFlagged`, `complete` e `flagged`.</span><span class="sxs-lookup"><span data-stu-id="0ecd1-120">Possible values are `notFlagged`, `complete`, and `flagged`.</span></span>|
|<span data-ttu-id="0ecd1-121">startDateTime</span><span class="sxs-lookup"><span data-stu-id="0ecd1-121">startDateTime</span></span>|<span data-ttu-id="0ecd1-122">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="0ecd1-122">**dateTimeTimeZone**</span></span>|<span data-ttu-id="0ecd1-123">Data e hora em que o acompanhamento deve começar.</span><span class="sxs-lookup"><span data-stu-id="0ecd1-123">The date and time that the follow-up is to begin.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0ecd1-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0ecd1-124">JSON representation</span></span>

<span data-ttu-id="0ecd1-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0ecd1-125">Here is a JSON representation of the resource.</span></span>

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

