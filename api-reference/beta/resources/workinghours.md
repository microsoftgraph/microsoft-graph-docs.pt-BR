---
title: Tipo de recurso workingHours
description: Representa os dias da semana e as horas de um fuso horário específico que o usuário trabalha.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: abheek-das
ms.openlocfilehash: 5e86df6eae7d1ae399cb764321e8fc2af1815409
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50472395"
---
# <a name="workinghours-resource-type"></a><span data-ttu-id="b9327-103">Tipo de recurso workingHours</span><span class="sxs-lookup"><span data-stu-id="b9327-103">workingHours resource type</span></span>

<span data-ttu-id="b9327-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b9327-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b9327-105">Representa os dias da semana e as horas de um fuso horário específico que o usuário trabalha.</span><span class="sxs-lookup"><span data-stu-id="b9327-105">Represents the days of the week and hours in a specific time zone that the user works.</span></span>

<span data-ttu-id="b9327-106">Ter acesso ao horário de trabalho de um usuário é útil em cenários que lidam com o planejamento de atividades ou recursos.</span><span class="sxs-lookup"><span data-stu-id="b9327-106">Having access to a user's working hours is useful in scenarios that handle activity or resource planning.</span></span> <span data-ttu-id="b9327-107">Você pode [obter](../api/user-get-mailboxsettings.md#example-3) e [definir](../api/user-update-mailboxsettings.md#example-2) o horário de trabalho de um usuário como parte das [configurações da caixa de correio](mailboxsettings.md) do usuário.</span><span class="sxs-lookup"><span data-stu-id="b9327-107">You can [get](../api/user-get-mailboxsettings.md#example-3) and [set](../api/user-update-mailboxsettings.md#example-2) the working hours of a user as part of the user's [mailbox settings](mailboxsettings.md).</span></span> 

<span data-ttu-id="b9327-108">Você pode optar por definir um fuso horário para seu horário de trabalho de maneira diferente do fuso horário definido no seu cliente do Outlook.</span><span class="sxs-lookup"><span data-stu-id="b9327-108">You can choose to set a time zone for your working hours differently from the time zone you have set on your Outlook client.</span></span> <span data-ttu-id="b9327-109">Isso pode ser útil em casos como quando você viaja para um fuso horário diferente daquele no qual você normalmente trabalha.</span><span class="sxs-lookup"><span data-stu-id="b9327-109">This can be useful in cases like when you travel to a different time zone than you usually work in.</span></span> <span data-ttu-id="b9327-110">É possível configurar o cliente do Outlook</span><span class="sxs-lookup"><span data-stu-id="b9327-110">You can set the Outlook client</span></span>  
<span data-ttu-id="b9327-111">no fuso horário de destino para que os valores de tempo do Outlook sejam exibidos no horário local enquanto você estiver lá.</span><span class="sxs-lookup"><span data-stu-id="b9327-111">to the destination time zone so that Outlook time values are displayed in local time while you are there.</span></span>
<span data-ttu-id="b9327-112">Quando outras pessoas solicitarem reuniões de trabalho com você no seu local habitual de trabalho, elas ainda poderão respeitar seu horário de trabalho no fuso horário apropriado.</span><span class="sxs-lookup"><span data-stu-id="b9327-112">When other people request work meetings with you in your usual place of work, they can still respect your working hours in the appropriate time zone.</span></span>


## <a name="properties"></a><span data-ttu-id="b9327-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b9327-113">Properties</span></span>
| <span data-ttu-id="b9327-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b9327-114">Property</span></span>     | <span data-ttu-id="b9327-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="b9327-115">Type</span></span>   |<span data-ttu-id="b9327-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="b9327-116">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b9327-117">daysOfWeek</span><span class="sxs-lookup"><span data-stu-id="b9327-117">daysOfWeek</span></span> | <span data-ttu-id="b9327-118">Coleção dayOfWeek</span><span class="sxs-lookup"><span data-stu-id="b9327-118">dayOfWeek collection</span></span> | <span data-ttu-id="b9327-119">Os dias da semana em que o usuário trabalha.</span><span class="sxs-lookup"><span data-stu-id="b9327-119">The days of the week on which the user works.</span></span> |
| <span data-ttu-id="b9327-120">startTime</span><span class="sxs-lookup"><span data-stu-id="b9327-120">startTime</span></span> | <span data-ttu-id="b9327-121">Edm.TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="b9327-121">Edm.TimeOfDay</span></span> | <span data-ttu-id="b9327-122">A hora do dia em que o usuário começa a trabalhar.</span><span class="sxs-lookup"><span data-stu-id="b9327-122">The time of the day that the user starts working.</span></span> |
| <span data-ttu-id="b9327-123">endTime</span><span class="sxs-lookup"><span data-stu-id="b9327-123">endTime</span></span> | <span data-ttu-id="b9327-124">Edm.TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="b9327-124">Edm.TimeOfDay</span></span> | <span data-ttu-id="b9327-125">A hora do dia em que o usuário para de trabalhar.</span><span class="sxs-lookup"><span data-stu-id="b9327-125">The time of the day that the user stops working.</span></span> |
| <span data-ttu-id="b9327-126">timeZone</span><span class="sxs-lookup"><span data-stu-id="b9327-126">timeZone</span></span> | [<span data-ttu-id="b9327-127">timeZoneBase</span><span class="sxs-lookup"><span data-stu-id="b9327-127">timeZoneBase</span></span>](timezonebase.md) | <span data-ttu-id="b9327-128">O fuso horário ao qual o horário de trabalho se aplica.</span><span class="sxs-lookup"><span data-stu-id="b9327-128">The time zone to which the working hours apply.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b9327-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b9327-129">JSON representation</span></span>

<span data-ttu-id="b9327-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b9327-130">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workingHours"
}-->

```json
{
  "daysOfWeek": ["string"],
  "startTime": "string (TimeOfDay)",
  "endTime": "string (TimeOfDay)",
  "timeZone": {"@odata.type": "microsoft.graph.timeZoneBase"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "workingHours resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


