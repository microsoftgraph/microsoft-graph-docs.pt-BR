---
title: tipo de recurso scheduleItem
description: Um item que descreve a disponibilidade de um usuário correspondente a um evento real no calendário padrão do usuário. Esse item também se aplica a um recurso.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-teams
author: ''
ms.openlocfilehash: f2901412dcf1d52d8b117afa214da159b4553a8a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008639"
---
# <a name="scheduleitem-resource-type"></a><span data-ttu-id="42fde-104">tipo de recurso scheduleItem</span><span class="sxs-lookup"><span data-stu-id="42fde-104">scheduleItem resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="42fde-105">Um item que descreve a disponibilidade de um usuário correspondente a um evento real no calendário padrão do usuário.</span><span class="sxs-lookup"><span data-stu-id="42fde-105">An item that describes the availability of a user corresponding to an actual event on the user's default calendar.</span></span> <span data-ttu-id="42fde-106">Este item se aplica a um recurso (sala ou equipamento) também.</span><span class="sxs-lookup"><span data-stu-id="42fde-106">This item applies to a resource (room or equipment) as well.</span></span>

## <a name="properties"></a><span data-ttu-id="42fde-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="42fde-107">Properties</span></span>
| <span data-ttu-id="42fde-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="42fde-108">Property</span></span>     | <span data-ttu-id="42fde-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="42fde-109">Type</span></span>   |<span data-ttu-id="42fde-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="42fde-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="42fde-111">end</span><span class="sxs-lookup"><span data-stu-id="42fde-111">end</span></span> |[<span data-ttu-id="42fde-112">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="42fde-112">dateTimeTimeZone</span></span>](datetimetimezone.md) |<span data-ttu-id="42fde-113">A data, a hora e o fuso horário em que o evento correspondente termina.</span><span class="sxs-lookup"><span data-stu-id="42fde-113">The date, time, and time zone that the corresponding event ends.</span></span> |
|<span data-ttu-id="42fde-114">IsPrivate</span><span class="sxs-lookup"><span data-stu-id="42fde-114">isPrivate</span></span> |<span data-ttu-id="42fde-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="42fde-115">Boolean</span></span> |<span data-ttu-id="42fde-116">A sensibilidade do evento correspondente.</span><span class="sxs-lookup"><span data-stu-id="42fde-116">The sensitivity of the corresponding event.</span></span> <span data-ttu-id="42fde-117">True se o evento estiver marcado `private`; caso contrário, false.</span><span class="sxs-lookup"><span data-stu-id="42fde-117">True if the event is marked `private`, false otherwise.</span></span> <span data-ttu-id="42fde-118">Opcional.</span><span class="sxs-lookup"><span data-stu-id="42fde-118">Optional.</span></span> |
|<span data-ttu-id="42fde-119">location</span><span class="sxs-lookup"><span data-stu-id="42fde-119">location</span></span> |<span data-ttu-id="42fde-120">String</span><span class="sxs-lookup"><span data-stu-id="42fde-120">String</span></span> | <span data-ttu-id="42fde-121">O local onde o evento correspondente é mantido ou participado.</span><span class="sxs-lookup"><span data-stu-id="42fde-121">The location where the corresponding event is held or attended from.</span></span> <span data-ttu-id="42fde-122">Opcional.</span><span class="sxs-lookup"><span data-stu-id="42fde-122">Optional.</span></span>|
|<span data-ttu-id="42fde-123">iniciar</span><span class="sxs-lookup"><span data-stu-id="42fde-123">start</span></span> |[<span data-ttu-id="42fde-124">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="42fde-124">dateTimeTimeZone</span></span>](datetimetimezone.md) |<span data-ttu-id="42fde-125">A data, a hora e o fuso horário em que o evento correspondente é iniciado.</span><span class="sxs-lookup"><span data-stu-id="42fde-125">The date, time, and time zone that the corresponding event starts.</span></span> |
|<span data-ttu-id="42fde-126">status</span><span class="sxs-lookup"><span data-stu-id="42fde-126">status</span></span> |<span data-ttu-id="42fde-127">freeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="42fde-127">freeBusyStatus</span></span> | <span data-ttu-id="42fde-128">O status de disponibilidade do usuário ou recurso durante o evento correspondente.</span><span class="sxs-lookup"><span data-stu-id="42fde-128">The availability status of the user or resource during the corresponding event.</span></span> <span data-ttu-id="42fde-129">Os valores possíveis são: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="42fde-129">The possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span> |
|<span data-ttu-id="42fde-130">subject</span><span class="sxs-lookup"><span data-stu-id="42fde-130">subject</span></span> |<span data-ttu-id="42fde-131">String</span><span class="sxs-lookup"><span data-stu-id="42fde-131">String</span></span> | <span data-ttu-id="42fde-132">A linha de assunto do evento correspondente.</span><span class="sxs-lookup"><span data-stu-id="42fde-132">The corresponding event's subject line.</span></span> <span data-ttu-id="42fde-133">Opcional.</span><span class="sxs-lookup"><span data-stu-id="42fde-133">Optional.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="42fde-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="42fde-134">JSON representation</span></span>

<span data-ttu-id="42fde-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="42fde-135">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "isPrivate",
    "location",
    "subject"
  ],
  "@odata.type": "microsoft.graph.scheduleItem"
}-->

```json
{
  "end": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "isPrivate": true,
  "location": "String",
  "start": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "status": "String",
  "subject": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "scheduleItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
