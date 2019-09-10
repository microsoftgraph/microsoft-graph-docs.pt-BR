---
title: Tipo de recurso workingHours
description: Representa os dias da semana e as horas de um fuso horário específico que o usuário trabalha.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: angelgolfer-ms
ms.openlocfilehash: 46f7cac83806dcf6fe1d4724da0a62a7929cd0c0
ms.sourcegitcommit: 3e7769ad097e9c34233fa5fea83afa23c34e14a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/10/2019
ms.locfileid: "36822722"
---
# <a name="workinghours-resource-type"></a><span data-ttu-id="4b297-103">Tipo de recurso workingHours</span><span class="sxs-lookup"><span data-stu-id="4b297-103">workingHours resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4b297-104">Representa os dias da semana e as horas de um fuso horário específico que o usuário trabalha.</span><span class="sxs-lookup"><span data-stu-id="4b297-104">Represents the days of the week and hours in a specific time zone that the user works.</span></span>

<span data-ttu-id="4b297-105">Ter acesso ao horário de trabalho de um usuário é útil em cenários que lidam com o planejamento de atividades ou recursos.</span><span class="sxs-lookup"><span data-stu-id="4b297-105">Having access to a user's working hours is useful in scenarios that handle activity or resource planning.</span></span> <span data-ttu-id="4b297-106">Você pode [obter](../api/user-get-mailboxsettings.md#example-3) e [definir](../api/user-update-mailboxsettings.md#example-2) o horário de trabalho de um usuário como parte das [configurações da caixa de correio](mailboxsettings.md) do usuário.</span><span class="sxs-lookup"><span data-stu-id="4b297-106">You can [get](../api/user-get-mailboxsettings.md#example-3) and [set](../api/user-update-mailboxsettings.md#example-2) the working hours of a user as part of the user's [mailbox settings](mailboxsettings.md).</span></span> 

<span data-ttu-id="4b297-107">Você pode optar por definir um fuso horário para seu horário de trabalho de maneira diferente do fuso horário definido no seu cliente do Outlook.</span><span class="sxs-lookup"><span data-stu-id="4b297-107">You can choose to set a time zone for your working hours differently from the time zone you have set on your Outlook client.</span></span> <span data-ttu-id="4b297-108">Isso pode ser útil em casos como quando você viaja para um fuso horário diferente daquele no qual você normalmente trabalha.</span><span class="sxs-lookup"><span data-stu-id="4b297-108">This can be useful in cases like when you travel to a different time zone than you usually work in.</span></span> <span data-ttu-id="4b297-109">É possível configurar o cliente do Outlook</span><span class="sxs-lookup"><span data-stu-id="4b297-109">You can set the Outlook client</span></span>  
<span data-ttu-id="4b297-110">no fuso horário de destino para que os valores de tempo do Outlook sejam exibidos no horário local enquanto você estiver lá.</span><span class="sxs-lookup"><span data-stu-id="4b297-110">to the destination time zone so that Outlook time values are displayed in local time while you are there.</span></span>
<span data-ttu-id="4b297-111">Quando outras pessoas solicitarem reuniões de trabalho com você no seu local habitual de trabalho, elas ainda poderão respeitar seu horário de trabalho no fuso horário apropriado.</span><span class="sxs-lookup"><span data-stu-id="4b297-111">When other people request work meetings with you in your usual place of work, they can still respect your working hours in the appropriate time zone.</span></span>


## <a name="properties"></a><span data-ttu-id="4b297-112">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4b297-112">Properties</span></span>
| <span data-ttu-id="4b297-113">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4b297-113">Property</span></span>     | <span data-ttu-id="4b297-114">Tipo</span><span class="sxs-lookup"><span data-stu-id="4b297-114">Type</span></span>   |<span data-ttu-id="4b297-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="4b297-115">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4b297-116">daysOfWeek</span><span class="sxs-lookup"><span data-stu-id="4b297-116">daysOfWeek</span></span> | <span data-ttu-id="4b297-117">coleção dayOfWeek</span><span class="sxs-lookup"><span data-stu-id="4b297-117">dayOfWeek collection</span></span> | <span data-ttu-id="4b297-118">Os dias da semana em que o usuário trabalha.</span><span class="sxs-lookup"><span data-stu-id="4b297-118">The days of the week on which the user works.</span></span> |
| <span data-ttu-id="4b297-119">startTime</span><span class="sxs-lookup"><span data-stu-id="4b297-119">startTime</span></span> | <span data-ttu-id="4b297-120">Edm.TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="4b297-120">Edm.TimeOfDay</span></span> | <span data-ttu-id="4b297-121">A hora do dia em que o usuário começa a trabalhar.</span><span class="sxs-lookup"><span data-stu-id="4b297-121">The time of the day that the user starts working.</span></span> |
| <span data-ttu-id="4b297-122">endTime</span><span class="sxs-lookup"><span data-stu-id="4b297-122">endTime</span></span> | <span data-ttu-id="4b297-123">Edm.TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="4b297-123">Edm.TimeOfDay</span></span> | <span data-ttu-id="4b297-124">A hora do dia em que o usuário para de trabalhar.</span><span class="sxs-lookup"><span data-stu-id="4b297-124">The time of the day that the user stops working.</span></span> |
| <span data-ttu-id="4b297-125">timeZone</span><span class="sxs-lookup"><span data-stu-id="4b297-125">timeZone</span></span> | [<span data-ttu-id="4b297-126">timeZoneBase</span><span class="sxs-lookup"><span data-stu-id="4b297-126">timeZoneBase</span></span>](timezonebase.md) | <span data-ttu-id="4b297-127">O fuso horário ao qual o horário de trabalho se aplica.</span><span class="sxs-lookup"><span data-stu-id="4b297-127">The time zone to which the working hours apply.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4b297-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4b297-128">JSON representation</span></span>

<span data-ttu-id="4b297-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4b297-129">Here is a JSON representation of the resource.</span></span>

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
