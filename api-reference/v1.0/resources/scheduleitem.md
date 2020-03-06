---
title: tipo de recurso scheduleItem
description: Um item que descreve a disponibilidade de um usuário correspondente a um evento real no calendário padrão do usuário. Este item se aplica a um recurso (sala ou equipamento) também.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 4136b71dfb273525e8793521d50545ee5b1873cb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533795"
---
# <a name="scheduleitem-resource-type"></a><span data-ttu-id="dd1d3-104">tipo de recurso scheduleItem</span><span class="sxs-lookup"><span data-stu-id="dd1d3-104">scheduleItem resource type</span></span>

<span data-ttu-id="dd1d3-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dd1d3-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="dd1d3-106">Um item que descreve a disponibilidade de um usuário correspondente a um evento real no calendário padrão do usuário.</span><span class="sxs-lookup"><span data-stu-id="dd1d3-106">An item that describes the availability of a user corresponding to an actual event on the user's default calendar.</span></span> <span data-ttu-id="dd1d3-107">Este item se aplica a um recurso (sala ou equipamento) também.</span><span class="sxs-lookup"><span data-stu-id="dd1d3-107">This item applies to a resource (room or equipment) as well.</span></span>

## <a name="properties"></a><span data-ttu-id="dd1d3-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="dd1d3-108">Properties</span></span>
| <span data-ttu-id="dd1d3-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dd1d3-109">Property</span></span>     | <span data-ttu-id="dd1d3-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="dd1d3-110">Type</span></span>   |<span data-ttu-id="dd1d3-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="dd1d3-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dd1d3-112">end</span><span class="sxs-lookup"><span data-stu-id="dd1d3-112">end</span></span> |[<span data-ttu-id="dd1d3-113">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="dd1d3-113">dateTimeTimeZone</span></span>](datetimetimezone.md) |<span data-ttu-id="dd1d3-114">A data, a hora e o fuso horário em que o evento correspondente termina.</span><span class="sxs-lookup"><span data-stu-id="dd1d3-114">The date, time, and time zone that the corresponding event ends.</span></span> |
|<span data-ttu-id="dd1d3-115">IsPrivate</span><span class="sxs-lookup"><span data-stu-id="dd1d3-115">isPrivate</span></span> |<span data-ttu-id="dd1d3-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="dd1d3-116">Boolean</span></span> |<span data-ttu-id="dd1d3-117">A sensibilidade do evento correspondente.</span><span class="sxs-lookup"><span data-stu-id="dd1d3-117">The sensitivity of the corresponding event.</span></span> <span data-ttu-id="dd1d3-118">True se o evento estiver marcado `private`; caso contrário, false.</span><span class="sxs-lookup"><span data-stu-id="dd1d3-118">True if the event is marked `private`, false otherwise.</span></span> <span data-ttu-id="dd1d3-119">Opcional.</span><span class="sxs-lookup"><span data-stu-id="dd1d3-119">Optional.</span></span>|
|<span data-ttu-id="dd1d3-120">location</span><span class="sxs-lookup"><span data-stu-id="dd1d3-120">location</span></span> |<span data-ttu-id="dd1d3-121">String</span><span class="sxs-lookup"><span data-stu-id="dd1d3-121">String</span></span> | <span data-ttu-id="dd1d3-122">O local onde o evento correspondente é mantido ou participado.</span><span class="sxs-lookup"><span data-stu-id="dd1d3-122">The location where the corresponding event is held or attended from.</span></span> <span data-ttu-id="dd1d3-123">Opcional.</span><span class="sxs-lookup"><span data-stu-id="dd1d3-123">Optional.</span></span>|
|<span data-ttu-id="dd1d3-124">iniciar</span><span class="sxs-lookup"><span data-stu-id="dd1d3-124">start</span></span> |[<span data-ttu-id="dd1d3-125">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="dd1d3-125">dateTimeTimeZone</span></span>](datetimetimezone.md) |<span data-ttu-id="dd1d3-126">A data, a hora e o fuso horário em que o evento correspondente é iniciado.</span><span class="sxs-lookup"><span data-stu-id="dd1d3-126">The date, time, and time zone that the corresponding event starts.</span></span> |
|<span data-ttu-id="dd1d3-127">status</span><span class="sxs-lookup"><span data-stu-id="dd1d3-127">status</span></span> |<span data-ttu-id="dd1d3-128">freeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="dd1d3-128">freeBusyStatus</span></span> | <span data-ttu-id="dd1d3-129">O status de disponibilidade do usuário ou recurso durante o evento correspondente.</span><span class="sxs-lookup"><span data-stu-id="dd1d3-129">The availability status of the user or resource during the corresponding event.</span></span> <span data-ttu-id="dd1d3-130">Os valores possíveis são: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="dd1d3-130">The possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span> |
|<span data-ttu-id="dd1d3-131">subject</span><span class="sxs-lookup"><span data-stu-id="dd1d3-131">subject</span></span> |<span data-ttu-id="dd1d3-132">String</span><span class="sxs-lookup"><span data-stu-id="dd1d3-132">String</span></span> | <span data-ttu-id="dd1d3-133">A linha de assunto do evento correspondente.</span><span class="sxs-lookup"><span data-stu-id="dd1d3-133">The corresponding event's subject line.</span></span> <span data-ttu-id="dd1d3-134">Opcional.</span><span class="sxs-lookup"><span data-stu-id="dd1d3-134">Optional.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="dd1d3-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="dd1d3-135">JSON representation</span></span>

<span data-ttu-id="dd1d3-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="dd1d3-136">The following is a JSON representation of the resource.</span></span>

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
  "tocPath": ""
}
-->
