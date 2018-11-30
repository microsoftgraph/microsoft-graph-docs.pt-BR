---
title: Tipo de recurso workingHours
description: Representa os dias da semana e as horas de um fuso horário específico que o usuário trabalha.
ms.openlocfilehash: 915ec185931d3f7e77f010517a3ef0c3bff92204
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038570"
---
# <a name="workinghours-resource-type"></a><span data-ttu-id="2c8fe-103">Tipo de recurso workingHours</span><span class="sxs-lookup"><span data-stu-id="2c8fe-103">workingHours resource type</span></span>

> <span data-ttu-id="2c8fe-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="2c8fe-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2c8fe-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="2c8fe-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2c8fe-106">Representa os dias da semana e as horas de um fuso horário específico que o usuário trabalha.</span><span class="sxs-lookup"><span data-stu-id="2c8fe-106">Represents the days of the week and hours in a specific time zone that the user works.</span></span>

<span data-ttu-id="2c8fe-107">Ter acesso ao horário de trabalho de um usuário é útil em cenários que lidam com o planejamento de atividades ou recursos.</span><span class="sxs-lookup"><span data-stu-id="2c8fe-107">Having access to a user's working hours is useful in scenarios that handle activity or resource planning.</span></span> <span data-ttu-id="2c8fe-108">Você pode [obter](../api/user-get-mailboxsettings.md#request-3) e [definir](../api/user-update-mailboxsettings.md#request-2) o horário de trabalho de um usuário como parte das [configurações da caixa de correio](mailboxsettings.md) do usuário.</span><span class="sxs-lookup"><span data-stu-id="2c8fe-108">You can [get](../api/user-get-mailboxsettings.md#request-3) and [set](../api/user-update-mailboxsettings.md#request-2) the working hours of a user as part of the user's [mailbox settings](mailboxsettings.md).</span></span> 

<span data-ttu-id="2c8fe-109">Você pode optar por definir um fuso horário para seu horário de trabalho de maneira diferente do fuso horário definido no seu cliente do Outlook.</span><span class="sxs-lookup"><span data-stu-id="2c8fe-109">You can choose to set a time zone for your working hours differently from the time zone you have set on your Outlook client.</span></span> <span data-ttu-id="2c8fe-110">Isso pode ser útil em casos como quando você viaja para um fuso horário diferente daquele no qual você normalmente trabalha.</span><span class="sxs-lookup"><span data-stu-id="2c8fe-110">This can be useful in cases like when you travel to a different time zone than you usually work in.</span></span> <span data-ttu-id="2c8fe-111">É possível configurar o cliente do Outlook</span><span class="sxs-lookup"><span data-stu-id="2c8fe-111">You can set the Outlook client</span></span>  
<span data-ttu-id="2c8fe-112">no fuso horário de destino para que os valores de tempo do Outlook sejam exibidos no horário local enquanto você estiver lá.</span><span class="sxs-lookup"><span data-stu-id="2c8fe-112">to the destination time zone so that Outlook time values are displayed in local time while you are there.</span></span>
<span data-ttu-id="2c8fe-113">Quando outras pessoas solicitarem reuniões de trabalho com você no seu local habitual de trabalho, elas ainda poderão respeitar seu horário de trabalho no fuso horário apropriado.</span><span class="sxs-lookup"><span data-stu-id="2c8fe-113">When other people request work meetings with you in your usual place of work, they can still respect your working hours in the appropriate time zone.</span></span>


## <a name="properties"></a><span data-ttu-id="2c8fe-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2c8fe-114">Properties</span></span>
| <span data-ttu-id="2c8fe-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2c8fe-115">Property</span></span>     | <span data-ttu-id="2c8fe-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="2c8fe-116">Type</span></span>   |<span data-ttu-id="2c8fe-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="2c8fe-117">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2c8fe-118">daysOfWeek</span><span class="sxs-lookup"><span data-stu-id="2c8fe-118">daysOfWeek</span></span> | <span data-ttu-id="2c8fe-119">Coleção de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2c8fe-119">String collection</span></span> | <span data-ttu-id="2c8fe-120">Os dias da semana em que o usuário trabalha.</span><span class="sxs-lookup"><span data-stu-id="2c8fe-120">The days of the week on which the user works.</span></span> |
| <span data-ttu-id="2c8fe-121">startTime</span><span class="sxs-lookup"><span data-stu-id="2c8fe-121">startTime</span></span> | <span data-ttu-id="2c8fe-122">Edm.TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="2c8fe-122">Edm.TimeOfDay</span></span> | <span data-ttu-id="2c8fe-123">A hora do dia em que o usuário começa a trabalhar.</span><span class="sxs-lookup"><span data-stu-id="2c8fe-123">The time of the day that the user starts working.</span></span> |
| <span data-ttu-id="2c8fe-124">endTime</span><span class="sxs-lookup"><span data-stu-id="2c8fe-124">endTime</span></span> | <span data-ttu-id="2c8fe-125">Edm.TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="2c8fe-125">Edm.TimeOfDay</span></span> | <span data-ttu-id="2c8fe-126">A hora do dia em que o usuário para de trabalhar.</span><span class="sxs-lookup"><span data-stu-id="2c8fe-126">The time of the day that the user stops working.</span></span> |
| <span data-ttu-id="2c8fe-127">timeZone</span><span class="sxs-lookup"><span data-stu-id="2c8fe-127">timeZone</span></span> | [<span data-ttu-id="2c8fe-128">timeZoneBase</span><span class="sxs-lookup"><span data-stu-id="2c8fe-128">timeZoneBase</span></span>](timezonebase.md) | <span data-ttu-id="2c8fe-129">O fuso horário ao qual o horário de trabalho se aplica.</span><span class="sxs-lookup"><span data-stu-id="2c8fe-129">The time zone to which the working hours apply.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="2c8fe-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2c8fe-130">JSON representation</span></span>

<span data-ttu-id="2c8fe-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2c8fe-131">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workingHours"
}-->

```json
{
  "daysOfWeek": ["string"],
  "startTime": "TimeOfDay",
  "endTime": "TimeOfDay",
  "timeZone": {"@odata.type": "microsoft.graph.timeZoneBase"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "workingHours resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->