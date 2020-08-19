---
title: Tipo de recurso followupFlag
description: 'Permite definir um sinalizador em um item para que o usuário acompanhe mais tarde. '
localization_priority: Normal
author: svpsiva
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 263d2c5552eabfed47210dd8d53b2ce14ba1be25
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812264"
---
# <a name="followupflag-resource-type"></a><span data-ttu-id="2a75d-103">Tipo de recurso followupFlag</span><span class="sxs-lookup"><span data-stu-id="2a75d-103">followupFlag resource type</span></span>

<span data-ttu-id="2a75d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2a75d-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="2a75d-105">Permite definir um sinalizador em um item para que o usuário acompanhe mais tarde.</span><span class="sxs-lookup"><span data-stu-id="2a75d-105">Allows setting a flag in an item for the user to follow up on later.</span></span>

## <a name="properties"></a><span data-ttu-id="2a75d-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2a75d-106">Properties</span></span>
| <span data-ttu-id="2a75d-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2a75d-107">Property</span></span>     | <span data-ttu-id="2a75d-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="2a75d-108">Type</span></span>   |<span data-ttu-id="2a75d-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="2a75d-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2a75d-110">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="2a75d-110">completedDateTime</span></span>|[<span data-ttu-id="2a75d-111">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="2a75d-111">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="2a75d-112">Data e hora em que o acompanhamento foi concluído.</span><span class="sxs-lookup"><span data-stu-id="2a75d-112">The date and time that the follow-up was finished.</span></span>|
|<span data-ttu-id="2a75d-113">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="2a75d-113">dueDateTime</span></span>|<span data-ttu-id="2a75d-114">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="2a75d-114">**dateTimeTimeZone**</span></span>|<span data-ttu-id="2a75d-115">A data e a hora em que o acompanhamento deve ser concluído.</span><span class="sxs-lookup"><span data-stu-id="2a75d-115">The date and time that the follow up is to be finished.</span></span> <span data-ttu-id="2a75d-116">**Observação**: para definir a data de conclusão, você também deve especificar o `startDateTime` ; caso contrário, você receberá uma `400 Bad Request` resposta.</span><span class="sxs-lookup"><span data-stu-id="2a75d-116">**Note**: To set the due date, you must also specify the `startDateTime`; otherwise, you will get a `400 Bad Request` response.</span></span>|
|<span data-ttu-id="2a75d-117">flagStatus</span><span class="sxs-lookup"><span data-stu-id="2a75d-117">flagStatus</span></span>|<span data-ttu-id="2a75d-118">followupFlagStatus</span><span class="sxs-lookup"><span data-stu-id="2a75d-118">followupFlagStatus</span></span>|<span data-ttu-id="2a75d-119">O status de acompanhamento de um item.</span><span class="sxs-lookup"><span data-stu-id="2a75d-119">The status for follow-up for an item.</span></span> <span data-ttu-id="2a75d-120">Os valores possíveis são: `notFlagged`, `complete` e `flagged`.</span><span class="sxs-lookup"><span data-stu-id="2a75d-120">Possible values are `notFlagged`, `complete`, and `flagged`.</span></span>|
|<span data-ttu-id="2a75d-121">startDateTime</span><span class="sxs-lookup"><span data-stu-id="2a75d-121">startDateTime</span></span>|<span data-ttu-id="2a75d-122">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="2a75d-122">**dateTimeTimeZone**</span></span>|<span data-ttu-id="2a75d-123">Data e hora em que o acompanhamento deve começar.</span><span class="sxs-lookup"><span data-stu-id="2a75d-123">The date and time that the follow-up is to begin.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2a75d-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2a75d-124">JSON representation</span></span>

<span data-ttu-id="2a75d-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2a75d-125">Here is a JSON representation of the resource.</span></span>

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
