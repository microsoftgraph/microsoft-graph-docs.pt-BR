---
title: Tipo de recurso workingHours
description: Representa os dias da semana e as horas de um fuso horário específico que o usuário trabalha.
localization_priority: Normal
ms.openlocfilehash: 8d0c0c96838af63cd0e1c665d23e54938b4ea34d
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573820"
---
# <a name="workinghours-resource-type"></a><span data-ttu-id="1fde3-103">Tipo de recurso workingHours</span><span class="sxs-lookup"><span data-stu-id="1fde3-103">workingHours resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1fde3-104">Representa os dias da semana e as horas de um fuso horário específico que o usuário trabalha.</span><span class="sxs-lookup"><span data-stu-id="1fde3-104">Represents the days of the week and hours in a specific time zone that the user works.</span></span>

<span data-ttu-id="1fde3-105">Ter acesso ao horário de trabalho de um usuário é útil em cenários que lidam com o planejamento de atividades ou recursos.</span><span class="sxs-lookup"><span data-stu-id="1fde3-105">Having access to a user's working hours is useful in scenarios that handle activity or resource planning.</span></span> <span data-ttu-id="1fde3-106">Você pode [obter](../api/user-get-mailboxsettings.md#request-3) e [definir](../api/user-update-mailboxsettings.md#request-2) o horário de trabalho de um usuário como parte das [configurações da caixa de correio](mailboxsettings.md) do usuário.</span><span class="sxs-lookup"><span data-stu-id="1fde3-106">You can [get](../api/user-get-mailboxsettings.md#request-3) and [set](../api/user-update-mailboxsettings.md#request-2) the working hours of a user as part of the user's [mailbox settings](mailboxsettings.md).</span></span> 

<span data-ttu-id="1fde3-107">Você pode optar por definir um fuso horário para seu horário de trabalho de maneira diferente do fuso horário definido no seu cliente do Outlook.</span><span class="sxs-lookup"><span data-stu-id="1fde3-107">You can choose to set a time zone for your working hours differently from the time zone you have set on your Outlook client.</span></span> <span data-ttu-id="1fde3-108">Isso pode ser útil em casos como quando você viaja para um fuso horário diferente daquele no qual você normalmente trabalha.</span><span class="sxs-lookup"><span data-stu-id="1fde3-108">This can be useful in cases like when you travel to a different time zone than you usually work in.</span></span> <span data-ttu-id="1fde3-109">É possível configurar o cliente do Outlook</span><span class="sxs-lookup"><span data-stu-id="1fde3-109">You can set the Outlook client</span></span>  
<span data-ttu-id="1fde3-110">no fuso horário de destino para que os valores de tempo do Outlook sejam exibidos no horário local enquanto você estiver lá.</span><span class="sxs-lookup"><span data-stu-id="1fde3-110">to the destination time zone so that Outlook time values are displayed in local time while you are there.</span></span>
<span data-ttu-id="1fde3-111">Quando outras pessoas solicitarem reuniões de trabalho com você no seu local habitual de trabalho, elas ainda poderão respeitar seu horário de trabalho no fuso horário apropriado.</span><span class="sxs-lookup"><span data-stu-id="1fde3-111">When other people request work meetings with you in your usual place of work, they can still respect your working hours in the appropriate time zone.</span></span>


## <a name="properties"></a><span data-ttu-id="1fde3-112">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1fde3-112">Properties</span></span>
| <span data-ttu-id="1fde3-113">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1fde3-113">Property</span></span>     | <span data-ttu-id="1fde3-114">Tipo</span><span class="sxs-lookup"><span data-stu-id="1fde3-114">Type</span></span>   |<span data-ttu-id="1fde3-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="1fde3-115">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1fde3-116">daysOfWeek</span><span class="sxs-lookup"><span data-stu-id="1fde3-116">daysOfWeek</span></span> | <span data-ttu-id="1fde3-117">coleção dayOfWeek</span><span class="sxs-lookup"><span data-stu-id="1fde3-117">dayOfWeek collection</span></span> | <span data-ttu-id="1fde3-118">Os dias da semana em que o usuário trabalha.</span><span class="sxs-lookup"><span data-stu-id="1fde3-118">The days of the week on which the user works.</span></span> |
| <span data-ttu-id="1fde3-119">startTime</span><span class="sxs-lookup"><span data-stu-id="1fde3-119">startTime</span></span> | <span data-ttu-id="1fde3-120">Cadeia de caracteres (TimeOfDay)</span><span class="sxs-lookup"><span data-stu-id="1fde3-120">String (TimeOfDay)</span></span> | <span data-ttu-id="1fde3-121">A hora do dia em que o usuário começa a trabalhar.</span><span class="sxs-lookup"><span data-stu-id="1fde3-121">The time of the day that the user starts working.</span></span> |
| <span data-ttu-id="1fde3-122">endTime</span><span class="sxs-lookup"><span data-stu-id="1fde3-122">endTime</span></span> | <span data-ttu-id="1fde3-123">Cadeia de caracteres (TimeOfDay)</span><span class="sxs-lookup"><span data-stu-id="1fde3-123">String (TimeOfDay)</span></span> | <span data-ttu-id="1fde3-124">A hora do dia em que o usuário para de trabalhar.</span><span class="sxs-lookup"><span data-stu-id="1fde3-124">The time of the day that the user stops working.</span></span> |
| <span data-ttu-id="1fde3-125">timeZone</span><span class="sxs-lookup"><span data-stu-id="1fde3-125">timeZone</span></span> | [<span data-ttu-id="1fde3-126">timeZoneBase</span><span class="sxs-lookup"><span data-stu-id="1fde3-126">timeZoneBase</span></span>](timezonebase.md) | <span data-ttu-id="1fde3-127">O fuso horário ao qual o horário de trabalho se aplica.</span><span class="sxs-lookup"><span data-stu-id="1fde3-127">The time zone to which the working hours apply.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="1fde3-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1fde3-128">JSON representation</span></span>

<span data-ttu-id="1fde3-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1fde3-129">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workingHours"
}-->

```json
{
  "daysOfWeek": ["dayOfWeek"],
  "startTime": "String (TimeOfDay)",
  "endTime": "String (TimeOfDay)",
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
  "suppressions": [
    "Error: /api-reference/beta/resources/workinghours.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
