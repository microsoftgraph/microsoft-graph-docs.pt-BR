---
title: Tipo de recurso workingHours
description: Representa os dias da semana e as horas de um fuso horário específico que o usuário trabalha.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: angelgolfer-ms
ms.openlocfilehash: 67a61c5ca767f00c32bf568cea4e495d5b0909ac
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519068"
---
# <a name="workinghours-resource-type"></a><span data-ttu-id="47a75-103">Tipo de recurso workingHours</span><span class="sxs-lookup"><span data-stu-id="47a75-103">workingHours resource type</span></span>

<span data-ttu-id="47a75-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="47a75-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="47a75-105">Representa os dias da semana e as horas de um fuso horário específico que o usuário trabalha.</span><span class="sxs-lookup"><span data-stu-id="47a75-105">Represents the days of the week and hours in a specific time zone that the user works.</span></span>

<span data-ttu-id="47a75-106">Ter acesso ao horário de trabalho de um usuário é útil em cenários que lidam com o planejamento de atividades ou recursos.</span><span class="sxs-lookup"><span data-stu-id="47a75-106">Having access to a user's working hours is useful in scenarios that handle activity or resource planning.</span></span> <span data-ttu-id="47a75-107">Você pode [obter](../api/user-get-mailboxsettings.md#example-3) e [definir](../api/user-update-mailboxsettings.md#example-2) o horário de trabalho de um usuário como parte das [configurações da caixa de correio](mailboxsettings.md) do usuário.</span><span class="sxs-lookup"><span data-stu-id="47a75-107">You can [get](../api/user-get-mailboxsettings.md#example-3) and [set](../api/user-update-mailboxsettings.md#example-2) the working hours of a user as part of the user's [mailbox settings](mailboxsettings.md).</span></span> 

<span data-ttu-id="47a75-108">Você pode optar por definir um fuso horário para seu horário de trabalho de maneira diferente do fuso horário definido no seu cliente do Outlook.</span><span class="sxs-lookup"><span data-stu-id="47a75-108">You can choose to set a time zone for your working hours differently from the time zone you have set on your Outlook client.</span></span> <span data-ttu-id="47a75-109">Isso pode ser útil em casos como quando você viaja para um fuso horário diferente daquele no qual você normalmente trabalha.</span><span class="sxs-lookup"><span data-stu-id="47a75-109">This can be useful in cases like when you travel to a different time zone than you usually work in.</span></span> <span data-ttu-id="47a75-110">É possível configurar o cliente do Outlook</span><span class="sxs-lookup"><span data-stu-id="47a75-110">You can set the Outlook client</span></span>  
<span data-ttu-id="47a75-111">no fuso horário de destino para que os valores de tempo do Outlook sejam exibidos no horário local enquanto você estiver lá.</span><span class="sxs-lookup"><span data-stu-id="47a75-111">to the destination time zone so that Outlook time values are displayed in local time while you are there.</span></span>
<span data-ttu-id="47a75-112">Quando outras pessoas solicitarem reuniões de trabalho com você no seu local habitual de trabalho, elas ainda poderão respeitar seu horário de trabalho no fuso horário apropriado.</span><span class="sxs-lookup"><span data-stu-id="47a75-112">When other people request work meetings with you in your usual place of work, they can still respect your working hours in the appropriate time zone.</span></span>


## <a name="properties"></a><span data-ttu-id="47a75-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="47a75-113">Properties</span></span>
| <span data-ttu-id="47a75-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="47a75-114">Property</span></span>     | <span data-ttu-id="47a75-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="47a75-115">Type</span></span>   |<span data-ttu-id="47a75-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="47a75-116">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="47a75-117">daysOfWeek</span><span class="sxs-lookup"><span data-stu-id="47a75-117">daysOfWeek</span></span> | <span data-ttu-id="47a75-118">coleção dayOfWeek</span><span class="sxs-lookup"><span data-stu-id="47a75-118">dayOfWeek collection</span></span> | <span data-ttu-id="47a75-119">Os dias da semana em que o usuário trabalha.</span><span class="sxs-lookup"><span data-stu-id="47a75-119">The days of the week on which the user works.</span></span> |
| <span data-ttu-id="47a75-120">startTime</span><span class="sxs-lookup"><span data-stu-id="47a75-120">startTime</span></span> | <span data-ttu-id="47a75-121">Edm.TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="47a75-121">Edm.TimeOfDay</span></span> | <span data-ttu-id="47a75-122">A hora do dia em que o usuário começa a trabalhar.</span><span class="sxs-lookup"><span data-stu-id="47a75-122">The time of the day that the user starts working.</span></span> |
| <span data-ttu-id="47a75-123">endTime</span><span class="sxs-lookup"><span data-stu-id="47a75-123">endTime</span></span> | <span data-ttu-id="47a75-124">Edm.TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="47a75-124">Edm.TimeOfDay</span></span> | <span data-ttu-id="47a75-125">A hora do dia em que o usuário para de trabalhar.</span><span class="sxs-lookup"><span data-stu-id="47a75-125">The time of the day that the user stops working.</span></span> |
| <span data-ttu-id="47a75-126">timeZone</span><span class="sxs-lookup"><span data-stu-id="47a75-126">timeZone</span></span> | [<span data-ttu-id="47a75-127">timeZoneBase</span><span class="sxs-lookup"><span data-stu-id="47a75-127">timeZoneBase</span></span>](timezonebase.md) | <span data-ttu-id="47a75-128">O fuso horário ao qual o horário de trabalho se aplica.</span><span class="sxs-lookup"><span data-stu-id="47a75-128">The time zone to which the working hours apply.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="47a75-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="47a75-129">JSON representation</span></span>

<span data-ttu-id="47a75-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="47a75-130">Here is a JSON representation of the resource.</span></span>

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
