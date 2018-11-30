---
title: tipo de recurso de bookingWorkHours
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
ms.openlocfilehash: 3346ee8eb20e381e1412dcfb16624954658c44fd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036667"
---
# <a name="bookingworkhours-resource-type"></a><span data-ttu-id="1be1a-104">tipo de recurso de bookingWorkHours</span><span class="sxs-lookup"><span data-stu-id="1be1a-104">bookingWorkHours resource type</span></span>

 > <span data-ttu-id="1be1a-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="1be1a-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1be1a-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="1be1a-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="1be1a-107">Representa o conjunto de horário de trabalho em um único dia da semana, para um [bookingBusiness](bookingbusiness.md) ou [bookingStaffMember](bookingstaffmember.md).</span><span class="sxs-lookup"><span data-stu-id="1be1a-107">Represents the set of working hours in a single day of the week, for a [bookingBusiness](bookingbusiness.md) or [bookingStaffMember](bookingstaffmember.md).</span></span>

## <a name="properties"></a><span data-ttu-id="1be1a-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1be1a-108">Properties</span></span>
| <span data-ttu-id="1be1a-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1be1a-109">Property</span></span>     | <span data-ttu-id="1be1a-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="1be1a-110">Type</span></span>   |<span data-ttu-id="1be1a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="1be1a-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1be1a-112">dia</span><span class="sxs-lookup"><span data-stu-id="1be1a-112">day</span></span>|<span data-ttu-id="1be1a-113">String</span><span class="sxs-lookup"><span data-stu-id="1be1a-113">String</span></span>| <span data-ttu-id="1be1a-114">O dia da semana representado por esta instância.</span><span class="sxs-lookup"><span data-stu-id="1be1a-114">The day of the week represented by this instance.</span></span> <span data-ttu-id="1be1a-115">Os valores possíveis são: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="1be1a-115">Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="1be1a-116">intervalos de tempo</span><span class="sxs-lookup"><span data-stu-id="1be1a-116">timeSlots</span></span>|<span data-ttu-id="1be1a-117">coleção [bookingWorkTimeSlot](bookingworktimeslot.md)</span><span class="sxs-lookup"><span data-stu-id="1be1a-117">[bookingWorkTimeSlot](bookingworktimeslot.md) collection</span></span>|<span data-ttu-id="1be1a-118">Uma lista de horas de início/término durante um dia.</span><span class="sxs-lookup"><span data-stu-id="1be1a-118">A list of start/end times during a day.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1be1a-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1be1a-119">JSON representation</span></span>

<span data-ttu-id="1be1a-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1be1a-120">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "bookingWorkHours resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->