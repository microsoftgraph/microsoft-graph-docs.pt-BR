---
title: tipo de recurso bookingWorkHours
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 389b035dcef92db166e4290c71160c12842dc887
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33338849"
---
# <a name="bookingworkhours-resource-type"></a><span data-ttu-id="3eb66-104">tipo de recurso bookingWorkHours</span><span class="sxs-lookup"><span data-stu-id="3eb66-104">bookingWorkHours resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="3eb66-105">Representa o conjunto de horas de trabalho em um único dia da semana, para um [bookingBusiness](bookingbusiness.md) ou [bookingStaffMember](bookingstaffmember.md).</span><span class="sxs-lookup"><span data-stu-id="3eb66-105">Represents the set of working hours in a single day of the week, for a [bookingBusiness](bookingbusiness.md) or [bookingStaffMember](bookingstaffmember.md).</span></span>

## <a name="properties"></a><span data-ttu-id="3eb66-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3eb66-106">Properties</span></span>
| <span data-ttu-id="3eb66-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3eb66-107">Property</span></span>     | <span data-ttu-id="3eb66-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="3eb66-108">Type</span></span>   |<span data-ttu-id="3eb66-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="3eb66-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3eb66-110">dia</span><span class="sxs-lookup"><span data-stu-id="3eb66-110">day</span></span>|<span data-ttu-id="3eb66-111">String</span><span class="sxs-lookup"><span data-stu-id="3eb66-111">String</span></span>| <span data-ttu-id="3eb66-112">O dia da semana representado por esta instância.</span><span class="sxs-lookup"><span data-stu-id="3eb66-112">The day of the week represented by this instance.</span></span> <span data-ttu-id="3eb66-113">Os valores possíveis são: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="3eb66-113">Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="3eb66-114">Intervalos</span><span class="sxs-lookup"><span data-stu-id="3eb66-114">timeSlots</span></span>|<span data-ttu-id="3eb66-115">coleção [bookingWorkTimeSlot](bookingworktimeslot.md)</span><span class="sxs-lookup"><span data-stu-id="3eb66-115">[bookingWorkTimeSlot](bookingworktimeslot.md) collection</span></span>|<span data-ttu-id="3eb66-116">Uma lista de horários de início/término durante um dia.</span><span class="sxs-lookup"><span data-stu-id="3eb66-116">A list of start/end times during a day.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3eb66-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3eb66-117">JSON representation</span></span>

<span data-ttu-id="3eb66-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3eb66-118">The following is a JSON representation of the resource.</span></span>

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
