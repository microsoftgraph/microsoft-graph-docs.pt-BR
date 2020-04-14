---
title: tipo de recurso bookingWorkHours
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: fab0282e3ce380b8aa4283bd9a783fe8b2fc3390
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43463597"
---
# <a name="bookingworkhours-resource-type"></a><span data-ttu-id="0a796-104">tipo de recurso bookingWorkHours</span><span class="sxs-lookup"><span data-stu-id="0a796-104">bookingWorkHours resource type</span></span>

<span data-ttu-id="0a796-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0a796-105">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="0a796-106">Representa o conjunto de horas de trabalho em um único dia da semana, para um [bookingBusiness](bookingbusiness.md) ou [bookingStaffMember](bookingstaffmember.md).</span><span class="sxs-lookup"><span data-stu-id="0a796-106">Represents the set of working hours in a single day of the week, for a [bookingBusiness](bookingbusiness.md) or [bookingStaffMember](bookingstaffmember.md).</span></span>

## <a name="properties"></a><span data-ttu-id="0a796-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0a796-107">Properties</span></span>
| <span data-ttu-id="0a796-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0a796-108">Property</span></span>     | <span data-ttu-id="0a796-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="0a796-109">Type</span></span>   |<span data-ttu-id="0a796-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="0a796-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0a796-111">dia</span><span class="sxs-lookup"><span data-stu-id="0a796-111">day</span></span>|<span data-ttu-id="0a796-112">String</span><span class="sxs-lookup"><span data-stu-id="0a796-112">String</span></span>| <span data-ttu-id="0a796-113">O dia da semana representado por esta instância.</span><span class="sxs-lookup"><span data-stu-id="0a796-113">The day of the week represented by this instance.</span></span> <span data-ttu-id="0a796-114">Os valores possíveis são: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="0a796-114">Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="0a796-115">Intervalos</span><span class="sxs-lookup"><span data-stu-id="0a796-115">timeSlots</span></span>|<span data-ttu-id="0a796-116">coleção [bookingWorkTimeSlot](bookingworktimeslot.md)</span><span class="sxs-lookup"><span data-stu-id="0a796-116">[bookingWorkTimeSlot](bookingworktimeslot.md) collection</span></span>|<span data-ttu-id="0a796-117">Uma lista de horários de início/término durante um dia.</span><span class="sxs-lookup"><span data-stu-id="0a796-117">A list of start/end times during a day.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0a796-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0a796-118">JSON representation</span></span>

<span data-ttu-id="0a796-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0a796-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingWorkHours"
}-->

```json
{
  "day": "String",
  "timeSlots": [{"@odata.type": "microsoft.graph.bookingWorkTimeSlot"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "bookingWorkHours resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
